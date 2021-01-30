# proj71-export-islua-build

为 isula-build 实现 export 接口：将镜像导出为 rootfs

### *描述* 

当前isula-build save出来的镜像都是按照image spec要求的、按镜像层分层的输出件格式。需要添加如下功能：

1. 添加`ctr-img export`接口，支持将镜像保存为一个展开的 rootfs 的 tarball 格式
2. 基于`ctr-img export`接口，添加flag，支持将镜像保存为一个仅包含image spec的empty.tar 和 一个展开的 rootfs
3. 给 `ctr-img import` 接口添加 flag，以支持导入这种镜像形式

### *难度* 

中

### *导师* 

 @jingxiaolu

*联系方式*  lujingxiao@huawei.com

### License

- MulanPSL v2

### *项目产出标准*

- 编写 isula-build 的源码、单元测试以及tests
- 更新 isula-build 相关使用文档
- 源码提交至 isula-build 源码仓

### *技术要求*

1. go语言开发

### *相关项目*

1. https://gitee.com/openeuler/isula-build
