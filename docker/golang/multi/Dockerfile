FROM golang:1.17-bullseye as go-builder

# 多阶段构建， 下面写你的 构建逻辑，最终镜像大小为 from镜像大小+ 本次构建step产生layer层大小

RUN make


FROM alpine:latest as final
# 第二阶段基础镜像为alpine， 非常小的基础镜像


ENV TZ Asia/Shanghai
RUN apk add tzdata && cp /usr/share/zoneinfo/${TZ} /etc/localtime \
    && echo ${TZ} > /etc/timezone

## 这一步是从 go-builder阶段拷贝 编译产物到本阶段， 因为构建过程很多依赖在真正运行时并不需要，因此可以减小最终构建产物大小
COPY --from=go-builder /workspace/bin/linux .
#RUN set -eux && sed -i 's/dl-cdn.alpinelinux.org/mirrors.ustc.edu.cn/g' /etc/apk/repositories






