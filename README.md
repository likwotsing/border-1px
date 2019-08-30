# border-1px
## 手写思路：

- 共有边框的几种class
  - border
  - border-top
  - border-right
  - border-bottom
  - border-left
  - border-topright
  - border-topbottom
  - border-topleft
  - border-rightbottom
  - border-rightleft
  - border-bottomleft

- 设置class的属性

  ```css
  position: relative;
  ```

- 设置伪元素的属性

  ```css
  content: '';
  overflow: hidden;
  position: absolute;
  ```

- 设置全局变量

  ```css
  :root {
      --border-1px-color: #eaeaea;
  }
  ```

- 分类别

  - width: 100%;height: 1px;
  - width: 1px; height: 100%;
  - border-top
  - border-right
  - border-bottom
  - border-left

- @media

  - 参考：[dpr](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/-moz-device-pixel-ratio)
  - 注意moz和webkit的前缀不一样 

  - -webkit -moz 和resolution: dpi 级别一样，谁在后面声明，谁生效
  - 目前不会用到不加前缀的 device-pixel-ratio 和 resolution: dppx
  - 注意`transform`的坐标轴

