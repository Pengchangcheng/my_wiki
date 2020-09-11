# SPRING的事务传播特性
| # | 事务注解配置 | 说明 |  
| - | - | - |
|1|	PROPAGATION_REQUIRED|	required:必须的。说明必须要有事物，没有就新建事物，常用选择|
|2|	PROPAGATION_SUPPORTS|	仅仅是支持当前事务，没有事务就非事务方式执行|
|3|	PROPAGATION_MANDATORY|	mandatory:强制的。说明一定要有事务，没有事务就抛出异常|
|4|	PROPAGATION_REQUIRES_NEW|	required_new:必须新建事物。如果当前存在事物就挂起|
|5|	PROPAGATION_NOT_SUPPORTED|	not_supported:不支持事物，如果存在事物就挂起|
|6|	PROPAGATION_NEVER|	never:绝不有事务。如果存在事物就抛出异常|
|7|	PROPAGATION_NESTED|	nested： 嵌套的。支持当前事务，新增Savepoint点，与当前事务同步提交或回滚|

<br>

#### 事务挂起
挂起的事务等待当前事务执行完成，当前事务执行的DB操作不在挂起事务的管理之下，当前事务执行完，挂起的事务继续执行，管理后续的DB操作，提交或回滚
