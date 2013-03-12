# 元素载入中插件

对指定（块级）元素应用载入中的插件

## 用法

### 引入

```html
    <link rel="stylesheet" href="loading/style.css" />
    <script type="text/javascript" src="jquery.loading.js"></script>
```

### 使用

```javascript
var elem = $('#target');

// 显示载入中样式
elem.loading();
// 或者加入参数
elem.loading({
    zIndex: 9999,
    opacity: 0.95
});

// 加载并渲染数据
//

// 移除载入中样式
elem.loading('hide');
```

## 选项

### `zIndex` 层级设定
当布局中有其他元素 z-index 比较高时，可以手动指定该值，默认值为 999。

### `opacity` 元素透明度
载入中元素的透明度，默认为 0.85。