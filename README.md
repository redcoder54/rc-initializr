[Spring Initializr](https://github.com/spring-io/initializr) 是一个基于Web的工具，可快速创建SpringBoot项目。一些流行的IDE，比如Intellij IDEA，已经集成了Spring Initializr，帮助我们快速创建一个SpirngBoot项目。

官方提供的Spring Initializr生成的SpringBoot项目十分简单，如下所示：

![](https://media.geeksforgeeks.org/wp-content/uploads/20210604131533/Screenshot20210604at11426PM-483x660.png)

我们在日常开发中，经常需要创建各种项目，而这些项目之间，可能存在大量相同，甚至类似的代码，比如Redis配置类、Quartz配置类、一些常用的工具类等等。为了在创建新的项目时，一并生成这些可重复使用的代码，rc-initializr诞生了，它是基于Spring Initializr定制的项目生成器。

下面以Intellij IDEA为例，演示如何使用rc-initializr创建项目：

(1)  打开Intellij IDEA，进入New Project界面

![step1.png](https://s2.loli.net/2023/02/17/MIJOx8D74CicuGP.png)

修改Service Url为：http://localhost:8080 (本地启动的服务地址，根据实际情况填写)

输入项目信息后，点击Next

(2) 选择SpringBoot版本和依赖

![step2.png](https://s2.loli.net/2023/07/30/EOBqJR3scH8do6y.png)

默认添加的依赖：spring-web, spring-data-redis, jedis, quartz, validation, apache-commons-pool, apache-commons-lang3, commons-collections, lombok, spring-data-jpa.

(3) 点击Finish，项目创建成功，目录结构如下

![step3.png](https://s2.loli.net/2023/07/30/aPyWQUC6wlOYrGN.png)

至此，项目创建完成，包含了我们常用的配置代码、工具类和一些依赖等。
