发不了请求需要服务器重启

路由前置守卫不生效，需要放在app.mount('#app') 前面

node渲染时没有window

今天在使用git的时候，发现无论怎么改.gitignore文件都无法添加文件到版本控制，最后发现是缓存的原因，需要删除缓存再重新add
git rm -rf --cached xxx

git察觉不到更新就清缓存

**nuxt3启动BUG**[nuxt] [request error] [unhandled] [500] Cannot read properties of undefined (reading 'modules')

Nginx 端口被占用问题。

```
输入命令：netstat -ano，列出所有端口的情况。
查看被占用端口对应的PID，输入命令：netstat -aon|findstr "8080"，回车，记下最后一位数字，即PID,这里是2668。
继续输入tasklist|findstr "2668"，回车，查看是哪个进程或者程序占用了2668端口，结果是：TIM.exe
```

Original error: Cannot use import statement outside a module

```javascript
// package.json中配置

"type": "module"
```

vue3 源码无法 commit

``` javascript
git commit -m "chore: add s" --no-verify   // 关闭验证



```

