
    1.安全
        1.编写代码
            1.代码签名 ....其他。。。
            2.类加载 字节码校验   双亲委派机制及自定义加载器实现     https://www.cnblogs.com/wxd0108/p/6681618.html
        2.用户认证  加密
        3.数字签名

            |
         用户登陆



-------------代码编写-----------编写安全可靠程序的75条建议-----https://yq.aliyun.com/articles/92618----------------------------
安全 确保Java应用程序安全性的编码建议

[建议1：限制敏感数据的生命周期](https://yq.aliyun.com/articles/92416)

[建议2：不要在客户端存储未经加密的敏感数据](https://yq.aliyun.com/articles/92419)

[建议3：为敏感可变类提供不可修改的包装器](https://yq.aliyun.com/articles/92425)

[建议4：确保安全敏感方法被调用时参数经过验证](https://yq.aliyun.com/articles/92432)

[建议5：防止任意文件上传](https://yq.aliyun.com/articles/92461)

[建议6：正确地编码或转义输出](https://yq.aliyun.com/articles/92469)

[建议7：防止代码注入](https://yq.aliyun.com/articles/92495)

[建议8：防止XPath注入](https://yq.aliyun.com/articles/92498)

[建议9：防止LDAP注入](https://yq.aliyun.com/articles/)

[建议10：不要使用clone()方法来复制不可信的方法参数}(https://yq.aliyun.com/articles/92509)

[建议11：不要使用Object.equals()来比较密钥[(https://yq.aliyun.com/articles/92518)

[建议12：不要使用不安全的弱加密算法](https://yq.aliyun.com/articles/92521)

[建议13：使用散列函数存储密码](https://yq.aliyun.com/articles/92526)

[建议14：确保SecureRandom正确地选择随机数种子](https://yq.aliyun.com/articles/92530)

[建议15：不要依赖可以被不可信代码覆盖的方法](https://yq.aliyun.com/articles/92535)

[建议16：避免授予过多特权](https://yq.aliyun.com/articles/92539)

[建议17：最小化特权代码](https://yq.aliyun.com/articles/92545)

[建议18：不要将使用降低安全性检查的方法暴露给不可信代码](https://yq.aliyun.com/articles/92561)

[建议19：对细粒度的安全定义自定义安全权限](https://yq.aliyun.com/articles/92565)

[建议20：使用安全管理器创建一个安全的沙盒](https://yq.aliyun.com/articles/92584)

[建议21：不要让不可信代码误用回调方法的特权](https://yq.aliyun.com/articles/92596)

防御式编程 通过这些建议，程序员可以编写出防御性的程序
建议22：最小化变量的作用域

建议23：最小化@SuppressWarnings注解的作用域

建议24：最小化类及其成员的可访问性

建议25：文档化代码的线程安全性

建议26：为方法的结果值提供反馈

建议27：使用多个文件属性识别文件

建议28：不要赋予枚举常量的序号任何特殊意义

建议29：注意数字提升行为

建议30：对可变参数的类型做编译时类型检查

建议31：不要把其值在以后版本里可能会发生变化的常量设置为public final

建议32：避免包之间的循环依赖

建议33：使用用户自定义的异常而非宽泛的异常类型

建议34：尽量从系统错误中优雅恢复

建议35：发布接口前请谨慎设计

建议36：编写对垃圾收集机制友好的代码

可靠性 提高Java应用程序可靠性和安全性的建议
建议37：不要在子作用域里遮蔽或者掩盖标识符

建议38：不要在一个声明里声明多个变量

建议39：在程序逻辑中用有意义的符号常量代表文字值

建议40：在常量定义中恰当地表示相互之间的关系

建议41：对于返回数组或者集合的方法，用返回一个空数组或者集合来替代返回一个空值

建议42：只在异常的情况下使用异常

建议43：使用try-with-resources语句安全处理可关闭的资源

建议44：不要使用断言来验证不存在的运行时错误

建议45：在条件表达式中，第二个和第三个操作数应使用相同类型

建议46：不要序列化直接指向系统资源的句柄

建议47：更倾向于使用迭代器而不是列举

建议48：对于短生存周期、不常用的对象不要使用直接缓冲区

建议49：从长生存周期容器对象中移除短生存周期对象

程序的可理解性 给出了让程序更易读易懂的建议
建议50：谨慎使用视觉上有误导性的标识符和文字

建议51：避免歧义重载变参方法

建议52：要避免使用带内错误指示器

建议53：不要在条件表达式中进行赋值

建议54：请使用大括号把if、for或while代码体括起来

建议55：不要直接在if、for或while条件语句后面加分号

建议56：在每一个case分支的代码块中加上break语句

建议57：避免不当的计算循环计数器

建议58：使用括号表示操作的优先级

建议59：不要对文件的创建做任何假设建议60：做浮点运算前把整数转换为浮点数

建议61：确保对象的clone()方法中有调用super.clone()

建议62：保持注释的一致性和可读性

建议63：检测并移除冗余的代码和值 199

建议64：尽量保证逻辑完备 203

建议65：避免有歧义的重载或者误导性的重载 206

程序员的常见误解 展示一些Java语言和编程概念经常被误解的情形
建议66：不要假设使用volatile关键字声明引用可以保证引用所指对象的安全发布

建议67：不要假设sleep()、yield()或getState()方法提供了同步语义

建议68：不要假设对整数做取余运算总是返回正整数

建议69：不要弄混抽象对象的相等性和引用的相等性

建议70：理解按位运算符和逻辑运算符之间的差异

建议71：理解加载字符串时如何做特殊字符转义

建议72：不要使用重载的方法来区分运行时类型

建议73：不要弄混引用的不可变性和对象的不可变性

建议74：谨慎使用序列化方法writeUnshared()和readUnshared()

建议75：不要试图通过把本地引用变量设置为null来帮助垃圾收集器

这75条建议出自《Java编码指南》











---------------------------------------------------------
