## 一、Apache与Tmocat的关系、区别、相同点

1 .Apache和Tomcat都是web网络服务器，在进行HTML、JSP等开发过程中，需要准确的知道各自的特点

2 .区别：
       
   - -Apache是web服务器解析静态页面如：HTML
   - -Tomcat是web服务器解析动态页面如：jsp
   - -Apache是有C语言实现的，支持各种特性和模块从而来扩展核心功能。
   - -Tomcat是Java编写的，更好的支持Servlet和JSP。
   
   
3 .相同点：
   
   - -两个都是Apache组织开发的
   - -两个都是有HTTP服务功能
   - -两个都是开源免费的
   
 4 .整合关系：
 
   - -如果客户端请求的是静态页面，则只需要Apache服务器响应请求。
   - -如果客户端请求动态页面，则是Tomcat服务器响应请求，将解析的jsp网页代码传回Apache服务器中，在由Apache服务器返回给客户端。
   - -Apache和Tomcat都是独立的，可以在同一台服务器上集成。
  
   -----------------
   
##二、Jetty 与 Tomcat的比较

  1 .相同点：
 
   - -Tomcat和Jetty都是一种Servlet引擎，它们都支持标准的servlet规范和JavaEE的规范。
  
  2 .不同点：
  
   - -架构比较：
       
      Jetty的架构比Tomcat的更为简单 
      Jetty的架构是基于Handler来实现的，主要的扩展功能都可以用Handler来实现，扩展简单。 
      Tomcat的架构是基于容器设计的，进行扩展是需要了解Tomcat的整体设计结构，不易扩展。
      
   - -性能比较 ：
      
      Jetty和Tomcat性能方面差异不大 
      Jetty可以同时处理大量连接而且可以长时间保持连接，适合于web聊天应用等等。 
      Jetty的架构简单，因此作为服务器，Jetty可以按需加载组件，减少不需要的组件，减少了服务器内存开销，从而提高服务器性能。 
      Jetty默认采用NIO结束在处理I/O请求上更占优势，在处理静态资源时，性能较高
      
   - -少数非常繁忙;Tomcat适合处理少数非常繁忙的链接，也就是说链接生命周期短的话，Tomcat的总体性能更高。 
      Tomcat默认采用BIO处理I/O请求，在处理静态资源时，性能较差。
      
   - -其它比较 
   
      Jetty的应用更加快速，修改简单，对新的Servlet规范的支持较好。 
      Tomcat目前应用比较广泛，对JavaEE和Servlet的支持更加全面，很多特性会直接集成进来。

   
