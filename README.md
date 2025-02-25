# BlogCommentSystemAPI
This is a simple and breif system of BlogComment on API

这是一个简单，简洁的博客评论系统 API
技术栈：go 1.22, mysql, redis, docker ,gin 框架,

重要文件描述
1、API_Document：API设计文档
2、create_test.go,get_test.go,delete_test.go,reply_test.go是4个单元测试文件，用于分别测试评论的四个功能（创建评论，获取评论，删除评论，评论回复）

声明：
  - 实现评论的 Markdown 支持。
  - 实现评论的通知功能（如邮件通知）。
  - 使用 Redis 缓存评论数据。

需要改善的点：
1、EMail包 需要更好的设计，以实现解耦
2、在高并发情况下，评论功能需要增加数据库连接池，来提高性能
