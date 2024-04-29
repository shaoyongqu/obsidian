## 1 redis命令行客户端
格式：
> redis-cli -h *host* -p *port* -a *password*

例：
```shell
redis-cli -h '127.0.0.1' -p 6379 -a password
```

执行后进入redis交互命令行。

若需要使用安全模式进入redis交互命令行，则去掉 -a 参数后，进入交互命令行，使用AUTH命令输入密码后，可正常使用。

也可以在redis-cli命令加-h -p -a 参数后加具体执行的redis命令，一个命令行达到执行redis命令的目的。

## 2 redis通用命令
### 2.1 查询符合指定模板的所有key
格式：
> KEYS *模板*

例：
```shell
KEYS *
KEYS a*
```
