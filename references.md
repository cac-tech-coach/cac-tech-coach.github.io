---
layout: default
title: "参考资料"
permalink: /references/
---

# 基础知识

1. 主干开发+分支发布：
   - [https://trunkbaseddevelopment.com/](https://trunkbaseddevelopment.com/)
   - [https://insights.thoughtworks.cn/gitflow-consider-harmful/](https://insights.thoughtworks.cn/gitflow-consider-harmful/)
3. 单元测试术语、模式、坏味道...：[http://xunitpatterns.com/](http://xunitpatterns.com/)、
4. 结对编程：
   - [https://insights.thoughtworks.cn/pair-programming/](https://insights.thoughtworks.cn/pair-programming/)
   - [https://codingstyle.cn/topics/244](https://codingstyle.cn/topics/244)
   - [https://insights.thoughtworks.cn/seven-skills-about-pair-programming/](https://insights.thoughtworks.cn/seven-skills-about-pair-programming/)
5. 测试驱动开发：
   - [http://insights.thoughtworkers.org/talk-about-tdd-again/](http://insights.thoughtworkers.org/talk-about-tdd-again/)
   - [https://insights.thoughtworks.cn/talk-about-tdd-again-2/](https://insights.thoughtworks.cn/talk-about-tdd-again-2/)
   - [https://insights.thoughtworks.cn/when-we-talk-about-bdd/](https://insights.thoughtworks.cn/when-we-talk-about-bdd/)
6. 代码检视：[https://insights.thoughtworks.cn/code-review/](https://insights.thoughtworks.cn/code-review/)
7. 重构：[https://insights.thoughtworks.cn/principles-of-refactoring/](https://insights.thoughtworks.cn/principles-of-refactoring/)
8. 质量内建：[https://insights.thoughtworks.cn/professional/](https://insights.thoughtworks.cn/professional/)
9. 代码覆盖率：[https://insights.thoughtworks.cn/code-coverage-2/](https://insights.thoughtworks.cn/code-coverage-2/)

# Android library 速查

## RxJava

// TODO

## Retrofit

// TODO

## Espresso

Espresso cheatsheet：[https://developer.android.com/training/testing/espresso/cheat-sheet](https://developer.android.com/training/testing/espresso/cheat-sheet)

Espresso Koltin DSL：[https://github.com/AdevintaSpain/Barista](https://github.com/AdevintaSpain/Barista)

```kotlin
clickOn(R.id.button)
clickOn(R.string.button_text)
clickOn("Next")
clickBack()

// list related
clickListItem(R.id.list, 4);
scrollListToPosition(R.id.list, 4);
assertListItemCount(R.id.list, 5)
assertListNotEmpty(R.id.list)
assertDisplayedAtPosition(R.id.list, 0, "text");
assertDisplayedAtPosition(R.id.list, 0, R.id.text_field, "text");
```

## Robolectric

让`androidTest`中的espresso测试可以放到`test`中执行。

app/build.gradle中的配置，参考：[https://medium.com/androiddevelopers/write-once-run-everywhere-tests-on-android-88adb2ba20c5](https://medium.com/androiddevelopers/write-once-run-everywhere-tests-on-android-88adb2ba20c5)
```groovy
android {
    testOptions {
        unitTests.includeAndroidResources = true
    }
}

dependencies {
    testImplementation 'androidx.test:runner:1.2.0'
    testImplementation 'androidx.test.ext:junit:1.1.1'
    testImplementation 'androidx.test.espresso:espresso-intents:3.2.0'
    testImplementation 'androidx.test.espresso:espresso-core:3.2.0'
    testImplementation 'androidx.test.ext:truth:1.2.0'
    testImplementation 'org.robolectric:robolectric:4.3'
}
```

不支持 API level 29 的解决方法，参考：[http://robolectric.org/configuring/](http://robolectric.org/configuring/)
```properties
# src/test/resources/com/mycompany/app/robolectric.properties
sdk=28
```


[返回](./index.md)