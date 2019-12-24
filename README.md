# go-grpc-demo


用于测试goland的grpc的开发  
参考官方链接：https://www.grpc.io/docs/quickstart  
本项目使用go mod管理包  

需安装protoc，而后运行命令：
protoc -I src/proto src/proto/greeter.proto --go_out=plugins=grpc:src/greeter_client  
解释：  
--go_out 参数为输出的pb文件位置；  
-I 参数表示输入文件位置，第一个路径src/proto，当proto文件引用其他的proto文件时生效；
第二个路径src/proto/greeter.proto表示proto文件位置；



然后将生成的代码复制到项目src相应位置下即可。  