# Dependencies
1. Spring Web
2. Spring Data JPA
3. Thymeleaf
4. H2

# Domain/Model Layer : User

- single class which will be responsible for modeling "User" entities

# Adding Validation Annotations
The basics of validating a Java bean with the standard framework – JSR 380, also known as Bean Validation 2.0.

-Add following dependencies manually:
1. Validation-API
<dependency>
    <groupId>javax.validation</groupId>
    <artifactId>validation-api</artifactId>
    <version>2.0.0.Final</version>
</dependency>

2. Validation API Reference Implementation
<dependency>
    <groupId>org.hibernate.validator</groupId>
    <artifactId>hibernate-validator</artifactId>
    <version>6.0.2.Final</version>
</dependency>
<dependency>
    <groupId>org.hibernate.validator</groupId>
    <artifactId>hibernate-validator-annotation-processor</artifactId>
    <version>6.0.2.Final</version>
</dependency>

3. Expression Language Dependencies
<dependency>
    <groupId>javax.el</groupId>
    <artifactId>javax.el-api</artifactId>
    <version>3.0.0</version>
</dependency>
<dependency>
    <groupId>org.glassfish.web</groupId>
    <artifactId>javax.el</artifactId>
    <version>2.2.6</version>
</dependency>

- import using the "javax.validation.constraints."

# Repository Layer
1. Create UserRespository.java in main (make as interface not class!)
2. extend CrudRepository to UserRepository interface
