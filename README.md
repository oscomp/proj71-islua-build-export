# proj71-islua-build-export

为 isula-build 实现 export 接口：将镜像导出为 rootfs

### *描述* 

当前isula-build save出来的镜像都是按照image spec要求的、按镜像层分层的输出件格式。需要添加如下功能：

1. 添加`ctr-img export`接口，支持将镜像保存为一个展开的 rootfs 的 tarball 格式
2. 基于`ctr-img export`接口，添加flag，支持将镜像保存为一个仅包含image spec的empty.tar 和 一个展开的 rootfs
3. 给 `ctr-img import` 接口添加 flag，以支持导入这种镜像形式

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

 @jingxiaolu

*联系方式*  lujingxiao@huawei.com

### 难度

中

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
