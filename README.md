# learn-recording

获取dom的宽高
1.内联样式：dom.style.width/height
2.计算样式（仅ie支持）：dom.currentStyle.width/height
3.计算样式：window.getComputedStyle(dom).width/height
4.dom.getBoundingClientRect().width/height

说明：3获取到的是标准模型下width/height，4获取到的是ie模型下的width/height

BFC
概念：块级格式化上下文
创建：
1.float取none以外的值
2.position取static、relative以外的值
3.display：table/table-cell
4.overflow:取visible以外的值

原理：
1.bfc元素在垂直方向上的边距发生重叠
2.bfc的区域不会与浮动元素的box重叠
3.bfc是一个独立的容器，外面的元素不会影响里面的元素，里面的元素也不会影响外面的元素
4.计算bfc高度时浮动元素也会参与计算
