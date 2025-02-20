---
layout: default
title: "培训要求"
permalink: /android/rules/
---

# 基本规则

整个三天的练习，各小组应该严格遵守以下基本规则：

1. 主干开发+分支发布（Github flow）
   - potetcted master branch
   - 采用 PR 合并代码
2. 持续集成
   - 每天每个成员（如结对，在提交记录中说明了结对的成员）都至少有一次代码提交
   - 构建失败立即响应
   - 每天最后一次构建是成功的，APP 可以下载（第一天除外）
3. 结对编程
4. 测试驱动开发
   - 每次提交都有测试代码
5. 原子提交
   - 没有少提、多提文件
   - 每次提交之前都全量运行测试
   - [七步提交法](https://static001.infoq.cn/resource/image/4c/d1/4c5d2f40c00ffd6d00b1d011108f66d1.png)
6. 及时重构
   - 及时使用 IDE 检查代码
   - 熟练运用 IDE 重构菜单
7. 代码整洁
   - lint 不出错
   - 命名有意义
   - PR 都要交叉 review
8. 架构整洁
   - 采用 MVVM 或 MVP
   - PR 都要交叉 review

我们会根据客观的流水线度量数据对各小组进行评分。我们也会在练习过程中观察各小组的表现，给予一定的“筹码”奖励。额外的加分项包括但不限于：
  - 每日小组站会
  - 每日小组回顾
  - 每日计划会
  - 每日集体代码检视
  - 使用看板跟踪进度
  - 快捷键用得溜
  - 重复代码少
  - 提交记录写得清楚
  - Tasking 做得好
  - 经常与教练交流，话题包括但不限于需求、架构


# 交付要求

用作练习的新闻客户端有[很多需求](https://cac-tech-coach.github.io/NewsClientSpecs/)，每个小组**必须**通过三天练习完成新闻客户端的“MVP”，即[新闻列表](https://cac-tech-coach.github.io/NewsClientSpecs/specs/news-list.html)。

**每天晚上8点**，我们会对每个小组的交付物和代码进行验收。交付物的验收条件如下：

- 第一天，**不要求**实现任何界面，**要求**实现 Model 和 ViewModel/Presenter。
- 第二天，**要求**实现新闻列表界面，交付一个可以运行的 APK。
- 第三天，**要求**实现更多界面，交付一个可以运行的 APK。

在完成基本要求（新闻列表）的情况下，小组可以选择更多的需求进行练习，在遵循基本规则的前提下完成的需求越多，打擂时通过展示获得评委的青睐。

# 鼓励采用 Kotlin

**如果采用 Koltin 完成整个练习，小组客观度量数据得分获得额外 20% 奖励。** 

# 打擂要求

第三天下午以小组为单位进行展示，每个小组有**20分钟**的展示时间。展示的内容包括：

- 练习结果的展示（APP演示以及过程数据展示，如客观得分的度量指标、GitHub 数据展示等等）
- 练习过程的体会（各种技术实践的心得体会，过程中小组的变化、调整以及改进）
- 未来的计划（结合自己的产品，谈谈这些技术实践在未来如何落地。哪些实践适合？哪些实践收效大？哪些实践落地需要调整？如何调整？）



[返回](./index.md)