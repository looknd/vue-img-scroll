# vue-img-scroll

一个模仿网易云音乐的vue图片滚动插件


based on vue 2.0

## Install
```
npm install vue-img-scroll 
```

### Local
```
git clone  https://github.com/ShanaMaid/vue-image-scroll.git

#安装依赖
npm install 

#启动
npm run dev

```


## Usage
```
<template>
  <div>
    <slider v-bind="setting">
  </div>
</template>

<script>
import slider from 'vue-image-scroll';

export default {
  components: {
    slider
  },
  data: function() {
    return {
      setting: {
        image: ['1.jpg', '2.jpg', '3.jpg']
      }
    }
  }
}
</script>          
```




## Update
- finish basics
- image add tagName and tagStyle

## Opitions
### Props
| Props     | Type    | Default | Description |
|-----------|---------|---------|-------------|
|styleObject| Object  | {width:'750',height:'240'}|scroll box style,please use lower camel case, eg: background-color => backgroundColor|
|image      | Array   | null    | imgae source path ,tagName,tagStyle; length >= 3|
|interval   | Integer | 2000    | unit: ms, rolling interval |
|imgStyle   | Object  | null    | image style, the same as `styleObject`  |
|autoRoll   | Boolean | true    |  `true` or `false` |
|direction  | String  | left    | scroll direction, `left` or `right` |