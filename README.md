![pixel_plurk_logo](https://user-images.githubusercontent.com/4176802/231839890-a084c430-d022-4727-ba72-2373189322c9.jpg)

# PixelPlurk.css

像素風格噗浪佈景！

![preview](https://images.plurk.com/2APmsPVm8ltOILPA01A9mH.png)

- 製作：[欸個](https://www.plurk.com/egg820/invite)
- 排版建議、字型技術支援：[千秋](https://www.plurk.com/akira02/invite)

## 安裝

複製[本體CSS](https://github.com/maid-cat/PixelPlurk.css/blob/main/PixelPlurk.css)，貼到 `自訂佈景` -> `自訂佈景風格` 欄位


## 特色

### 高完成度！

調整了河道、噗文展開、頂端列、浮動視窗、主控面板、發噗介面...

<img src="https://images.plurk.com/2D3D03XRbHLObfoyscy5TY.png" width="40%"></img>
<img src="https://images.plurk.com/RG7wHrSuAlW06ss0gZyc0.png" width="40%"></img>
<img src="https://images.plurk.com/4TSdsZTyyjp6I1ZqMARGcY.png" width="80%"></img>


### 自訂色彩

可以依喜歡的風格，自由選擇背景色與邊線色彩

<img src="https://images.plurk.com/6zoMTZdw7DHQOzGYa0GT2C.png" width="40%"></img>
<img src="https://images.plurk.com/1vaULZXh8vqCCeKOEenF2C.png" width="40%"></img>
<img src="https://images.plurk.com/sbU5O7sslqxiNcmfiKZyZ.png" width="40%"></img>
<img src="https://images.plurk.com/1koyae3ZxNNbyrFVQC9cKr.jpg" width="40%"></img>


## 自訂

### 邊線顏色

預設為黑色邊線，可修改CSS中 `/* 參數設定 */` 區塊的 `--pixel-color` 值來指定想要的顏色。例如：

```
  --pixel-color: #009487;
```

### 河道背景圖

建議使用語法來更改背景，避免圖片被壓縮。

```css
/* 河道背景圖 */
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
/* 噗文背景色 */
.timeline-cnt .plurk_cnt, #form_holder, :is(url({)), .pop-window-view, :is(url(})) {
  background-color: <色碼>;
}
#form_holder .plurk_cnt, #form_holder .login_to_see, :is(url({)), .divplurk, .response_box, .mini_form, :is(url(})) {
  background-color: transparent !important;
}
```

### 主控台背景色

```css
/* 主控台背景色 */
.segment-content {
  background-color: <色碼>;
}
```



## 特別感謝

- [NES.css](https://nostalgic-css.github.io/NES.css/): 像素風語法參考
- [俐方體11號／Cubic 11](https://github.com/ACh-K/Cubic-11): 像素風字型
- [CSS-Tricks](https://css-tricks.com/cut-corners-using-css-mask-and-clip-path-properties/): `conic-gradient`語法