### 姓名
陆琦

### 实习项目
新 IR API + 自动微分推全和核心组件完善

### 本周工作

1. **维护第三期的 PIR 迁移的任务**
    （xxxx 待更新 xxxx）
    * 发布并第三期的 PIR API 迁移任务, 为开发者提供答疑和 pr review, 推进迁移任务进行：
        https://github.com/PaddlePaddle/Paddle/issues/58067
	
    * review PR, 并解决开发者问题, 总结共性问题至 「PIR 迁移任务的 bug 修复手册」：
        1. ...


2. **推进 API PIR 下的推全验证工作**
    （xxxx 待更新 xxxx）
   * 完成 pr :
        1. atan, atanh: https://github.com/PaddlePaddle/Paddle/pull/58473
        2. asin, asinh: https://github.com/PaddlePaddle/Paddle/pull/58470
        3. FusedMultiHeadAttention, FusedFeedForward: https://github.com/PaddlePaddle/Paddle/pull/58453
        4. acosh: https://github.com/PaddlePaddle/Paddle/pull/58450
        5. acos: https://github.com/PaddlePaddle/Paddle/pull/58317

    * 正在推进 pr :
        1. nn.initializer.Uniform: https://github.com/PaddlePaddle/Paddle/pull/58642
        2. cosh: https://github.com/PaddlePaddle/Paddle/pull/58608
        3. group_norm: https://github.com/PaddlePaddle/Paddle/pull/58608
        4. logsumexp: https://github.com/PaddlePaddle/Paddle/pull/58843
        5. lgamma: https://github.com/PaddlePaddle/Paddle/pull/58840
        6. log1p: https://github.com/PaddlePaddle/Paddle/pull/58840

3. **完善 PIR API 相关机制**
    1. 代码自动生成触发阶段由 make 编译阶段移至 cmake 构建阶段：https://github.com/PaddlePaddle/Paddle/pull/59129
    2. 为 OpResult 添加 id 属性，以支撑 check_numerics 在 pir 模式下运行：https://github.com/PaddlePaddle/Paddle/pull/59064
    3. 在 Executor 运行前，pop 出 program 中不存在的 feed variable ：https://github.com/PaddlePaddle/Paddle/pull/58984

4. **支持动静半架构升级工作**
    1. eager_properties.cc support auto parallel : https://github.com/PaddlePaddle/Paddle/pull/58746
    2. embedding_grad support AutoParallel : https://github.com/PaddlePaddle/Paddle/pull/58928


### **问题疑惑与解答**

    1. paddle/fluid/pir/dialect/operator/ir/ops.yaml 与 paddle/phi/api/yaml/ops.yaml 有什么区别？

### 下周工作

1. 与外部开发者协作沟通，管理任务发布, review PR, 答疑和 bug 修复 issue，推进 API PIR 下的推全验证工作
2. 继续完善 API PIR 下的迁移工作
3. 完成 code reading 笔记

### 导师点评
