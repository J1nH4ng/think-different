# lock dot env files

## 来源

在部署软件时，源码是存放在`git`仓库中的，有没有一个组件，可以读取`.env`中的配置信息，例如数据库的配置信息，而不是写在源代码的分支内，同时使用密码保护，生成一个`.env.lock`文件。

每次部署时，使用密码传输进源代码中，而不是明文写入，有效防止被攻击盗取源码后得到数据库等关键信息。同时，防止上传到 github 等公共仓库导致密码泄露。
