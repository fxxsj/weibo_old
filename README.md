如果执行以下这条指令
`
SASS_BINARY_SITE=npm.taobao.org/mirrors/node-sass yarn
`
出现了类似 
`
The engine “node” is incompatible with this module. Expected version “>=12.14.0”. Got “12.10.0” 
`
这样的报错
这个报错是告诉我们模块不兼容
只需要执行 
`
yarn config set ignore-engines true
`
 后再次执行
 `
SASS_BINARY_SITE=npm.taobao.org/mirrors/node-sass yarn
`
就行了。
