# 通用mapper的逆向生成工程

## 实现的功能

- 主要通过mybatis-generator-maven-plugin插件生成了通用mapper的实体类和mapper接口,
同时也整合了lombok进去

## 用法

- 在`generator-config.properties`里面配置一些必须的配置
- 在`generator-config.properties`里面`plugins.CommentPlugin`和`plugins.LombokPlugin`这个填入的是自定义的插件
的路径, 可以参考https://www.jianshu.com/p/7f57be69bb94,这里面有详细的介绍,https://github.com/GuoGuiRong/mybatis-generator-lombok-plugin
这个是自定义插件的git地址
- 以上如果都配置好的话, 可以点开`maven`, 找到`mybatis-generator:generate`,然后点击就可以生层对应的实体类和mapper

## 参考文档

- mybatis-generator.xml配置文件详解 https://blog.csdn.net/weixin_39805338/article/details/80999186
- mybatis 通用mapper，generator代码生成器,generator 生成 lombok https://blog.csdn.net/lwang_IT/article/details/89021755