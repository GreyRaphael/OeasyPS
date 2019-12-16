选择之后，右键，羽化，复制粘贴，进行图片的融合

color range     select/colorRange进行相同颜色的选择

shift+快捷键    同一个工具组切换(eg. shift+W)

选区即是编辑的区域
选区里面可以移动选区，选取外面单击会取消选区

Ctrl+T          变形工具

Edit/Stroke     描边

图层窗口，按住Ctrl+点击，将图层的内容选中

选区后，select/Modify/Expand    扩展选区的大小

智能对象        保持图像不马赛克 layer/Smart Objects

Ctrl+T          transform     (scale,rotate,screw,distort,perspective,wrap)

将一个图片放到另一个图片上时，选择图层模式为 multiply(正片叠底)
为了不损失像素，转换为智能对象

选区，Ctrl+T,进行移动、旋转、扭曲，enter，Ctrl+Shift+T就可以反复进行

拾色器/到其他图片点击（会出现自动吸管工具）

选区后          Select/Grow    扩大选区，用的是魔术棒的模式,选区连续
选区后          Select/Similar 扩大选区，用的是魔术棒的模式，选区非连续

选区后          Select/Refine Edge   调整边缘
选取后          Select/Save selection  防止选了其他之后，这一个消失了，以后要用的话Select/load Selection，对应有各种选区的运算

前景色，背景色
D               恢复默认的黑白（default）
X               交换黑白(exchange)

油漆桶工具
shift+油漆桶单击图片外面，将外面上色

Ctrl+A,Del      删除后剩下背景色（可设置）

在渐变编辑器中
将箭头按住上拖，下拖即可消失

Ctrl+Shift+Alt+UP(down)   复制移动

直方图（windows/Histogram）与image/adjustment相互配合
图片太亮（曝光过度），1-lightness（hue&saturation）,2-Brightness,3-Exposure,4-Equlize来进行调整
反差过度（逆光拍摄），1-shadow/highlight(暗的地方亮，亮的地方暗)

色阶（level）Ctrl+L：代替上面的直方图和adjustment的配合
0~黑箭头：变成纯黑（按住Alt再拖动，显示改变的区域）
白箭头~255：变成纯白
灰色箭头：整体直方图平移
对应于黑吸管，白吸管
灰吸管比较特殊：选出灰色（类似照相的白平衡功能）
channel:
选择R,G,B通道
然后用中间的灰箭头来调颜色
output:
黑箭头：选取黑的最值
白箭头：选取白的最值

当选中RGB其中的一个或者几个通道的时候，是对这几个通道的整体进行色阶调整

曲线（Ctrl+M）:色阶的二维版本（更加好用）
     单击：确定图像中的点在曲线上的位置
Ctrl+单击：确定图像中的点在曲线上的位置，并且锚点


选区(Select/ColorRange),然后Ctrl+U

Adjustment/ColorReplace

吸管：
shift                   增加
alt                     减少

matchColor              将一个张图颜色与另一张图匹配（选择source）

当发现不能操作颜色的时候，修改为
Image/Mode/RGB

渐变映射（Gradient Map）（match color）
渐变编辑器中，点击一个箭头，换一个位置，点击，复制粘贴这个箭头

adjust/vibrance
vibrance饱和度加的自然一些
saturation饱和度加的生硬一些

adjust/Black&White
分RGB光，滑动条右边的更加白一些，左边的黑一些

adjust/Desaturate
Ctrl+Shift+U:           直接转换为灰色图片（相当于Ctrl+U,把饱和度降到最低）

adjust/colorlookup
未知

adjust/posterize
色调分离
值越小越接近底稿

adjust/threshold（为了提取线条）
箭头左边纯白，右边纯黑
提取线条：
Filter/other/High Pass+Image/adjust/threshold+调整箭头得到线条

Lab模式：
L                       lightness
a                       Green to Magenta
b                       Blue to Yellow

可以复制一个图层，进行处理，将处理过头的部分用橡皮擦檫掉

Lab模式下冷暖平衡：
a,b通道的直方图是在0附近的，才会冷暖平衡

Brush刷子工具（使用前景色）
Mode:（画笔，油漆桶，渐变，图层）
  Normal：
  Dissolve:没有中间色来过渡，只是散开像素点
  Behind:在背后才能画出东西（背后没有像素点）
  Clear:相当于橡皮擦
  *****************************

  Darken:保留深色地方，涂抹浅色地方（变暗）
  Multiply:印刷学成色（CMYK），越打越暗
  ColorBurn:
  LinearBurn:
  DarkerColor:
  （这一组主要是变暗）
  *****************************
  Lighten:保留浅色地方，涂抹深色地方（变亮）
  Screen:光学成色（RGB），越打越亮（如果一个图片是黑色背景，用Screen粘贴到图层，可以直接去掉背景）
  ColorDodge:
  LinearDodge(add):
  LighterColor:
  （这一组主要是变亮）
  *****************************
  Overlay::
  SoftLight:
  HardLight:
  VividLight:
  LinearLight:
  PinLight:
  HardMix:
  （这一组主要是亮的更亮，暗的更暗）
  *****************************
  Difference:与前景色进行RGB作差
  Exclusion:与Difference差不多
  Subtract:
  Divide:
  *****************************
  Hue:用色相涂，保留其他
  Saturation:用饱和度涂，保留其他
  Color:用颜色直接涂，老照片恢复（相当于色相+饱和度）
  Luminosity:用选取颜色的明度涂，保留其他
  *****************************

画笔设置：
  不透明度是涂的最大值，流量是每一次流出的值，多涂几次就会变成最值
  纯度抖动与饱和度抖动相似
  湿边：中间会散开

画笔&铅笔：按住Shhift，点击两个点，画直线
铅笔工具/自动涂抹：交替使用前景色、背景色

吸管工具和信息调板配合使用（eyedropper(I) Info(F8)）
放大工具和导航调板配合使用（Zoom(z) windows/navigator）
色阶曲线和直方图调板配合使用（Ctrl+L,Ctrl+M windows/histogram）
历史记录画笔和历史记录调板配合使用（HistoryBrush(Y) windows/history）

历史记录画笔：
以历史调板的选中的地方为蓝本来涂抹

裁剪之后，图片大小改变了，有可能historyBrush不让用

CloneStamp Tools（s）
按住Alt取样，然后涂抹
可以在不同图片上面取样

PatternStamp Tools（s）
选择图案涂在目标图片上面

spotHealingBrush Tools(J)
直接点击去点点

HeallingBrush Tools(j)
按住Alt取样，然后涂抹
可以在不同图片上面取样

PatchTool(J)
Source:
选择一个地区，然后移动到完整的地方
Destination:
与source相反的操作

RedEyeTool
选取后，就可以去红眼

Blur&Sharp&Smudge Tools
涂抹工具：变形+模糊

Dodge&Burn&Sponge(O)
加深：可以选择中间调，阴影，高光进行加深
减淡：
海绵：增加，降低饱和度

Eraser&BackgroundEraser&MagicEraser
BackgroundEraser:会转为图层      按住Alt取样，然后保护前景色,擦除其他颜色
Magic:Wand+Del

图层蒙版（Mask）
黑色是蒙住了，白色没有蒙住
Alt+点击蒙版               禁用图层蒙版
Shift+点击蒙版             只显示图层蒙版
解开锁链                   点击图层移动的是图层，点击蒙版移动的是蒙版
利用好反相（颜色）                   Ctrl+I

图层组
可以对整体进行蒙版，然后在组内仍然可以蒙版

渐变工具补充
刷了一个渐变之后，还要再加一个，在渐变工具栏，选择印刷模式（正片叠底）

剪切蒙版（都是可以转换为普通蒙版的,建议使用图层蒙版）Layer/CreateClippingMask
上图下形（上面负责图，下面负责形状）
Alt+鼠标在两个图层之间       剪切蒙版开关

Alpha通道（保存的选区）

选区,select/Save Select，select/load select（根据Alpha通道来载入）
Ctrl+点击 Alpha通道           获得选区

选区                          Alpha通道
快速蒙版                      建立临时的Alpha通道(Q)
蒙版                          本质上也是alpha通道

双击快速蒙版                  可以设置属性，反相

精细的使用图层蒙版，可以反复的修
粗糙的使用快速蒙版

选区后，添加图层蒙版，也可以

原色通道
分离                          在通道面板下拉菜单，splitChannel
合并                          在通道面板下拉菜单，MergeChannel

将原色通道复制之后，新生成的通道就是AlphaChannel，不再记录颜色信息，只是记录选中没选中信息。

通道可以复制黑白的信息到其他通道中

图层所有东西设置好之后，影响的是RGB通道
其他通道：专色（打光的），蒙版，选区

RGB先要转到灰度，才能转Duotone

索引颜色对应256种颜色，RGB有8bit,16bit,32bit

图层：
Ctrl+E                        向下合并一个通道
双击图层锁                    转换成图层，Layer/New/BackgroundFromLayer
右击图层缩略图                图层属性设置，可以给图层设置颜色名称，多个叠加在一起的时候，右键可以选择图层
Alt+点击图层眼睛              只显示这个图层
图层上面有4种锁定
透明锁定                      不能对透明区域操作
画笔锁定                      不能使用画笔
移动锁定                      不能移动
全部锁定                      不能进行任何操作（背景图层就是这样）

填充图层（Layer/NewFillLayer）图层面板的黑白半圆
Solid,Gradient,Pattern
注意：填充图层不让选区，要先栅格化（layer/rasterize/fill content）,或者新建一个图层，然后合并这两个图层，实现栅格化

调整图层(等价于图像的某些命令+蒙版）：
色阶调整图层                  Layer/newAdjustmentLayer/leverl                选区后，进行调整，然后利用蒙版进行细加工

图层混合模式：
上色                           新建图层/涂上颜色/图层混合模式改为“颜色”
选择图层混合模式

图层混合选项：图层混合模式只是图层混合选项的一种（双击图层）

LayerStyle:
Opacity                       整体的不透明度
Fill Opacity                  填充部分的不透明度
BlendIf:
Alt+点击箭头                  拆开箭头
箭头左边是没有，右边是有，拆开是过渡

InnerShadow
NnnerGloW
OuterGlow
DropShadow

从上到下
Color Overlay
Gradient Overlay
Pattern Overlay

图层复合（view/layerComps）
不能保存图层的上下关系，能保存图层中图形的相对位置

矢量工具（钢笔，文本，矢量选择，图形）
矢量选择（黑箭头）               选择全部
矢量选择（白箭头）               选择单个点或者多个点

选区后点击Channel的新建，即可建立Alpha Channel
选区后点击Path的load,即可建立临时Path，然后拖动到新建即可建立稳定的path

Pen tools
ConvertPointTools               可以折起钢笔锚点画的切线
矢量蒙版（layer/vectorMask）：没有中间过渡的情形

先要生成一个路径，然后layer/vectorMask/path，接着同样可以用钢笔来调节

选择pathPanel，可以用钢笔画路径

选择path，然后用蒙版的新建，就可以建立矢量蒙版

钢笔工具：Shape,path,Pixels相互转化
shape2Pixels                  rasterize
path2pixels                   rasterize
shape2path                    pathPanel
pixels2path                   选区，新建

双击工作路径变成一般路径
右击一般路径                  FillPath,StrokePath
StrokePath                    可以用来生成蜗牛组成的蜗牛
如果路径不闭合，从头到尾的描边（图形）
选区描边不能用画笔描边，路径描边可以用各种笔描边

不透明度                      0~9（0:100%，9:90%）

创建矢量蒙版                  Ctrl+创建蒙版

tips:
矢量蒙版控制形状，图层蒙版控制隐藏，不透明

文字蒙版工具：
先写字，切换到移动工具，自动变成选区
写好的文字可以用Ctrl+T变形

先画一条路径，然后保存路径，然后就可以在路径上写文字，pathMoveTool可以进行各种移动

闭合的路径可以在路径上写字，也可以在路径包围的内部写字

图章存储为png或者gif格式

滤镜：
先用wand选区，然后RefineEdge细调，效果相当好
VanishingPoint:三维空间的调整

智能对象，马赛克之后仍然能够找回

扭曲/置换:                     用模型去置换材质，然后叠加材质

祛痘可以使用Noise调节

锐化，尽量在LAB模式的L通道做

渲染，打光

高反差保留，可以用于提取线稿