# vue-search
用于搜索的input组件
![](//cdn.51talk.com/apollo/images/5304470fcb7302b97e43f30047a3bf28.png)
## install
NPM
```
npm install nat-vue-search
```
## 用法
```
<template lang="html">
    <div id="project-features">
        <h1 class="title">Vue 搜索框</h1>
        <div class="features">
            <search v-model="searchText"></search>
            <p>{{searchText}}</p>
        </div>
    </div>
</template>
```
```
<script>
    import search from 'vue-search';

    export default {
        name: 'ProjectFeatures',
        components: {
            search
        },
        data() {
            return {
                searchText: ''
            }
        }
    };
</script>
```
## API
#### props
属性 | 说明 | 类型 | 默认值
---|---|---|---
placeholder | placeholder | string | 请输入查询信息
## 启动
```
npm run dev
```
## 编译
```
npm run build-lib
```
