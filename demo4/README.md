### index1.html ###
绘制简单的矩形

>表1 矩形的清楚、描边和填充

| 方法 | 描述 |
|------|------|
|clearRect(double x,double y,double w,double h)|将制定矩形与当前剪辑区域相交范围内的所有像素清除。所谓的“清除像素”，将其颜色设置为全透明的黑色。|
|strokeRect(double x,double y,double w,double h)|使用如下属性，为指定的矩形描边： 1.strokeStyle:描边样式； 2.lineWidth:描边线宽；3.lineJoin:连接方式(bevel:斜面;round:圆;miter:斜角)4.miterLimit:最大斜接长度|
|fillRect(double x,double y,double w,double h)|使用fillStyle属性填充指定的矩形|