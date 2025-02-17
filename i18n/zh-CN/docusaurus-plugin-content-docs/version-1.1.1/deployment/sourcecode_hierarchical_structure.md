---
title: 源码目录结构
sidebar_position: 5
---

# Linkis源码目录结构

> Linkis代码层级目录结构说明，如果您想详细了解Linkis各个模块，请查看[Linkis的相关架构设计](architecture/overview.md)


```html

├── assembly-combined-package  //编译整个项目的模块
│   ├── assembly-combined
│   ├── bin
│   ├── deploy-config
│   └── src
├── linkis-commons  //核心抽象,里面放所有的公用模块
│   ├── linkis-common  //通用模块,内置很多通用工具
│   ├── linkis-hadoop-common
│   ├── linkis-httpclient  //Java SDK顶层接口
│   ├── linkis-module
│   ├── linkis-mybatis  //SpringCloud的Mybatis模块
│   ├── linkis-protocol
│   ├── linkis-rpc  //RPC模块，基于Feign实现的复杂双向通信
│   ├── linkis-scheduler  //通用调度模块
│   ├── linkis-storage
├── linkis-computation-governance  //计算治理服务
│   ├── linkis-client  //Java SDK，用户通过Client可直接访问Linkis
│   ├── linkis-computation-governance-common
│   ├── linkis-engineconn
│   ├── linkis-engineconn-manager
│   ├── linkis-entrance  //通用底层entrance模块
│   ├── linkis-jdbc-driver
│   ├── linkis-manager
├── linkis-engineconn-plugins
│   ├── engineconn-plugins
│   ├── linkis-engineconn-plugin-framework
├── linkis-extensions
│   ├── linkis-io-file-client
├── linkis-orchestrator
│   ├── linkis-code-orchestrator
│   ├── linkis-computation-orchestrator
│   ├── linkis-orchestrator-core
│   ├── plugin
├── linkis-public-enhancements  //公共增强服务
│   ├── linkis-bml           //物料库
│   ├── linkis-context-service  //统一上下文
│   ├── linkis-datasource  //数据源服务
│   ├── linkis-publicservice  //公共服务
├── linkis-spring-cloud-services
│   ├── linkis-service-discovery
│   ├── linkis-service-gateway  //网关Gateway
├── db  //数据库信息
│   ├── linkis_ddl.sql
│   ├── linkis_dml.sql
│   ├── module
│   └── upgrade
├── tool  //工具脚本
│   ├── dependencies
│   └── modify_license.sh
└── web  //linkis的管理台代码
├── scalastyle-config.xml  //Scala 代码格式检查配置文件
├── CONTRIBUTING_CN.md
├── CONTRIBUTING.md
├── DISCLAIMER
├── LICENSE  //项目源码的LICENSE
├── LICENSE-binary  //二进制包的LICENSE
├── LICENSE-binary-ui  //前端web编译包的LICENSE
├── licenses-binary  //二进制包的详细依赖的license文件
├── licenses-binary-ui  //前端web编译包详细依赖的license文件
├── NOTICE  //项目源码的NOTICE
├── NOTICE-binary  //二进制包的NOTICE
├── NOTICE-binary-ui  //前端web二进制包的NOTICE
├── README.md
├── README_CN.md

```