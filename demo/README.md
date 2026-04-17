# Spring Boot Demo Application

这是一个使用 Spring Boot 搭建的简单示例项目。

## 技术栈

- Java 17
- Spring Boot 3.2.5
- Maven
- Spring Web

## 项目结构

```
demo/
├── src/
│   ├── main/
│   │   └── java/com/example/
│   │       └── DemoApplication.java
│   └── test/
│       └── java/com/example/
│           └── DemoApplicationTests.java
├── pom.xml
└── README.md
```

## 快速开始

### 前置条件

- JDK 17 或更高版本
- Maven 3.6+

### 构建项目

```bash
cd demo
mvn clean package
```

### 运行应用

```bash
mvn spring-boot:run
```

或者运行打包后的 jar 文件：

```bash
java -jar target/demo-1.0-SNAPSHOT.jar
```

### 访问接口

应用启动后，访问以下端点：

- http://localhost:8080/ - 返回 "Hello, Spring Boot!"
- http://localhost:8080/api/greeting - 返回 "Welcome to Spring Boot Application!"

## 运行测试

```bash
mvn test
```

## 功能说明

本项目包含以下功能：

1. **Spring Boot 自动配置** - 使用 `@SpringBootApplication` 注解
2. **RESTful API** - 提供两个简单的 GET 接口
3. **单元测试** - 包含基本的上下文加载测试

## 自定义

你可以根据需要修改 `DemoApplication.java` 来添加更多功能：

- 添加数据库支持（spring-boot-starter-data-jpa）
- 添加安全认证（spring-boot-starter-security）
- 添加更多 REST 接口

## 许可证

MIT License
