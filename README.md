# SXU-ComputerNetwork exam





## 基本配置

服务器实体在系楼四楼网络工程实验室，核心6 机柜的 S6 下面一个。

> 服务器启动非常慢，慢慢等服务启动

技术栈用的是 php thinkphp 开发

用的是 JVM 虚拟化即实机的 ip 为 115.24.12.233 （密码忘了），JVM 虚拟机跑的是系统，ip 是 115.24.12.240 用户名是 unbunt 密码是 lzx23333333

项目代码位于 240 的 /var/www/network

系统教师端的 URL 是 115.24.12.240/teacher/home/student.html ，用户名是 admin 密码是 admin



## 可能需要做的/注意

### 帮老师导入学生信息

这个系统是按照之前的教务管理系统写的，所以需要帮忙生成一份以下格式的 csv 学生列表文件（注意一定要 **utf8** 编码）

1. 可以直接先用之前的列表导出一份 csv 文件，按照那个格式即可
2. 需要修改的就名字和学号，密码自动生成

### 删除班级不删除数据库

系统存在一点问题，删除班级时候，内部的学生信息仍然在数据库中。也就是说如果反复建相同学生，就造成这个学生有多个账号，而且是相同学号的多个账号

如果出现这种情况：

进入数据库 mysql  `sudo mysql` ，然后将 student 表中重复数据删除即可





## 其他



115.24.12.240/666 可以进入可视化界面





## 关于

系统是由 2016 级计科李政兴开发

文档由 2019 级计科陈舜泽记录







