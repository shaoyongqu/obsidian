## 1 redis命令行客户端

```shell
redis-cli -h $(host) -p $(port) -a $(password)
```

执行后进入redis交互命令行。

若需要使用安全模式进入redis交互命令行，则去掉 -a 参数后，进入交互命令行，使用AUTH命令输入密码后，可正常使用。
```

```