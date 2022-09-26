发不了请求需要服务器重启

路由前置守卫不生效，需要放在app.mount('#app') 前面

node渲染时没有window

今天在使用git的时候，发现无论怎么改.gitignore文件都无法添加文件到版本控制，最后发现是缓存的原因，需要删除缓存再重新add
git rm -rf --cached xxx

git察觉不到更新就清缓存

**nuxt3启动BUG**[nuxt] [request error] [unhandled] [500] Cannot read properties of undefined (reading 'modules')