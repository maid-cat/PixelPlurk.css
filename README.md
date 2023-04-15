![pixel_plurk_logo](https://user-images.githubusercontent.com/4176802/231839890-a084c430-d022-4727-ba72-2373189322c9.jpg)

# PixelPlurk.css

像素風格噗浪佈景！

![preview](https://images.plurk.com/2APmsPVm8ltOILPA01A9mH.png)


## 安裝

複製[本體CSS](https://github.com/maid-cat/PixelPlurk.css/blob/main/PixelPlurk.css)，貼到 `自訂佈景` -> `自訂佈景風格` 欄位

## 特色

### 高完成度！

調整了河道、噗文展開、頂端列、浮動視窗、主控面板、發噗介面...

<img src="https://images.plurk.com/2D3D03XRbHLObfoyscy5TY.png" width="30%"></img>

### 自訂色彩

可自行搭配背景色與邊線顏色，

<img src="https://images.plurk.com/6zoMTZdw7DHQOzGYa0GT2C.png" width="30%"></img>
<img src="https://images.plurk.com/1vaULZXh8vqCCeKOEenF2C.png" width="30%"></img>


## 自訂

### 邊線顏色

預設為黑色邊線，可修改CSS開頭`/* 參數設定 */`區塊的`--pixel-color`值來調整為想要的顏色。例如：

```
  --pixel-color: #009487;
```

### 河道背景圖

建議使用語法來更改背景，避免圖片被壓縮。

```
._lch_::before {
  display: block;
  position: fixed;
  content: '';
  width: 100%;
  height: 100%;
  background-image: url(<圖片網址>);
  background-size: cover;
  image-rendering: pixelated;
}
```


### 噗文背景色

```css
.timeline-cnt .plurk_cnt, #form_holder, :is(url({)), .pop-window-view, :is(url(})) {
  background-color: <色碼>;
}
#form_holder .plurk_cnt, #form_holder .login_to_see, :is(url({)), .divplurk, .response_box, .mini_form, :is(url(})) {
  background-color: transparent !important;
}
```

### 主控台背景色

```css
.segment-content {
  background-color: <色碼>;
}
```



## 特別感謝

- [NES.css](https://nostalgic-css.github.io/NES.css/): 像素風語法參考
- [俐方體11號／Cubic 11](https://github.com/ACh-K/Cubic-11): 像素風字型
- [CSS-Tricks](https://css-tricks.com/cut-corners-using-css-mask-and-clip-path-properties/): `conic-gradient`語法