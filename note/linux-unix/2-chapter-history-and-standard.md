## 第2章 基本概念

#### 2.1 操作系统的核心-内核

##### 内核的职责

* 进程调度

	抢占式多任务系统

* 内存管理

	1. 进程与进程之间，进程与内核之间彼此隔离，因此一个进程无法读取或修改内核或其他进程的内存内容。

	2. 只需要将进程的一部分保持在内存中，可以加载更多进程。


* 提供文件系统

* 创建和终止进程

* 对设备的访问

* 联网

* 提供系统调用应用编程接口

##### 内核态和用户态

所拥有的权限不一样，内核态可以管理内存和其他进程，用户态只能拥有本身进程中资源。

#### 2.9 静态库和共享库

* 静态库

	每个可执行文件链接过程中加载所有需要的模块，这是重复的。

* 共享库

    通过动态链接器在运行时加载，存储在内存中，只需要加载一次。


#### 2.19 /proc文件系统

可用于用户可读方式配置系统配置。