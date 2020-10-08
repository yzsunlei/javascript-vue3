## Vue.js作者谈：Vue 3 最新进展_VueConf 2018

- 本文只是针对视频内容的重点整理，如若不清楚的地方请看文末链接的现场视频内容。

### Vue3.0会带来些什么：
- 更快
- 更小
- 更易于维护
- 更好的多端渲染支持
- 其他新功能

### 更快：
- 重构虚拟DOM：更多虚拟时的优化；优化slots生成；内联事件函数提取；
- 基于Proxy的新数据监听系统：全语言特性支持+更好的性能；使用时才会去做监听；利用Proxy减少减少组件实例初始化开销；
- 达到效果：速度加倍；内存占用减半；

### 更小：
- 便于Tree-Shaking的代码结构：内置组件；指令的运行时；各种工具函数；
- 效果：代码大小可以减半，约10kb

### 更易于维护：
- 用TypeScript完全重写
- 内部模块解耦
- 编译器重构（插件化设计）
- 带位置信息的parser（source maps）为更好的IDE工具链铺路

### 更好的多端渲染支持
- Custom Renderer API
- runtime-core

### 其他新功能
- 响应式数据监听API（observable、effect）
- 更轻松排查组件更新的触发原因（render Triggered）
- 更好的TypeScript支持包括原生Class API 和 TSX更好的警告信息
- Experimental Hooks Api
- Experimental Slicing Support
- 关于IE会有一个专门的版本，自动降级，IE11还会有很多年

### 相关资料
- [Vue.js作者谈：Vue 3 最新进展[VueConf 2018 杭州 ]](https://www.bilibili.com/video/av36787459/)