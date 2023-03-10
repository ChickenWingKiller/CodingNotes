# 核心容器
- IoC(Inversion of Control)控制反转
  - 使用对象时，由主动new产生对象转换为由外部提供对象，此过程中对象创建控制权由程序转移到外部。
- Spring技术对IoC思想进行了实现
  - Spring提供了一个容器，成为IoC容器，用来充当IoC思想中的外部。
  - IoC容器负责对象的创建、初始化等一系列工作，被创建或被管理的对象在IoC容器中统称为Bean。
- DI(Dependency Injection)依赖注入
  - 在容器中建立bean与bean之间的依赖关系的整个过程，称为依赖注入。
  - 依赖注入方式
    - setter注入
      - 简单类型
      - 引用类型
    - 构造器注入
      - 简单类型
      - 引用类型
  - 依赖自动装配
    - IoC容器根据bean所依赖的资源在容器中自动查找并注入到bean中的过程成为自动装配
    - 自动装配方式
      - 按类型（常用）
      - 按名称
      - 按构造方法
      - 不启动自动装配
    - 依赖自动装配特征
      - 自动装配用于引用类型依赖注入，不能对简单类型进行操作
      - 使用按类型装配时（byType）必须保障容器中相同类型的bean唯一，推荐使用
      - 使用按名称装配时（byName）必须保障容器中具有指定名称的bean，因变量名与配置耦合，不推荐使用
      - 自动装配优先级低于setter注入与构造器注入，同时出现时自动装配配置失效
  - 加载properties文件
    - 开启context命名空间
    - 使用context命名空间，加载指定properties文件
    - 使用${}读取加载的属性值
- 容器
- 注解开发
---
# 整合（整合数据层技术MyBatis）
---
# AOp
---
# 事务处理
