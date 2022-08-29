# iflytek开源项目示例模板

***本Readme只提供一个样例模板，具体部分操作以实际项目为主***

本篇为readme.md文件模板

## 模板内容


![AthenaServing](logo.png)

# XXXX

[![Build Status](https://travis-ci.com/xfyun/AthenaServing.svg?branch=master)](https://travis-ci.com/xfyun/AthenaServing)
[![Language](https://img.shields.io/badge/Language-Go-blue.svg)](https://golang.org/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/xfyun/AthenaServing/blob/master/LICENSE)
[![EN doc](https://img.shields.io/badge/document-English-blue.svg)](README_EN.md)
[![CN doc](https://img.shields.io/badge/文档-中文版-blue.svg)](README.md)

## 什么是 iflytek开源项目示例模板 ?

iflytek开源项目示例模板旨在提供待开源项目一个开源仓库范例


## 用途场景


1. 提供一些常用的Dockerfile模板

参考 [Dockerfile](docker/golang/multi/Dockerfile) 进行多阶段构建，构建最终产物镜像会非常小，根据需要选用

参考 [Dockerfile](docker/golang/single/Dockerfile)阶段构建， 产物镜像大小依赖于基础镜像，和本次构建产物大小

2. 提供一些Github CI Action模板

参考 [ci.yaml](.github/workflows/ci.yaml) 进行ci配置， 产物最终推送到 aws的docker公共仓库  iflytek-open 仓库下，

3. 提供Readme.md模板

4. 示例[License](LICENSE)


以上均为模板，复制对应文件到自己项目下进行对应配置修改即可， ci action yaml依赖的 docker仓库秘钥已全局配置到组织下，可直接使用，无需更改。



## 为什么选择 开源项目示例模板

遵循统一的规范标准，有助于整体开源工作的开展


## Quickstart
***示例****
```bash
以下均为demo
kubectl create namespace argo
kubectl apply -n argo -f https://raw.githubusercontent.com/argoproj/argo-workflows/master/manifests/install.yaml
```

## Client Libraries
***示例****
Check out our [Java, Golang and Python clients](docs/client-libraries.md).


## 谁在用?
***示例****
[Official Argo Workflows user list](USERS.md)

## 文档

***示例****
* [Get started here](docs/quick-start.md)
* [How to write Argo Workflow specs](https://github.com/argoproj/argo-workflows/blob/master/examples/README.md)
* [How to configure your artifact repository](docs/configure-artifact-repository.md)

## 特性

* 1
* 2


## 联系我们

* [Iflytek-opensource](https://github.com/iflytek/community)

## 友情链接

* Iflytek GitHub:  [Iflytek-opensource](https://github.com/iflytek)
* Iflytek Website: [https://argoproj.github.io/](https://iflytek.github.io/)
