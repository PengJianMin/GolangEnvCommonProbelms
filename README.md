# GolangEnvCommonProbelms
+ A：Goland创建项目后没法Run起来？
  + 可以在右上角的“edit configurations...”里把Working directory选择成项目路径
  + 如果依然不行，对项目进行**模块化**，即使用`go mod`命令工具链。
+ A：go get 到本地的包，Goland没有识别，导致在编码的时候没有弹出**包内变量和方法提示**，编码很难受
  + 在File --> Settings --> Go Modules(vgo) 页面中，把 "Enable Go Modules(vgo) integration" 勾选上[https://blog.csdn.net/itopit/article/details/120271264](https://blog.csdn.net/itopit/article/details/120271264)
+ A：第三方的模块和包**下载很慢**或者**无法下载**
  + 需要翻墙，一般通过配置代理解决
  + `export GOPROXY="https://goproxy.cn,direct"`
  + Windows 配置同样的环境变量即可
