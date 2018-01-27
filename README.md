# 大作业 - 课程系统改进

### 原项目的github地址[戳这里](https://github.com/PENGZhaoqing/CourseSelect)

### 本项目用cloud9作为IDE,项目部署在Heroku上，项目地址[点这里](https://course-ttt.herokuapp.com)

### 项目改进点
- 添加了课程考试安排的相关信息
- 对管理员后台进行了汉化

## 使用

1.学生登陆：
账号：`student1@test.com`
密码：`password`

2.老师登陆：
账号：`teacher1@test.com`
密码：`password`

3.管理员登陆：
账号：`admin@test.com`
密码：`password`

账号中数字都可以替换成2,3...等等

### 效果截图
管理员可以在后台的课程编辑页面对每个课程的"考试时间"、"考试地点"信息进行添加、修改、删除
<img src="/lib/1.png" width="900">

老师在课程管理页面点击左栏的"考试安排"可以看到自己所授课程的考试安排情况
<img src="/lib/2.jpg" width="900">

学生在我的课程页面点击左栏的"考试安排"可以看到自己所选课程的考试安排情况
<img src="/lib/3.jpg" width="900">   

下面三张图是对管理员后台界面各字段进行汉化的结果
<img src="/lib/4.png" width="900">
<img src="/lib/5.png" width="900">
<img src="/lib/6.png" width="900">


## 项目实现的大致过程

### 添加考试信息
1. 修改模型，在Course模型(文件路径:/db/migrate/20160907152104_create_courses.rb )中添加 考试时间(exam_time) 和 考试地点(exam_room) 两个属性字段
