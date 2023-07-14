## this is structure for board.json

```
board.json
├── name: 板子的名称，用于显示
├── url: 板子的网址，用于提供更多信息
├── vendor: 板子的厂商，用于标识来源
├── upload: 板子的上传设置，用于指定上传协议、速率、端口等
│   ├── protocol: 上传协议，必须是已经支持的协议之一
│   ├── speed: 上传速率，单位是波特率
│   ├── port: 上传端口，可以是自动检测或指定值
│   └── maximum_size: 最大上传大小，单位是字节
├── frameworks: 板子支持的框架，用于编程
│   ├── %FRAMEWORK_NAME_1%: 框架的名称，必须是已经支持的框架之一或多个
│   └── %FRAMEWORK_NAME_N%: 框架的名称，必须是已经支持的框架之一或多个
└── build: 板子的构建设置，用于指定核心、变体、mcu、f_cpu等
    ├── core: 核心类型，必须是已经支持的核心之一
    ├── variant: 变体类型，必须是已经支持的变体之一
    ├── mcu: MCU型号，必须是已经支持的型号之一
    ├── f_cpu: CPU频率，单位是赫兹
    ├── extra_flags: 额外的编译标志，可以根据需要添加


```
