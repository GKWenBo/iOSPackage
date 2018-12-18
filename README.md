# iOSPackage
iOS打包方式整理，自带工具打包，Jenkins，脚本，fastlane。

# 前言
> 从事iOS开发也有一段时间了，实习的时候自己就了解了iOS打包分发的一些方式，自己也写了一篇博客[iOS打测试包与分发测试](https://www.jianshu.com/p/fc6721cf5c7f),介绍了如何打测试包以及上传相关的分发平台，也提到了脚本自动打包。现在自己负责几个项目的维护与开发工作，发现打一个包出来到上传到iTunes Connect上实在是太慢了，步骤也多，比较的耗时间，也不够自动化。后面自己了解了Jenkins持续构建工具，和fastlane自动打包工具，下面开始介绍如何使用这些工具吧。

# fastlane
## 相关地址
- GitHub地址：[fastlane](https://github.com/fastlane/fastlane)
- 官方地址：[fastlane.tools](https://fastlane.tools/)
- 文档地址：[官方文档](https://docs.fastlane.tools/)

### 安装fastlane
- 安装command line tools
```
xcode-select --install
```

- Install fastlane
```
brew cask install fastlane
```

- 切换到工程目录，初始化fastlane
```
cd [工程目录]

fastlane init
```
