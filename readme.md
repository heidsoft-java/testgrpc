# learn grpc 
```
1. 下载安装java版本protoc程序
https://github.com/protocolbuffers/protobuf/releases/tag/v3.6.1
2. 编译安装
3. 设置环境变量
export DST_DIR=/Users/heidsoft/research/testgrpc/java
export SRC_DIR=/Users/heidsoft/research/testgrpc/proto
protoc -I=$SRC_DIR --java_out=$DST_DIR $SRC_DIR/test.proto
```

# proto 语法
```
定义生产类名称
option java_outer_classname = "Foo";

定义包名称
package foo.bar;

定义java包，生产包时将忽略域名部分
option java_package = "io.heidsoft.foo.bar";
```

