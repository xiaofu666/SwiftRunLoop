# SwiftRunLoop
一款功能强大的轮播视图的工具
添加轮播试图后
```
let loopView = SFRunLoopView.init(frame: CGRect(x: 10, y: 100, width: self.view.frame.size.width - 20, height: 150))
self.view.addSubview(loopView)
```

一行代码便可实现视图轮播
```
let imgArr = [
            "https://t7.baidu.com/it/u=963301259,1982396977&fm=193&f=GIF",
            "https://t7.baidu.com/it/u=737555197,308540855&fm=193&f=GIF",
            "https://t7.baidu.com/it/u=1297102096,3476971300&fm=193&f=GIF",
            "https://t7.baidu.com/it/u=3655946603,4193416998&fm=193&f=GIF",
            "https://t7.baidu.com/it/u=12235476,3874255656&fm=193&f=GIF",
        ]
loopView.reloadViews(loopView.getImageViews(imgArr, bounds: loopView.bounds))
```

支持多种pageControl样式

![IMG_0046.PNG](https://upload-images.jianshu.io/upload_images/12555132-f0aa61cc33b4c541.PNG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![IMG_0045.PNG](https://upload-images.jianshu.io/upload_images/12555132-509892f00b409d7b.PNG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![IMG_0044.PNG](https://upload-images.jianshu.io/upload_images/12555132-46f6ccd6376a9f78.PNG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


还可支持图片样式
```
loopView.pageControlStyle = .animated
loopView.currentPageDotImage = UIImage.init(named: "pageControlCurrentDot")
loopView.pageDotImage = UIImage.init(named: "pageControlDot")
```
![IMG_0043.PNG](https://upload-images.jianshu.io/upload_images/12555132-2e48a0eb372a3747.PNG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


