## Vue 3.0 进展_VueConf CN 2019

- 本文只是针对视频内容的重点整理，如若不清楚的地方或觉得有漏掉的地方请自行看文末链接的现场视频内容。

### 3.0 设计目标
- 更小
- 更快
- 加强 API 设计一致性
- 加强 TypeScript 支持
- 提高自身可维护性
- 开放更多底层功能

### 更小
- 全局 API 和内置组件 / 功能支持 tree-shaking
- 常驻的代码尺寸控制在 10kb gzipped 上下

### 更快
- 基于 Proxy 的变动侦测，性能整体优于 getter / setter
- 长远来看，JS 引擎会继续优化 Proxy，但 getter / setter 基本不会再有针对性的优化
- Virtual DOM 重构
- 更新速度 / 内存占用均有质的提升
- 编译器架构重构，更多的编译时优化

### 提高自身可维护性
- 代码采用 monorepo 结构，内部分层更清晰
- TypeScript 使得外部贡献者更有信心做改动

### 开放更多底层功能
- Custom Renderer

### TypeScript
- 3.0 本身用 TypeScript 重写，内置 typing
- TSX 支持
- 不会影响不使用 TS 的用户

### Class API
- Class API 提案已撤销，注意

### Function-based API
- 更灵活的逻辑复用能力
- 更好的 TypeScript 类型推导支持
- 更好的性能
- Tree-shaking 友好
- 代码更容易被压缩

### 关于逻辑复用
- Mixin（混入的属性来源不清晰；命名空间冲突；）
- 高阶组件HOC（Props 来源不清晰；Props 命名空间冲突；多余的组件实例造成的性能浪费；）
- Scoped Slots（来源清晰；无命名空间冲突；多余的组件实例造成的性能浪费；）
- Composition Functions（就是简单的函数组合；无额外的组件实例开销；）

### 相关资料
- [Vue.js作者尤雨溪谈 Vue 3.0 进展_VueConf CN 2019](https://www.bilibili.com/video/BV1X4411S7gu)
- [http://www.vuecss.com/?thread-334.htm](http://www.vuecss.com/?thread-334.htm)