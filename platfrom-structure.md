# structure for platform.json
```
├── name: 开发板的名称，必须是唯一的
├── title: 开发板的标题，用于显示
├── description: 开发板的描述，用于介绍
├── homepage: 开发板的主页，用于提供更多信息
├── license: 开发板的许可证，用于声明版权
├── keywords: 开发板的关键词，用于搜索
├── repository: 开发板的仓库，用于存放源码
│   ├── type: 仓库的类型，比如git或svn
│   └── url: 仓库的地址，用于访问
├── version: 开发板的版本，用于标识更新
├── frameworks: 开发板支持的框架，用于编程
│   ├── %FRAMEWORK_NAME_1%: 框架的名称，必须是已经支持的框架之一或多个
│   │   ├── package: 框架对应的package名称，必须是已经存在的package之一
│   │   └── script: 框架对应的构建脚本文件，必须是已经存在的文件之一
│   └── %FRAMEWORK_NAME_N%: 框架的名称，必须是已经支持的框架之一或多个
│       ├── package: 框架对应的package名称，必须是已经存在的package之一
│       └── script: 框架对应的构建脚本文件，必须是已经存在的文件之一
└── packages: 开发板依赖的packages，用于提供工具或框架
    ├── toolchain-gccarmnoneeabi: package的名称，必须是唯一的
    │   ├── type: package的类型，比如toolchain或framework
    │   ├── owner: package的所有者，比如platformio或自定义
    │   └── version: package的版本，可以指定范围或精确值
    ├── framework-%FRAMEWORK_NAME_1%: package的名称，必须是唯一的
    │   ├── type: package的类型，比如toolchain或framework
    │   ├── optional: package是否是可选的，默认为false
    │   └── version: package的版本，可以指定范围或精确值
    ├── framework-%FRAMEWORK_NAME_N%: package的名称，必须是唯一的
    │   ├── type: package的类型，比如toolchain或framework
    │   ├── optional: package是否是可选的，默认为false
    │   └── version: package的版本，可以指定范围或精确值
    └── tool-direct-vcs-url: package的名称，必须是唯一的
        ├── type: package的类型，比如toolchain或framework
        ├── optional: package是否是可选的，默认为false
        └── version: package直接使用版本控制系统（VCS）地址作为版本号
```

