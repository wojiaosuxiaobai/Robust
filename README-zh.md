###Fixed official low version gradle compilation problems and Java9 compilation errors. Two plug-ins are packaged for the problematic version. You only need to adjust the original
###Fixed Android Gradle Plugin Version 4.x compilation errors.
###Fixed Targeting R+ (version 30 and above) installed APKs error.

Copy repo dir to your project root path

```
classpath'com.meituan.robust:gradle-plugin:0.4.99'
classpath'com.meituan.robust:auto-patch-plugin:0.4.99'
```

Change to

```
classpath'com.effective.android:gradle-plugin-fix:0.4.99.5'
classpath'com.effective.android:auto-patch-plugin-fix:0.4.99.5'
```

Add repositories

```
    repositories {
        //...
        repository(url: uri('../repo'))
    }
```

All other usages remain unchanged.

[Official document](https://github.com/Meituan-Dianping/Robust/blob/master/README-zh.md)

