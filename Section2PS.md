# Photoshop window

- [Photoshop window](#Photoshop-window)
  - [window](#window)
  - [view](#view)
  - [Transform](#Transform)
  - [Crop](#Crop)
  - [Selection](#Selection)
    - [Marquee](#Marquee)
    - [Laso](#Laso)
    - [Magic wand](#Magic-wand)

## window

## view

some useful:
- `F`(view/screen mode): 在基本窗口、放大窗口、全屏之间切换;
- `space`: HandTool

Menubar/View
- `ctrl+0`: fit to screen
- `ctrl+1`: 100%
- `ctrl+2`: R,G,B all channels
- `ctrl+3`: R channel
- `ctrl+4`: G channel
- `ctrl+5`: B channel

Trick:
- ZoomTool与Navigator panel配合;
- RulerTool与info panel配合;

Example: 制作1寸照片
1. crop tool按照5:7裁剪
2. Image/ImageSize/调整DPI=300, width=2.5cm, height=3.5cm
3. 新建如下图片
   > <img src="example2/1inch_photo01.png" width="400">
4. 移动调整的头像到新建的空白图像，打印
   > <img src="example2/1inch_photo02.png" width="400">
5. 同理2寸照片
   > <img src="example2/2inch_photo.png" width="400">

## Transform

Example: 倾斜图片调正method1
1. RulerTool
2. Image/ImageRotation/Arbitratry

Example: 倾斜图片调正method2
1. RulerTool, 展开的菜单选择StraightenLayer

Example: 倾斜图片调正method3(Best)
1. CropTool, 展开的菜单选择Straighten
2. 拉一条线
   > <img src="example2/transform01.png" width="400">

## Crop

- crop: crop选区可以旋转所以可以旋转裁切
- perspective crop: 近大远小

Example: 制作1寸照片
1. Image/ImageSize/DPI=300
2. CropTool菜单/Width=2.5cm, Height=3.5cm, DPI=300
3. Crop
4. 新建如下图片
   > <img src="example2/1inch_photo01.png" width="400">
5. 移动调整的头像到新建的空白图像，打印
   > <img src="example2/1inch_photo02.png" width="400">

Example: 两张图片拼接到一张图中
> <img src="example2/pic1.png" height="400">
> <img src="example2/pic2.png" height="400">
1. pic1的Image/CanvasSize增大
2. pic2移动到pic1, 设置pic2的图层透明度
3. 对准，然后恢复不透明度，就可以拼接
   > <img src="example2/pic3.png" height="400">

Example: 多张图拼接到一张图中(Recommended)
1. File/Automate/Photomerge/OK
> ![](example2/photomerge.png)

## Selection

### Marquee

Shortcuts:
- `m`: activate marquee
- `Shift+M`: switch marquee
- `Ctrl+D`: Deselect
- `Ctrl+E`: Merge layers
- `Ctrl+J`: Copy selection & paste to new layer

Example: 去logo
1. method1: 选区, 复制粘贴(`Ctrl+J`)
2. method2: 选区, Alt移动粘贴
3. method3: 选区, `Ctrl+T`变形覆盖

Example: 修复缺的老照片
- 选区, `Ctrl+T`变形覆盖

Selection Operation:
- `Shift`: 并集
- `Alt`: 差集
- `Shift+Alt`: 交集

Selection Fill: 选区, Edit/Fill
- Foreground color fill: `Alt+Del`, `Alt+Backspace`
- Background color fill: `Ctrl+Del`, `Ctrl+Backspace`

### Laso

Shortcuts:
- `L`: activate laso
- `Shift+L`: switch laso
- `Del`: 删除一个点
- `Esc`: 删除全部的点
> magnetic lasso: 最后一点双击，得到闭合选区

### Magic wand

Shortcuts:
- `W`: activate wand

Trick:
- Tolerance
- Continuous
- Sample all layers: 下图包含三个图层
  > <img src="example2/sample_all_layers.png" height="300">