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