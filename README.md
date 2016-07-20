# UI/UX 设计规范与资源整理


目录

[toc]




## 1. 设计规范

### 1.1 移动端

> 移动端我们分为原生app设计和移动网页设计，原生app遵循苹果和谷歌的官方文档，在设计时尽可能的使用手机系统自带的组件，保证视觉和操作的统一性。



-官方设计规范英文版
- 
[iOS Human Interface Guidelines](https://developer.apple.com/ios/human-interface-guidelines/) 

[Google Material Design](https://material.google.com/)

-官方设计规范中文翻译版
- 
[ios9 人机交互指南](http://wiki.jikexueyuan.com/project/ios-9-human-computer-interface-guidelines/)

[Material Design 中文版](http://wiki.jikexueyuan.com/project/material-design/)
 
- 中台移动端设计规范
- 
根据对官方文档的分析以及我们的产品的页面需求，我们总结出了目前中台系统下移动端的设计规范。该规范主要以IOS的设计为标准，同时根据行业主流APP中的界面交互方式，归纳出通用样式的app所需的设计元素以及典型页面的设计规范。
  

- 移动网页规范
- 
对于手机上的移动网页，即不是原生开发的页面，我们以微信团队出品的weUI作为规范参考。

 微信weUI
 
 [weUI组件](https://weui.io/#/)
 
 [weUI视觉标准 sketch](https://github.com/weui/weui-sketch)
 
 weUI手机预览二维码
 
![此处输入图片的描述][1]


----------


### 1.2 PC端

>pc端的网页设计，我们基于bootstrap框架设计响应式的网页，以适配不同尺寸的屏幕。设计时尽量使用bootstrap的默认参数和组件，保证视觉和操作的统一性。

- [bootstrap3 中文文档](http://v3.bootcss.com/)
- 
bootstrap的文档中介绍了页面的CSS属性以及各组件的基准样式，在设计时尽量以此为标准。

- [antdesign](http://ant.design/)

当有一些特殊的界面或交互样式bootstrap里没有提及的，可以参照antdesign.

- [<font color="red">中台管理后台web设计规范</font>](https://www.zybuluo.com/rabbielulu/note/441897)
布局规范和基本组件都按照bootstrap的默认参数，特殊页面需求参考了antdesign以及行业其它管理后台的样式。


 

 


----------


## 2. 设计流程以及工具


### 2.1 功能和流程的交互线框图

 >制定流程的过程中，可以使用线框组件，也可以直接截图参考案例，快速的组合出页面流程，从而确定页面需求。

[墨刀](https://modao.cc) <font color="red"><i class="icon-star"></i> (推荐)</font> 
 
操作方便快速，适合跳转逻辑比较简单的交互，基本上可以满足移动端的交互和效果预览。

[Axure](http://pan.baidu.com/s/1slCIeZz)

功能全面，适合比较复杂的页面，以及详细的交互说明。



### 2.2 视觉效果图

页面流程确定后开始视觉效果图的设计，PS中我们以**750*1334px**， 72ppi为设计稿尺寸。（原因详情见中台移动端设计规范-尺寸标准）

 - photoshop cc 2015
 - sketch
 - illustrator

>Photoshop推荐使用cc2014 以上的版本，因为新加入的“画板”功能，以及CC以上版本对于矢量图形的编辑功能加强，都利于了移动页面的开发。（请抛弃CC以下的版本）

 **软件下载：**
 
 已在互动部网络硬盘里分享了最新版Adobe Family“全家桶”，文件为iso格式。
 
win7系统安装虚拟光驱软件deamon tools后打开；

win10系统使用右键“资源管理器”打开，选择需要的软件安装。

  Mac软件下载  链接: http://pan.baidu.com/s/1pLeqptx 密码: 1m5i

**跨屏预览:**

使用app在手机上实时预览电脑工作稿的效果

- photoshop内置Device preview
- sketch内置mirror
- 
以上两款内置功能都需要下载搭配的app，但是adobe preview在中国区苹果商店是搜不到的，只能切换到美区；而sketch到mirror需要30元付费下载。

- [PS play](https://isux.tencent.com/app/psplay) <font color="red"><i class="icon-star"></i> (推荐)</font> 

推荐使用腾讯出品的免费app PS play.

### 2.3 标记图

设计稿完成后，需要给前端交付标记图，以保证设计准确呈现。

[标你妹啊](http://www.biaonimeia.com/)  <font color="red"><i class="icon-star"></i> (推荐)</font> 

在线自动标注工具，简便。上传psd至网站，分享链接给前端人员，即可自行查看标记信息。

[Assistor PS](http://witstudio.net/)

辅助手动标记工具，ps外挂软件，单独运行，可在图层上生成标记图层。

[Zeplin](https://zeplin.io/)

zeplin和标你妹啊类似，导入文档自动标记，除此之外Zeplin还会生成一份当前文件字体和颜色的style guide，同时可以添加文字评论，并包含切图资源。不过由于Zeplin为境外服务器，注册时需要梯子，注册后使用不需要梯子。


### 2.4 资源切图

ios需要切@2x和@3x两种的图

安卓需要hdpi,xhdpi,xxdpi三种尺寸的图

界面中的元素都以矢量图形来绘制

sketch和phtoshop cc 2015都有了快速切图功能，可以直接切图。

- 切图插件[cutterman](http://www.cutterman.cn/cutterman) <font color="red"><i class="icon-star"></i> (推荐)</font> 

 windows下的Photoshop切图插件，快速一键导出安卓和ios所需尺寸的资源图片。

- web图标可以使用icon font文件，将图形以类似字体的形式嵌入到页面中.

图标来源如[阿里巴巴矢量图标库](http://www.iconfont.cn/)，[fontawesome](http://fontawesome.io/icons/).

- 也可以导出svg或pdf格式的矢量图片，程序可以基于一套资源自动适配大小。AI和sketch都可以生成矢量图标，PS则需要借助插件[zeick](https://gumroad.com/l/Zeick4/25OFF),将ps的文件导出成svg格式.


- 其它切图插件[LayerCraft](http://lab.rayps.com/lc/).


----------


## 3. 资源网站

### 3.1 矢量图标资源

[阿里巴巴矢量图标库](http://www.iconfont.cn/) <font color="red"><i class="icon-star"></i> (推荐)</font> 

[fontawesome](http://fontawesome.io/icons/)<font color="red"><i class="icon-star"></i> (推荐)</font> 

[ico moon](https://icomoon.io/)

[Material icons](https://design.google.com/icons/)


### 3.2 UI Kit 组件模版资源

[iOS9 ui组件](http://ozzik.co/freebies/ios9kit)

[Material Design UI组件](https://ui8.net/products/free-material-ui-kit)

[Sketch APP sources](http://www.sketchappsources.com/)

###3.3 无版权大图资源

https://pixabay.com/zh/

http://www.imcreator.com/free

http://publicdomainarchive.com/


### 3.4 灵感图参考图

[花瓣网](http://huaban.com/) 综合图片搜索

[behance](https://www.behance.net/) 图形，交互，整套设计

[dribbble](https://dribbble.com/) 图形，动效设计

[90设计](http://90sheji.com/) 电商 banner 

[shutterstuch](http://www.shutterstock.com/) 矢量插图，图标

[Pinterest](https://www.pinterest.com/) 综合图片搜索

### 3.5 充电网站和行业用户体验团队博客

[UI中国](http://www.ui.cn/)

[优设](http://www.uisdc.com/)

[腾讯社交用户体验设计团队IXUI](http://isux.tencent.com/)

[腾讯移动互联网团队](http://mxd.tencent.com/)

[阿里巴巴国际用户体验团队](http://www.aliued.com/?cat=15)

[网易用户体验中心](http://uedc.163.com/)






























  [1]: https://cloud.githubusercontent.com/assets/4652816/15662614/178efd46-2725-11e6-8952-09d7836e968d.png







