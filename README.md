# 百度地图 拱墅区教育地图
1. 百度地图绘制刑侦边界的时候，边线为dashed虚线的时候会引起地图卡顿；
2. 引用个性化地图碰到的问题：
    1. 引用线上的个性化地图的ID加载地图拖动和放大的时候会引起地图卡顿，解决办法是：将线上的地图的JSON数据拷到本地，本地引用；
    2. 当引用个性化地图的时候，`centerAndZoom(point,zoom)` 第一个参数不能传入string类型，不然会报错，解决方案是用`map.setCenter(str)`，然后在用一个变量来存储`map.getCenter()`的返回值，再放进`centerAndZoom()`中即可；

    