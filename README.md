# IoTLauncher
面向IoT时代的桌面系统

## 方案设计

由于IOT时代，类似车机，冰箱等屏幕与手机屏幕的操作习惯不同，通常不太易于进行非常细致的近距离操作，所以希望能通过桌面透出尽量多的有用信息，并且能在桌面即可完成大部分常用设置。

当然桌面只是提供容器，这里就需要实现一套规则，能让各个应用自己实现要显示在桌面的内容，听着有点像桌面小部件（widget），是的，widget的时代来了，但是我们希望实现的是更加易于开发，更加灵活的widget。

初步设想是使用多个window实现类似WindowsPhone的效果。

参考widget的设计，会让桌面的window内容带一些快捷操作以及状态显示，原生widget会限制使用特定的控件，并且是运行在系统进程，这些限制都是需要完善拓展的。



最简单的实现方式，完全使用widget实现。
