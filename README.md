![pixel_plurk_logo](https://user-images.githubusercontent.com/4176802/231839890-a084c430-d022-4727-ba72-2373189322c9.jpg)

# PixelPlurk.css

![preview](https://images.plurk.com/2APmsPVm8ltOILPA01A9mH.png)
像素風格噗浪佈景！


## 安裝

複製[本體CSS](https://github.com/maid-cat/PixelPlurk.css/blob/main/PixelPlurk.css)，貼到 `自訂佈景` -> `自訂佈景風格` 欄位

## 自訂

### 邊線顏色

預設為黑色邊線，可修改CSS開頭`/* 參數設定 */`區塊的`--pixel-color`值來調整為想要的顏色。例如：
```
  --pixel-color: #009487;
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