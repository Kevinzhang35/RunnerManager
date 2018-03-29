<h2>简介</h2>

这个项目是一个简单的比赛管理系统，该练手小项目希望能帮助到大家，熟悉SSM的整合开发

<h2>使用技术</h2>

IOC容器：Spring

Web框架：SpringMVC

ORM框架：Mybatis

数据源：C3P0

日志：log4j

前端框架：Hui


<h2>快速上手</h2>

<h4>1.运行环境和所需工具</h4>

编译器：Eclipse
项目构建工具：Maven
数据库：Mysql
JDK版本：jdk1.8
Tomcat版本：Tomcat8.x

2.初始化项目
在你的Mysql中，创建一个数据库名称为 pingpongmanager 的数据库，并导入我提供的 .sql 文件。<br/>
进入src/main/resources修改beans.xml配置文件,把数据库登录名和密码，改为你本地的<br/>
使用 Eclipse 导入项目，选择Maven项目选项，一路点击next就行，导入项目后，如果src目录等，都没显示出来，别急先使用Maven构建该项目<br/>
在 Eclipse 中，配置我们的 Tomcat， 然后把使用Maven构建好的项目添加到Tomcat中<br/>
Maven install 顺序 : 
com-xyf-parent → com-xyf-pojo → com-xyf-common →
com-xyf-mapper → com-xyf-service → com-xyf-front
运行com-xyf-front

登录账户
超级管理员账户：admin 密码为：123123<br/>
管理账户：admin3  密码为：123123<br/>
运动员账户：1550000  密码为：123456<br/>


<h2>功能模块介绍</h2>

<h4>1.登录模块功能</h4>

实现登录验证和登录信息的储存，根据不同的登录账户，对不同页面url进行角色设置
 <img src="/other/login.jpg" alt="主页" style="max-width:100%;">

<h4>2.裁判模块功能</h4>
 <img src="/other/admin3.jpg" alt="主页" style="max-width:100%;">

裁判，裁判长可对、运动员信息、比赛信息 进行 增删改查 操作，管理员账户，可以重置非裁判账户的密码
比赛管理：增加删除修改比赛,添加运动员到比赛中，对比赛中的学生进行评分
 <img src="/other/score.jpg" alt="主页" style="max-width:100%;">

运动员管理：添加运动员信息时，其信息也会添加到登录表中，可以对学生进行评价
 <img src="/other/runner.jpg" alt="主页" style="max-width:100%;">

账户密码重置：
修改密码： 

<h4>3.裁判长模块</h4>
 <img src="/other/project.jpg" alt="主页" style="max-width:100%;">

拥有最高权限
可以添加裁判信息
拥有上述所有功能。

<h4>4.运动员模块</h4>
 <img src="/other/look.jpg" alt="主页" style="max-width:100%;">

运动员可以查看所在的比赛项目
运动员可以查看比赛的评分

<h4>4.其他模块</h4>

密码修改
<img src="/other/password.jpg" alt="主页" style="max-width:100%;">
