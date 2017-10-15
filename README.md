# learn-recording

获取dom的宽高
1.内联样式：dom.style.width/height
2.计算样式（仅ie支持）：dom.currentStyle.width/height
3.计算样式：window.getComputedStyle(dom).width/height
4.dom.getBoundingClientRect().width/height

说明：3获取到的是标准模型下width/height，4获取到的是ie模型下的width/height
