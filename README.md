# js_opencv_zxing_qrcode_demo
front decode qrcode with opencv and zxing
用原生js实现的单html扫码,**opencv.js**和**zxing-js**用cdn调用

在线演示：［演示地址］（https://houseway.github.io/js_opencv_zxing_qrcode_demo/）

# 注意事项
## 1. 摄像头调用
使用 `navigator.mediaDevices.getUserMedia` 需要在https中
## 2. https
win10测试, `npm i -g anywhere`安装之后, 在项目中打开命令行窗口, 运行`anywhere 端口号`,模拟https环境
## 3. video标签宽高
监听`loadedmetadata`事件中,设置
```
video.height = video.videoHeight;
video.width = video.videoWidth;
```

# 好奇点
`navigator.mediaDevices.getUserMedia`的**constraints**在配置video宽高时,和`video`标签的宽高是反着的

# 资源链接
[opencv.js](https://docs.opencv.org/3.4/d5/d10/tutorial_js_root.html)

[zxing-js/browser](https://github.com/zxing-js/browser)