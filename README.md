## vue-confirm

* 基于 vue 2.0 开发的 confirm 对话框插件
* 占用内存小，性能好，样式好看

## 效果
<img src="https://zwhgithub.github.io/vue-confirm/dist/demo2.jpeg" width="300px" />


 ## Demo
   [在线demo](https://zwhgithub.github.io/vue-confirm/dist/#/)

## Install

```shell
npm i vue-confirm  --save
cnpm i vue-confirm  --save //国内npm
```
## Quick Start Usage

```javascript
//main.js中引入
import Confirm from 'vue-confirm';
Vue.use(Confirm);



//在某个vue文件中使用;
this.$confirm('content');

//举例  点击确定和取消之后有回调函数的
this.$confirm('是否确定删除联系人')
  .then(() => {
    console.log('点击确定');
  })
  .catch(() => {
    console.log('点击取消');
  });
