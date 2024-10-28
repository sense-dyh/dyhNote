# dyhNote
在 Spring Boot 应用程序中，当你使用 -Dspring.profiles.active=sit 参数启动应用时，Spring 会优先加载对应环境的配置文件（在这种情况下是 application-sit.yml）。不过，application.yml 文件仍然会被加载，因为它被视为默认的基础配置文件。

具体来说，Spring Boot 的配置加载过程大致如下：

基础配置文件：总是会加载 application.properties 或 application.yml 文件的内容，即使指定了环境配置文件也是如此。这是为了提供一个通用的基本配置集。
环境特定配置文件：如果指定了环境（如通过 -Dspring.profiles.active=sit），则会加载与该环境相关的配置文件（即 application-sit.yml）。这些配置文件中的属性会覆盖基础配置文件中的同名属性。
因此，在你的例子中，application.yml 和 application-sit.yml 都会被加载。application-sit.yml 中的配置会覆盖 application.yml 中相同名称的配置项。这样做的好处是可以保持基本配置的一致性，同时允许每个环境有不同的定制化配置。
