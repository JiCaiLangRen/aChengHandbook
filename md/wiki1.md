# **IDEA 如何在一个project中运行多个项目**



>
>   ### 注意事项：旧版本IDEA（IntelliJ IDEA 2020.2.2 版本）对多项目GIT操作不友好 建议配合其他git管理工具使用、
> 
> 较新版本已经解决多项目GIT不方便处理的问题了  
> 
> 当前不建议使用2023.1.5以后的版本 因为1.5以后的版本不支持公司自己开发的插件
> 
> 本文档中使用的是 IntelliJ IDEA 2023.1.5 版本进行截图 与



## 1. 创建一个空白项目

省略



## 2. 打开项目结构设置
点击导入模块找到对应的项目点击导入

![img.png](../img/项目结构_导入模块.png)

选择从现有项目创建模块

![从现有项目创建模块.png](..%2Fimg%2F%E4%BB%8E%E7%8E%B0%E6%9C%89%E9%A1%B9%E7%9B%AE%E5%88%9B%E5%BB%BA%E6%A8%A1%E5%9D%97.png)

选择代码源文件，不要选已经编译好的文件

![选择代码源文件.png](..%2Fimg%2F%E9%80%89%E6%8B%A9%E4%BB%A3%E7%A0%81%E6%BA%90%E6%96%87%E4%BB%B6.png)

选择对应的库配置 （lib） 请注意 out/artfacts 是idea编译后的输出位置，不要选这个

![选择库配置.png](..%2Fimg%2F%E9%80%89%E6%8B%A9%E5%BA%93%E9%85%8D%E7%BD%AE.png)

确认选择的配置，无误后点击下一步

![导入模块名称配置.png](..%2Fimg%2F%E5%AF%BC%E5%85%A5%E6%A8%A1%E5%9D%97%E5%90%8D%E7%A7%B0%E9%85%8D%E7%BD%AE.png)

out/artfacts 是idea编译后的输出位置，不要选这个

![选择WEB_INF.png](..%2Fimg%2F%E9%80%89%E6%8B%A9WEB_INF.png)

## 3. 调整配置

处理多余的web配置 （多余的配置是idea自动添加的）

![处理多余的WEB配置.png](..%2Fimg%2F%E5%A4%84%E7%90%86%E5%A4%9A%E4%BD%99%E7%9A%84WEB%E9%85%8D%E7%BD%AE.png)

配置对应的工件（翻译过来是这个） tomcat中配置的也是这个

![创建对应的工件.png](..%2Fimg%2F%E5%88%9B%E5%BB%BA%E5%AF%B9%E5%BA%94%E7%9A%84%E5%B7%A5%E4%BB%B6.png)

处理工件依赖

![处理工件依赖.png](..%2Fimg%2F%E5%A4%84%E7%90%86%E5%B7%A5%E4%BB%B6%E4%BE%9D%E8%B5%96.png)

在tomcat中进行配置就可以运行了

![配置tomcat运行项目.png](..%2Fimg%2F%E9%85%8D%E7%BD%AEtomcat%E8%BF%90%E8%A1%8C%E9%A1%B9%E7%9B%AE.png)

然后就可以运行了

## 4.git 代码提交

旧版本可以使用 Sourcetree 进行提交 （公司内部比较推荐的git可视化管理工具）

idea 中的操作

![img.png](../img/ideaGit管理.png)