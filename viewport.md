#viewport的基本原理


   1 . viewportj就是设备屏幕上用来显示，我们网页的一块区域，但不是浏览器可视区域，一般来说，移动设备上的viewport都要大于浏览器的可视区域。
   移动设备上的浏览器会把默认的viewport设置为980px或1024px，这样会造成浏览器出现横向滚动条。
   
   2 . css中的1px(像素)不等于设备的1px(像素)；分辨率越大，css中1px代表的物理像素就会越多。
  
   3 . 三个viewpor理论：layout viewport ；visual viewpoint，ideal viewp。
   
   　layout viewport:如果把移动设备上浏览器的可视区域设为viewport的话，某些网站就会因为viewport太窄而显示错乱，所以这些浏览器就决定默认情况下把viewport设为一个较宽的值，比如980px，这样的话即使是那些为桌面设计的网站也能在移动浏览器上正常显示了。   
   　visual viewport：浏览器的可视区域的大小。
   
   　ideal viewport:完美适配移动设备的viewport，它的宽度等于移动设备的屏幕宽度。
       
   
