# jdk1.5新特性
### 1. 自动装箱与拆箱
(在没有加入自动装箱和拆箱前，得先将类型转换成int类型才能相加，加入新特性后编译器会自动将类型转换成int让后相加，不需要我们再手动转换类型)

```

Integer iObj = 3;

System.out.println(iObj + 12);

   Integer i1 = 137(-128--127范围时，为true);

   Integer i2 = 137(-128--127范围时，为true);

   System.out.println(i1 == i2); //false，但是括号中时却返回ture，原因是Integer采用的是享元模式

   Integer i3 = Integer.valueOf(213);

   Integer i4 = Integer.valueOf(213);

   System.out.println(i3==i4);//同上，另一种包装形式

```
### 2. 静态导入
> * 非静态导入

```

class Employee {

　　public Double calculateSalary(Double salary{

　　return salary + Increment.INCREMENT * salary;

　} 
}

```
c

```

class Employee {

　　public Double calculateSalary(Double salary{

　　return salary + INCREMENT * salary;

　　	}
　　}

```

### 3.泛型

```

List<Integer> list=new ArrayList<Integer>();

```

### 4.For-Each循环
> * 没有加强前使用for循环

```

void printAll(Collection c) {

　　 for (Iteratori = c.iterator(); i.hasNext(); ) {

　 Employee emp = (Employee)i.next();

　　System.out.println(emp.getName());

　　	}
　　}

```

> * 加强for循环后

```

void printAll(Collection c) {

　　for (Object o : c)

　　System.out.println(o.getName());

　　}

```

### 5.注解
> * 不使用注解

```

public interface EmployeeI extends Java.rmi.Remote	{

　　	public String getName()

　　	throws Java.rmi.RemoteException;

　　	public String getLocation ()

　　	throws Java.rmi.RemoteException;

　　}

```
> * 使用注解


```

public class Employee {

　　@Remote public String getName() { 

　　...

　　}

```

### 6.可变参数（Varargs）

```

    public static void main(String[] args) {
        int[] arr = {1,2,45,6,7};
        /*System.out.println(arr);
            add(arr);*/
        add();
    }
    
    
    public static void add(int... arr){ //长度是0
        
        int result = 0;
        for(int item : arr){
            result+=item;
        }
        System.out.println("总和："+ result);
    }
   

```

### 7.枚举
public class EnumTest {


public static void main(String[] args) {
   WeekDay1 weekDay = WeekDay1.MON;
   System.out.println(weekDay.nextDay());
   WeekDay weekDay2 = WeekDay.FRI;
   System.out.println(weekDay2);
   System.out.println(weekDay2.name());
   System.out.println(weekDay2.ordinal()); 
   System.out.println(WeekDay.valueOf("SUN").toString());
   System.out.println(WeekDay.values().length);
   new Date(300){};
}
public enum WeekDay{
   SUN(1),MON(),TUE,WED,THI,FRI,SAT;
   private WeekDay(){System.out.println("first");}
   private WeekDay(int day){System.out.println("second");}
}


public enum TrafficLamp{
   RED(30){
    public TrafficLamp nextLamp(){
     return GREEN;
    }
   },
   GREEN(45){
    public TrafficLamp nextLamp(){
     return YELLOW;
    }   
   },
   YELLOW(5){
    public TrafficLamp nextLamp(){
     return RED;
    }   
   };
   public abstract TrafficLamp nextLamp();
   private int time;
   private TrafficLamp(int time){this.time = time;}
}
}

# jdk1.6新特性
> * 1.AWT新增加了两个类:Desktop和SystemTray，其中前者用来通过系统默认程序来执行一个操作，如使用默认浏览器浏览指定的URL,用默认邮件客户端给指定的邮箱发邮件,用默认应用程序打开或编辑文件(比如,用记事本打开以txt为后缀名的文件),用系统默认的打印机打印文档等。后者可以用来在系统托盘区创建一个托盘程序

> * 2.使用JAXB2来实现对象与XML之间的映射，可以将一个Java对象转变成为XML格式，反之亦然

> * 3.StAX，一种利用拉模式解析(pull-parsing)XML文档的API。类似于SAX，也基于事件驱动模型。之所以将StAX加入到JAXP家族，是因为JDK6中的JAXB2和JAX-WS 2.0中都会用StAX。

> * 4.使用Compiler API，动态编译Java源文件，如JSP编译引擎就是动态的，所以修改后无需重启服务器。

> * 5.轻量级Http Server API，据此可以构建自己的嵌入式HttpServer,它支持Http和Https协议。

> * 6.插入式注解处理API(PluggableAnnotation Processing API)

> * 7.提供了Console类用以开发控制台程序，位于java.io包中。据此可方便与Windows下的cmd或Linux下的Terminal等交互。

> * 8.对脚本语言的支持如: ruby,groovy, javascript

> * 9.Common Annotations，原是J2EE 5.0规范的一部分，现在把它的一部分放到了J2SE 6.0中

> * 10.嵌入式数据库 Derby

# jdk1.7新特性

> * 1.对Java集合（Collections）的增强支持，可直接采用[]、{}的形式存入对象，采用[]的形式按照索引、键值来获取集合中的对象。如：

```
List<String>list=[“item1”,”item2”];//存

Stringitem=list[0];//直接取

         Set<String>set={“item1”,”item2”,”item3”};//存

         Map<String,Integer> map={“key1”:1,”key2”:2};//存

         Intvalue=map[“key1”];//取
```

> * 2.在Switch中可用String

> * 3.数值可加下划线用作分隔符（编译时自动被忽略）

> * 4.支持二进制数字，如：

```

int binary= 0b1001_1001;

```

> * 5.简化了可变参数方法的调用

> * 6.调用泛型类的构造方法时，可以省去泛型参数，编译器会自动判断。

> * 7.Boolean类型反转，空指针安全,参与位运算

> * 8.char类型的equals方法: booleanCharacter.equalsIgnoreCase(char ch1, char ch2)

> * 9.安全的加减乘除: Math.safeToInt(longv); Math.safeNegate(int v); Math.safeSubtract(long v1, int v2);Math.safeMultiply(int v1, int v2)……

> * 10 .Map集合支持并发请求，注HashTable是线程安全的，Map是非线程安全的。但此处更新使得其也支持并发。另外，Map对象可这样定义：Map map = {name:"xxx",age:18};

# jdk1.8新特性
> * 1.接口的默认方法：即接口中可以声明一个非抽象的方法做为默认的实现，但只能声明一个，且在方法的返回类型前要加上“default”关键字。

> * 2. Lambda 表达式：是对匿名比较器的简化，如：

         Collections.sort(names,(String a, String b) -> {

       returnb.compareTo(a);

});

> *  对于函数体只有一行代码的，你可以去掉大括号{}以及return关键字。如：

         Collections.sort(names,(String a, String b) -> b.compareTo(a));

或：Collections.sort(names, (a, b) -> b.compareTo(a));

> * > * 3. 函数式接口：是指仅仅只包含一个抽象方法的接口，要加@FunctionalInterface注解

> * 4. 使用 :: 关键字来传递方法或者构造函数引用

> * 5.多重注解

```

/***/

```

> * 6.还增加了很多与函数式接口类似的接口以及与Map相关的API等……


# jdk1.9新特性
> * 1. Java 平台级模块系统
> > * Java 9 的定义功能是一套全新的模块系统。当代码库越来越大，创建复杂，盘根错节的“意大利面条式代码”的几率呈指数级的增长。这时候就得面对两个基础的问题: 很难真正地对代码进行封装, 而系统并没有对不同部分（也就是 JAR 文件）之间的依赖关系有个明确的概念。每一个公共类都可以被类路径之下任何其它的公共类所访问到, 这样就会导致无意中使用了并不想被公开访问的 API,模块化的 JAR 文件都包含一个额外的模块描述器。在这个模块描述器中, 对其它模块的依赖是通过 “requires” 来表示的。另外, “exports” 语句控制着哪些包是可以被其它模块访问到的。所有不被导出的包默认都封装在模块的里面。如下是一个模块描述器的示例，存在于 “module-info.java” 文件中:

```

module blog {

  exports com.pluralsight.blog;
 
  requires cms;

}

```

> * 改进的 Javadoc

> * 集合工厂方法
> > * (通常，您希望在代码中创建一个集合（例如，List 或 Set ），并直接用一些元素填充它。 实例化集合，几个 “add” 调用，使得代码重复。 Java 9，添加了几种集合工厂方法：
Set<Integer> ints = Set.of(1, 2, 3);
List<String> strings = List.of("first", "second");
除了更短和更好阅读之外，这些方法也可以避免您选择特定的集合实现。 事实上，从工厂方法返回已放入数个元素的集合实现是高度优化的。这是可能的，因为它们是不可变的：在创建后，继续添加元素到这些集合会导致 “UnsupportedOperationException” 。)

> * 改进的 Stream API
> > * 长期以来，Stream API 都是 Java 标准库最好的改进之一。通过这套 API 可以在集合上建立用于转换的申明管道。在 Java 9 中它会变得更好。Stream 接口中添加了 4 个新的方法：dropWhile, takeWhile, ofNullable。还有个 iterate 方法的新重载方法，可以让你提供一个 Predicate (判断条件)来指定什么时候结束迭代：
IntStream.iterate(1, i -> i < 100, i -> i + 1).forEach(System.out::println);
第二个参数是一个 Lambda，它会在当前 IntStream 中的元素到达 100 的时候返回 true。因此这个简单的示例是向控制台打印 1 到 99。
除了对 Stream 本身的扩展，Optional 和 Stream 之间的结合也得到了改进。现在可以通过 Optional 的新方法 `stram` 将一个 Optional 对象转换为一个(可能是空的) Stream 对象：

> * 私有接口方法

> > * Java 8 为我们带来了接口的默认方法。 接口现在也可以包含行为，而不仅仅是方法签名。 但是，如果在接口上有几个默认方法，代码几乎相同，会发生什么情况？ 通常，您将重构这些方法，调用一个可复用的私有方法。 但默认方法不能是私有的。 将复用代码创建为一个默认方法不是一个解决方案，因为该辅助方法会成为公共API的一部分。 使用 Java 9，您可以向接口添加私有辅助方法来解决此问题：
public interface MyInterface {
 
    void normalInterfaceMethod();
 
    default void interfaceMethodWithDefault() {  init(); }
 
    default void anotherDefaultMethod() { init(); }
 
    // This method is not part of the public API exposed by MyInterface
    private void init() { System.out.println("Initializing"); }
}