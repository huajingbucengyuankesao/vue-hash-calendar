[![Build Status](https://travis-ci.org/TangSY/vue-hash-calendar.svg?branch=master)](https://travis-ci.org/TangSY/vue-hash-calendar)

# 按照惯例，先上效果图

![calendar.gif](https://www.hxkj.vip/demo/calendar/calendar.gif)

# vue-hash-calendar

* 基于 vue 2.X 开发的日历组件
* 支持手势滑动操作·1
* 原生 js 开发，没引入第三方库
* 上下滑动 切换 周/月 模式
>【周模式中】 左右滑动可切换 上一周/下一周
 【月模式中】 左右滑动可切换 上一月/下一月
 
# 安装使用说明
  ```
npm i vue-hash-calendar
```

  ```
// 在入口文件中（main.js），导入组件库
import vueHashCalendar from 'vue-hash-calendar'
// 引入组件CSS样式
import 'vue-hash-calendar/lib/vue-hash-calendar.css'
// 注册组件库
Vue.use(vueHashCalendar)
```

  ```
  // 在VUE文件中引入组件
   <vue-hash-calendar></vue-hash-calendar>
```

# Demo

![demo_qrcode.png](https://www.hxkj.vip/demo/calendar/demo.webp)

或者请用浏览器的手机模式查看：[https://www.hxkj.vip/demo/calendar/](https://www.hxkj.vip/demo/calendar/)

* 🎉 觉得好用可以给一个 star 哦~~ 🎉

## github地址：[https://github.com/TangSY/vue-hash-calendar](https://github.com/TangSY/vue-hash-calendar) 

# API

| 属性          | 说明                                                                                                   |  默认  | 是否必传 |
| :------------ | :----------------------------------------------------------------------------------------------------- | :----: | :------: |
| model      | 日历组件以哪种形式展示。inline：内联的方式。dialog：弹窗的方式                                                            |   inline   |    否    |
| defaultDatetime| 指定默认时间。数据类型为 Date                                                      |   当前时间   |    否    |
| format       | 确认日期时，回调事件返回的日期格式。如“YY/MM/DD hh:mm” 、“YY 年 MM 月第 DD 天，当前时间 hh 时 mm 分”                                      |  YY/MM/DD hh:mm   |    否    |
| weekStart      | 以星期几作为日历每一周的起始星期。可选['sunday', 'monday', 'tuesday', 'wednesday', 'thursday', 'friday', 'saturday']            | sunday |    否    |
| pickerType  | 选择器类型 datetime：日期+时间   date：日期   time：时间                                                               | datetime |    否    |
| showTodayButton    | 是否显示返回今日按钮                                                          |   true    |    否    |
| confirm | 确认选择的回调事件。当 model 为 inline 的时候没有该事件                                                            |  ---  |    否    |

## Other

* 在 dialog 模式中，如何显示日历组件？
```
<vue-hash-calendar ref="picker"></vue-hash-calendar>

//调用内置 show 方法
this.$refs.picker.show();
```

* 如果有其他问题， 或者功能上不兼容的。可以邮件沟通 t@tsy6.com，或者 github 提交 issue。



## Project setup
```
npm install
```

## Compiles and hot-reloads for development
```
npm run serve
```

## Compiles and minifies for production
```
npm run build
```
