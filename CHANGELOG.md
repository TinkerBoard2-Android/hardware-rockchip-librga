# 更新日志

## 1.2.0 (2021-04-26)

### 新增

* im2d api支持ROP。
* sample目录下增加示例图片。
* 支持Gralloc4.0。
* rgaImDemo的循环选项和打印预期选项。
* color key功能。
* color fill支持YUV格式。
* 对RGA1的校验。
* 多种方式查询librga版本号。
* CHANGLOG.md。

### 变更

* 部分定义的索引值。
* 更新im2d api说明文档。
* 使用Apache-2.0 license。
* imresize()使用系数进行缩放时使用向下对齐。
* 取消全局初始化。
* librga版本号的管理。

### 优化

* 整合不同版本Android平台源码。
* 兼容Android、Linux平台。
* C_API的易用性。
* librga图像格式与Android平台图像格式兼容。
* imStrError()内存使用上的风险。
* 兼容两种同步/异步的配置方法。
* rgaSlt demo中支持配置虚拟地址和fd。
* rgaSlt demo返回报错值。
* 获取硬件支持信息的逻辑。
* imcheck()校验功能的可扩展性。
* rotate功能与mirror功能可以同时配置。
* nn_quantize功能与Alpha混合功能可以同时配置。

### 修复

* 修复一些已知错误。
* 在一些旧版本的Android的编译问题。
* C_API向下兼容问题。
* YUV对齐width stride只支持4对齐问题。
* A+B->C模式color space异常的问题。

### 移除

* 一些无效的定义。
* 对libhardware的依赖。
* makefile编译。
* librga初始化的打印。

* C_API对RGA模块的初始化。



###

### 1.1.1 (2020-10-16)

## 1.1.1 (2020-11-12)

### 新增

* color palette功能。
* 支持A+B->C模式进行Alpha混合。
* src、dst、dst over Alpha混合模式。
* 输入格式YUYV422，输出格式YUYV422/420支。
* 输出格式Y400、Y4、Y1。
* wrapbuffer_handle api。
* meson支持编译im2d demo。

### 变更

* license变更。

### 优化

* librga版本管理机制。
* Android NDK编译。

### 修复

* 虚拟地址调用RGA结果输出黑线的问题（cache）。

* 修复一些已知错误。

## 1.0.3 (2020-09-18)

### 新增

* 在原本librga的代码基础上封装im2d api。
* 增加meson、cmake的编译支持。

### 变更

* 修改C_API的实现逻辑。

### 优化

* 整合源代码，使Linux和Android共用同一套源码。

## 1.0.0 （2020-06-03）

### 新增

* 移植librga到Android Q。
