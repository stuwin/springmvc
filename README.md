# springmvc
整理笔记本翻几四年前学习springmvc的代码，存起来留个纪念
 
- [springmvc](/springmvc)
  基本概念和使用方法，涉及概念介绍、环境搭建、编程细节、运行调试
  套笔记整体偏入门和应用，适合快速上手，对底层实现和机理并未做过多分析。
-----
## 目录
  - [springmvc](/springmvc)
  
    - 框架原理和入门配置
    - 非注解的处理器映射器和适配器
    - 注解的处理器映射器和适配器
    - 前端控制器
    - 入门程序小结
    - springmvc整合mybatis(IDEA中通过maven构建)
    - springmvc整合mybatis之mapper
    - springmvc整合mybatis之service
    - springmvc整合mybatis之controller
    - springmvc注解开发之商品修改功能
    - springmvc注解开发之简单参数绑定
    - springmvc注解开发之包装类型参数绑定
    - springmvc注解开发之集合类型参数绑定
    - springmvc校验
    - 数据回显
    - 异常处理器
    - 上传图片
    - json数据交互.
    - RESTful支持
    - 拦截器
    - springmvc整合mybatis遇到的问题及解决小结
    - springmvc开发小结
-----
环境准备:
- jdk 1.8+
- intellij IDEA 15.0.2+
- mysql 5.1+
- maven 3.3+
- tomcat 8+


数据库导入:

- 新建一个数据库,项目中默认的数据库名为 `mybatis001`
- 导入 [sourcecode/sql](/sourcecode/sql) 中的 [create.sql](/sourcecode/sql/create.sql) 创建数据表
- 导入 [sourcecode/sql](/sourcecode/sql) 中的 [data.sql](/sourcecode/sql/data.sql) 添加测试数据


在IDE中添加 tomcat 容器:

- ToolBar -> 运行按钮旁边的下拉 -> "Edit Configurations" -> "+" -> "Tomcat Server" 选 local
- 如果是第一次添加,还需要配置 tomcat 的路径

源码导入:

- 将 sourcecode 中的任意子文件夹拷贝出来作为项目根目录,打开即可
- 每个子文件夹的项目请参考 [sourcecode 说明](#sourcecode说明)

-----

## sourcecode 说明

该文件夹下是涉及到的源码，其中 mybatis 部分都是直接新建的 web 工程，springmvc 部分都是使用 maven 构建的。

我使用的 IDE 是 intellij IDEA 15.0.2,以下每个子文件夹对应一个 project。

- [mybatis](/sourcecode/mybatis):mybatis 部分前 16 篇笔记用到的源码
- [mybatis-spring](/sourcecode/mybatis-spring):mybatis 部分笔记(17)对应的源码
- [mybatis-generator](/sourcecode/mybatis-generator):逆向工程的源码
- [springmvcfirst](/sourcecode/springmvcfirst):springmvc 部分前两篇笔记对应的非注解方式配置的源码
- [springmvcsecond](/sourcecode/springmvcsecond):springmvc 部分前几篇笔记对应的注解方式配置的源码
- [**learnssm-firstssm**](/sourcecode/learnssm-firstssm):**核心代码**,springmvc 和 mybatis 整合部分的笔记几乎所有的源码

-----
