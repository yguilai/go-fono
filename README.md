# go-fono

idea: 根据`.fn`文件直接生成接口调用的代码, 灵感来自[feign](https://github.com/OpenFeign/feign), 但feign太java

暂时只实现http接口调用生成, rpc接口客户端代码大部分都能直接生成, 暂不考虑实现

- [ ] 设计`.fn`文件协议
  - [ ] 协议多版本如何实现
- [ ] fono库本身
  - [ ] http client interface设计, 支持多种客户端
  - [ ] mertrics接入
  - [ ] 日志
  - [ ] 耗时统计
  - [ ] encoder/decoder (不同库支持)
    - [ ] 协议只支持json, protoc(待商榷)
  - [ ] 客户端熔断策略
  - [ ] mock
- [ ] 代码生成工具, 参考go-zero/goctl
  - [ ] `.fn`->`.go`代码生成
  - [ ] 考虑兼容feign, 实现`.fn`->`.java`
  - [ ] `.http`->`.fn`转换
- [ ] `.fn`文件ide(vscode, jetbrain系列)代码提示, 语法检测idea

