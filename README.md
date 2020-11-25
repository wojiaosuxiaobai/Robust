### 修复官方低版本gradle编译问题及Java9编译错误,针对有问题的版本打包了两个插件，只需要调整原来的
```
classpath 'com.meituan.robust:gradle-plugin:0.4.99'
classpath 'com.meituan.robust:auto-patch-plugin:0.4.99'
```

改成

```
classpath 'com.effective.android:gradle-plugin-fix:0.4.99.1'
classpath 'com.effective.android:auto-patch-plugin-fix:0.4.99.1'
```

添加仓库

```
    repositories {
        //...
        maven { url 'https://dl.bintray.com/yummylau/maven' }
    }
```
其他所有用法保持不变。
[官方文档](https://github.com/Meituan-Dianping/Robust/blob/master/README-zh.md)
