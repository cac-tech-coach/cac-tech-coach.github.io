
# 目标

建立对敏捷的基本认知。通过 8 小时左右的示例项目实操演练，掌握持续交付与质量内建所包括的关键技术实践，学会如何引导团队在 Android 新应用、新代码中逐步实现持续交付和质量内建。

# 小组划分

参训学员组成[**6个学习小组**](teams.md)，以小组为单位，在三天的培训时间里，根据讲师所讲收的内容和布置的任务，采用正确的技术实践完成示例项目的持续演练。在培训的最后一天下午，以小组为单位展示三天所学内容在示例项目中的运用，进行PK。最终根据小组互动表现、度量数据、以及打擂展示的[**综合得分**](scoring-rules.md)确定[**最终排名**](https://coda.io/d/CAC-OPPO_dWBwjkLuEXF/_subOs)。

| 小组        | 仓库                                       | 成员                                                       | 构建                                                                                                                              | 覆盖率                                                                                                                                   | 应用下载地址               |
| ----------- | ------------------------------------------ | ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| Oreo        | https://github.com/CAC-0pp0/CACOreo        | https://github.com/orgs/CAC-0pp0/teams/oreo/members        | [![Build Status](https://travis-ci.org/CAC-0pp0/CACOreo.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACOreo)               | [![codecov](https://codecov.io/gh/CAC-0pp0/CACOreo/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACOreo)               | https://www.pgyer.com/GD4q |
| Nougat      | https://github.com/CAC-0pp0/CACNougat      | https://github.com/orgs/CAC-0pp0/teams/nougat/members      | [![Build Status](https://travis-ci.org/CAC-0pp0/CACNougat.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACNougat)           | [![codecov](https://codecov.io/gh/CAC-0pp0/CACNougat/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACNougat)           | https://www.pgyer.com/9ykK |
| Marshmallow | https://github.com/CAC-0pp0/CACMarshmallow | https://github.com/orgs/CAC-0pp0/teams/marshmallow/members | [![Build Status](https://travis-ci.org/CAC-0pp0/CACMarshmallow.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACMarshmallow) | [![codecov](https://codecov.io/gh/CAC-0pp0/CACMarshmallow/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACMarshmallow) | https://www.pgyer.com/qbSY |
| Lollipop    | https://github.com/CAC-0pp0/CACLollipop    | https://github.com/orgs/CAC-0pp0/teams/lollipop/members    | [![Build Status](https://travis-ci.org/CAC-0pp0/CACLollipop.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACLollipop)       | [![codecov](https://codecov.io/gh/CAC-0pp0/CACLollipop/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACLollipop)       | https://www.pgyer.com/955w |
| KitKat      | https://github.com/CAC-0pp0/CACKitKat      | https://github.com/orgs/CAC-0pp0/teams/kitkat/members      | [![Build Status](https://travis-ci.org/CAC-0pp0/CACKitKat.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACKitKat)           | [![codecov](https://codecov.io/gh/CAC-0pp0/CACKitKat/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACKitKat)           | https://www.pgyer.com/UFQH |
| Jelly Bean  | https://github.com/CAC-0pp0/CACJellyBean   | https://github.com/orgs/CAC-0pp0/teams/jelly-bean/members  | [![Build Status](https://travis-ci.org/CAC-0pp0/CACJellyBean.svg?branch=master)](https://travis-ci.org/CAC-0pp0/CACJellyBean)     | [![codecov](https://codecov.io/gh/CAC-0pp0/CACJellyBean/branch/master/graph/badge.svg)](https://codecov.io/gh/CAC-0pp0/CACJellyBean)     | https://www.pgyer.com/2SL2 |

# 充分准备

## 开发环境

本次培训有8小时左右的 Android 编码演练，学员需要提前准备好Android开发环境。要求如下：

1. 安装 JDK 8
2. 安装最新 Android SDK（API Level 29）
3. 安装最新 Android Studio（3.5）
4. 安装 Git 客户端
5. 安装 Gradle 或使用 Gradle Wrapper

各小组的代码仓库都已经建立好（见上表），学员们在培训前可以拉取模板工程代码，提前编译缓存好相关依赖，提高练习时的编译效率。

## 熟悉练习

本次练习要完成的是一个 Android 新闻客户端。

1. 熟悉新闻客户端的**[用户故事](https://cac-tech-coach.github.io/NewsClientSpecs)**。
2. 熟悉新闻客户端要使用的**[服务 API](https://cac-tech-coach.github.io/NewsClientAPI/)**。

## 知识准备（建议）

1. 学习 Android Components，了解最新的 Android 分层架构风格，请参考：https://codelabs.developers.google.com/codelabs/android-room-with-a-view 或 https://codelabs.developers.google.com/codelabs/android-room-with-a-view-kotlin/
2. 学习 Android 测试知识，了解可以使用的 Android 测试库，请参考：https://codelabs.developers.google.com/codelabs/android-testing。
3. 学习 Kotlin（本次培训演示将全部使用 Koltin，[**使用 Kotlin 完成练习也能获得额外加分**](scoring-rules.md)），请参考：https://kotlinlang.org/docs/reference/ 和 https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012




