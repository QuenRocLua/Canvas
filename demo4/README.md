### index1.html ###
绘制简单的矩形

>表1 矩形的清楚、描边和填充

| 方法 | 描述 |
|------|------|
|clearRect(double x,double y,double w,double h)|将制定矩形与当前剪辑区域相交范围内的所有像素清除。所谓的“清除像素”，将其颜色设置为全透明的黑色。|
|strokeRect(double x,double y,double w,double h)|使用如下属性，为指定的矩形描边： 1.strokeStyle:描边样式； 2.lineWidth:描边线宽；3.lineJoin:连接方式(bevel:斜面;round:圆;miter:斜角)4.miterLimit:最大斜接长度|
|fillRect(double x,double y,double w,double h)|使用fillStyle属性填充指定的矩形|

### index2.html ###
线性渐变和放射渐变

>表2 线性渐变，放射渐变方法

| 方法 | 描述 |
|------|------|
|CanvasGradient createLinearGradient(double x0,doubley0,double x1, double y1)| 创建线性渐变，参数表示渐变线的两个端点。该方法返回一个CanvasGradient实例。|
|CanvasGradient createRadialGradient(double x0, double y0, double r0, double x1, double y1, double r1) | 创建放射渐变，参数表示位于圆锥渐变区两端的原型。该方法返回一个CanvasGradient实例。|

>提醒：放射渐变的填充范围仅局限于由传递给createRadialGradient()方法的那两个圆形所定义的圆锥区域内，线性渐变使用最后一个渐变颜色来填充渐变线以外的区域。

### index3.html ###
路径、描边与填充

> 表3 路径相关的方法

| 方法 | 描述 |
|------|------|
| arc() | 在当前路径中增加一段表示圆弧或圆形的子路径。可以通过一个boolen参数来控制该子路径的方向。如果此参数是true，为顺时针，false为逆时针。如果在调用该方法时已有其他的子路径存在，那么arc()方法则会用一条线段把已有路径的终点与这段圆弧路径的起点连接起来。|
| beginPath() | 将当前路径之中的所有子路径都清除掉。|
| closePath() | 显示的封闭某段开放路径。用于封闭圆弧路径以及由曲线或线段所创建的开放路径。|
| fill() | 使用fillStyle对当前路径的内部进行填充。|
| rect(double x, double y, double width, double height) | 在坐标(x,y)处建立一个宽度为width,高度为height的矩形子路径。该子路径一定是封闭的，而且总是按逆时针方向来创建。|
| stroke() | 使用strokeStyle 来描绘当前路径的轮廓线。|