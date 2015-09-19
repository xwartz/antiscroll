# Antiscroll: 自定义默认滚动条

fork https://github.com/Automattic/antiscroll

## Features

- Supports mousewheels, trackpads, other input devices natively.
- Total size is **1kb** minified and gzipped.
- Doesn't magically autowrap your elements with divs
- Fade in/out controlled with CSS3 animations.
- Shows scrollbars upon hovering.
- Scrollbars are draggable.
- Size of container can be dynamically adjusted and scrollbars will adapt.
- Supports IE7+, Firefox 3+, Chrome, Safari

- IE10+ 使用 scss 隐藏默认滚动条
- 动态计算滚动区域

## Demo

Please click [here](http://codepen.io/xwartz/pen/Yyqdqb) to see it in action.

## Usage

1. 滚动区域标签添加 class ```antiscroll-inner```
1. 滚动外框添加 class ```antiscroll-wrap```
1. 初始化滚动条

```javascript
   $('.antiscroll-wrap').antiscroll();
```

## How does it work?

1. 滚动外框设置 `overflow: hidden`
2. 计算滚动区域的宽高，将其宽高加上滚动条的大小，使默认滚动条超出区域
3. 监听事件，更新滚动条

## Todo
- [ ] Mac未插如鼠标，默认滚动条为0，Firefox下无法隐藏默认滚动条
- [ ] 当滚动区域在调用前未渲染或 `display:none;`,没法正确计算宽高


## Dependencies

- [jQuery 2.0+](http://github.com/jquery/query)

## License 

MIT