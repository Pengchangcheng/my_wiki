# spring Schema
```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns="http://www.springframework.org/schema/beans"
	xmlns:aop="http://www.springframework.org/schema/aop"
	xmlns:batch="http://www.springframework.org/schema/batch"
	xmlns:cache="http://www.springframework.org/schema/cache"
	xmlns:cloud="http://www.springframework.org/schema/cloud"
	xmlns:context="http://www.springframework.org/schema/context"
	xmlns:hadoop="http://www.springframework.org/schema/hadoop"
	xmlns:jdbc="http://www.springframework.org/schema/jdbc"
	xmlns:jms="http://www.springframework.org/schema/jms"
	xmlns:lang="http://www.springframework.org/schema/lang"
	xmlns:mvc="http://www.springframework.org/schema/mvc"
	xmlns:oxm="http://www.springframework.org/schema/oxm"
	xmlns:rabbit="http://www.springframework.org/schema/rabbit"
	xmlns:redis="http://www.springframework.org/schema/redis"
	xmlns:security="http://www.springframework.org/schema/security"
	xmlns:task="http://www.springframework.org/schema/task"
	xmlns:tool="http://www.springframework.org/schema/tool"
	xmlns:tx="http://www.springframework.org/schema/tx"
	xmlns:util="http://www.springframework.org/schema/util"
	xmlns:web-services="http://www.springframework.org/schema/web-services"
	xmlns:webflow-config="http://www.springframework.org/schema/webflow-config"
	xmlns:webflow="http://www.springframework.org/schema/webflow"
	xmlns:websocket="http://www.springframework.org/schema/websocket"
	xsi:schemaLocation="http://www.springframework.org/schema/beans 
			http://www.springframework.org/schema/beans/spring-beans.xsd 
			http://www.springframework.org/schema/aop 
			http://www.springframework.org/schema/aop/spring-aop.xsd 
			http://www.springframework.org/schema/batch
			http://www.springframework.org/schema/batch/spring-batch.xsd
			http://www.springframework.org/schema/cache
			http://www.springframework.org/schema/cache/spring-cache.xsd
			http://www.springframework.org/schema/cloud
			http://www.springframework.org/schema/cloud/spring-cloud.xsd
			http://www.springframework.org/schema/context
			http://www.springframework.org/schema/context/spring-context.xsd
			http://www.springframework.org/schema/hadoop
			http://www.springframework.org/schema/hadoop/spring-hadoop.xsd
			http://www.springframework.org/schema/jdbc
			http://www.springframework.org/schema/jdbc/spring-jdbc.xsd
			http://www.springframework.org/schema/jms
			http://www.springframework.org/schema/jms/spring-jms.xsd
			http://www.springframework.org/schema/lang
			http://www.springframework.org/schema/lang/spring-lang.xsd
			http://www.springframework.org/schema/mvc
			http://www.springframework.org/schema/mvc/spring-mvc.xsd
			http://www.springframework.org/schema/oxm
			http://www.springframework.org/schema/oxm/spring-oxm.xsd
			http://www.springframework.org/schema/rabbit
			http://www.springframework.org/schema/rabbit/spring-rabbit.xsd
			http://www.springframework.org/schema/redis
			http://www.springframework.org/schema/redis/spring-redis.xsd
			http://www.springframework.org/schema/security
			http://www.springframework.org/schema/security/spring-security.xsd
			http://www.springframework.org/schema/task
			http://www.springframework.org/schema/task/spring-task.xsd
			http://www.springframework.org/schema/tool
			http://www.springframework.org/schema/tool/spring-tool.xsd
			http://www.springframework.org/schema/tx
			http://www.springframework.org/schema/tx/spring-tx.xsd
			http://www.springframework.org/schema/util
			http://www.springframework.org/schema/util/spring-util.xsd
			http://www.springframework.org/schema/web-services
			http://www.springframework.org/schema/web-services/web-services.xsd
			http://www.springframework.org/schema/webflow-config
			http://www.springframework.org/schema/webflow-config/spring-webflow-config.xsd
			http://www.springframework.org/schema/webflow
			http://www.springframework.org/schema/webflow/spring-webflow.xsd
			http://www.springframework.org/schema/websocket
			http://www.springframework.org/schema/websocket/spring-websocket.xsd
			">
</beans>
```
</br>

| schema | desc |
| ---- | ---- |
| xmlns="http://www.springframework.org/schema/beans | 声明xml文件默认的命名空间，表示未使用其他命名空间的所有标签的默认命名空间 |
| xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance | 声明XML Schema 实例，声明后就可以使用 schemaLocation 属性|
| xmlns:aop="http://www.springframework.org/schema/aop | 声明前缀为aop的命名空间，后面的URL用于标示命名空间的地址不会被解析器用于查找信息。其惟一的作用是赋予命名空间一个惟一的名称。当命名空间被定义在元素的开始标签中时，所有带有相同前缀的子元素都会与同一个命名空间相关联。|
| xsi:schemaLocation= "http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans-3.0.xsd " | 指定Schema的位置这个属性必须结合命名空间使用。这个属性有两个值，第一个值表示需要使用的命名空间。第二个值表示供命名空间使用的 XML schema 的位置 |

</br>

#### 参考
[1](https://www.cnblogs.com/doit8791/p/5757798.html)  
[2](https://blog.csdn.net/hengyunabc/article/details/22295749)