# xfyun 项目示例模板


## 模板内容

1. Dockerfile模板

参考 `docker/golang/multi/Dockerfile` 进行多阶段构建，构建最终产物镜像会非常小，根据需要选用

参考 `docker/golang/single/Dockerfile`阶段构建， 产物镜像大小依赖于基础镜像，和本次构建产物大小

2. Github CI Action模板

参考 `.github/workflows/ci.yaml` 进行ci配置， 产物最终推送到 aws的docker公共仓库  iflytek-open 仓库下，


以上均为模板，复制对应文件到自己项目下进行对应配置即可， ci action yaml依赖的 docker仓库秘钥已全局配置到xfyun组织下，可直接使用，无需更改。

