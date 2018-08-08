#viewport的基本原理


   1 . viewportj就是设备屏幕上用来显示，我们网页的一块区域，但不是浏览器可视区域，一般来说，移动设备上的viewport都要大于浏览器的可视区域。
   移动设备上的浏览器会把默认的viewport设置为980px或1024px，这样会造成浏览器出现横向滚动条。
   
   2 . css中的1px(像素)不等于设备的1px(像素)；分辨率越大，css中1px代表的物理像素就会越多。
  
   3 . 三个viewpor理论：layout viewport ；visual viewpoint，ideal viewp。