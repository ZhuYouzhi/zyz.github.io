### 简明教程

[IDEA建立Spring MVC Hello World 详细入门教程](https://www.cnblogs.com/wormday/p/8435617.html)

关键点：

<context:component-scan base-package="wormday.springmvc.helloworld"/>
配置后会报”context“标签无法识别的错误
完成配置如下

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context-3.0.xsd"
>

    <context:component-scan base-package="wormday.springmvc.helloworld"/>
</beans>
