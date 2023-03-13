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

FATAL ERROR: Ineffective mark-compacts near heap limit Allocation failed - JavaScript heap out of me

````js
全局安装increase-memory-limit 命令行cmd ,dos窗口运行：cnpm install -g increase-memory-limit， 进入项目文件夹，运行：increase-memory-limit 可解决问题。 // 在 Node 中通过 JavaScript 使用内存时只能使用部分内存（64位系统下约为1.4 GB，32位系统下约为0.7 GB），这就是我们编译项目时为什么会出现内存泄露了，因为前端项目如果非常的庞大，webpack 编译时就会占用很多的系统资源，如果超出了V8对 Node 默认的内存限制大小就会出现刚刚错误了，那怎么解决呢？V8依然提供了选项让我们使用更多的内存。Node 在启动时可以传递 --max-old-space-size 或 --max-new-space-size 来调整内存大小的使用限制
````

