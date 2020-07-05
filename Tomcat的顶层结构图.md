Tomcat的顶层结构图:

![image-20200704180351925](C:\Users\lulud\AppData\Roaming\Typora\typora-user-images\image-20200704180351925.png)

Tomcat中最顶层的容器是Server，代表着整个服务器，从上图中可以看出，一个Server可以包含至少一个Service，用于具体提供服务。

Service主要包含两个部分：Connector和Container。从上图中可以看出 Tomcat 的心脏就是这两个组件.

多个 Connector 和一个 Container 就形成了一个 Service，有了 Service 就可以对外提供服务了

![image-20200704180701174](C:\Users\lulud\AppData\Roaming\Typora\typora-user-images\image-20200704180701174.png)

Container用于封装和管理Servlet，以及具体处理Request请求，在Connector内部包含了4个子容器

![image-20200704180811500](C:\Users\lulud\AppData\Roaming\Typora\typora-user-images\image-20200704180811500.png)