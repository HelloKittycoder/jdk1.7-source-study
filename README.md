# jdk1.7-source-study
jdk1.7源码学习（jdk版本 jdk1.7.0_79）

### 搭建源码阅读环境
1. 解压src.zip放到新建好的项目jdk1.7-source-study的src目录下  
2. 关联jdk目录下的lib包（不然会提示com.sun.tools下的一堆类都找不到），在Project Structure->Libraries中添加  
3. 手动添加UNIXToolkit和FontConfigManager这两个类（https://blog.csdn.net/m4330187/article/details/116407136 直接到openjdk官网找即可）  
我下载的是 https://hg.openjdk.org/jdk7u/jdk7u60/jdk/ 的openjdk  
4. 编译时可能会报内存不足（idea里File->Settings->Compiler->Build process heap size调大一点，我的改成1000就行了）  
5. 在代码调试时能自动关联上源码（在Project Structure->SDKs中，把1.7复制一份1.7study，在Sourcepath中把src.zip换成当前目录下的src）  
说明：如果Main.java运行没问题，说明环境搭建OK了  
参考链接：https://blog.csdn.net/u010999809/article/details/101922489