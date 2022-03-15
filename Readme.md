# java 数据库操作-学习笔记
2022-03-10
## 动机
2022-03-10，在现场做项目，决定将 21-推送报表数据至数据平台 代码从 web 模块拆分出来，
做成单独的 spring boot 项目。其中涉及到简单的数据库增删改查，我有种茫然无措之感，可见
基础知识薄弱，加油补充。

## 大纲
- 理论与实践结合
- 准备数据库
- 聚焦目标
  - 编写后台接口测试代码逻辑的正确性；
  - 不写前台页面，等到学习前端的时候可以用这个后台服务
  - 针对功能性代码必须写单元测试，
  - 不搞复杂的单元测试，比如mook对象，这一块知识也要单独学习
- 我其实有一定基础，其实各个知识点都已经接触过，所以学习路线和完全的初学者必然不同。
  这次学习更多是夯实基础，积累实战经验。我基础实在太差，必须努力。

### 理论
- jdbc
- mybatis
- spring boot + mybatis
- spring boot + jdbcTemplate

少量示例，重点在库的体系结构和使用规范上。

### 实战
列举常见任务，尽可能的全面

- 单表的增删改查
- 事务提交、回滚
- DDL 语句
- 不同数据类型以及对应留心的方面
  - 字符串：溢出和编码问题
  - 整数：溢出问题
  - 浮点数：溢出问题，精度问题
  - 定点数：溢出，精度
  - 日期、时间：日期、时间、时间戳的区分，时区问题，秒还是毫秒的精度问题
  - 大字段：文本、二进制

- 客户端连接服务器时的国际化和本地化
  - 时区：影响日期时间字段的插入、查询结果
  - 字符编码：影响字符串（尤其是汉字）的插入、查询结果
  - locale：Q. 会影响什么呢？
场景：学生信息管理系统。


### 知识补充
- 数据库事务

### 环境
- jdk 17：稀罕它的 var 变量
- 最新版 MyBatis
- 最新版 Spring Boot
- MySQL 8.0

## 相关链接
[java jdbc 样例代码](https://github.com/chenxizhan1995/java-demo-db-jdbc)
