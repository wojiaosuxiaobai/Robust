### 修复官方低版本gradle编译问题及Java9编译错误,针对有问题的版本打包了两个插件，只需要调整原来的
### Fixed Android Gradle Plugin Version 4.x compilation errors.
### Fixed Targeting R+ (version 30 and above) installed APKs error.

复制repo文件夹到工程的根目录

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
         repository(url: uri('../repo'))
    }
```
其他所有用法保持不变。
[官方文档](https://github.com/Meituan-Dianping/Robust/blob/master/README-zh.md)
