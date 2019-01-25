# MongoDBSink

#### 介绍
实现​Java写日志到Flume，Flume最终把日志写到MongoDB

#### 更新说明
1.依赖更新至官方
2.加入后续更多案例

#### 安装教程

1. 前往Flume官方地址下载Flume1.9.0
2. 前往MongoDB下载4.0以上版本MongoDB（其他版本没有测试）
3. 线上使用需在flume/lib下添加一下几个jar包
- mongodb-driver-3.9.1.jar
- mongodb-driver-core-3.9.1.jar
- bson-3.9.1.jar

#### 使用说明

1. 下载本项目后打JAR包放入flume/lib下
2. 在Flume的conf目录配置MongoDBFlume.conf （仓库有案例配置文件）
3. 运行：bin/flume-ng agent --conf conf --conf-file conf/MongoDBFlume.conf --name a1 -Dflume.root.logger=info,console
4. 本地测试：telnet localhost 44444
5. 在telnet插入JSON数据测试

#### 使用注意
- 如果没有密码和用户名 就不需要user password authentication_enabled这3个参数
- 如果有密码，请设置authentication_enabled = True

#### 参与贡献

1. Fork 本仓库
2. 新建分支
3. 提交代码
4. 新建 Pull Request

#### 联系作者
1. 红警专家 [blog.gzczy.top](https://blog.gzczy.top)
2. 关注微信公众号：JAVA大咖说

![Image discription](http://image.gzczy.top/2018/12/qrcode_for_gh_c464884a70ff_258.jpg)

