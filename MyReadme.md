# Spring5webapp

This material was generated from 
[Spring Framework 5: Beginner to Guru](http://www.udemy.com/course/spring-framework-5-beginner-to-guru) 
Course.

## Introduction

1. To execute: 

```
./mvnw spring-boot:run
```

2. Go to branch starter-jpa-entities

2.1 See [UsingJPAEntities.pptx](docs/ppts/UsingJPAEntities.pptx)

2.2 Tasks:

- Put the ```@Entity``` annotation on both ```Author``` and ```Book``` classes
- Add the unique identifiers for both classes (Long id, getter and setter)
- Add the ```@Id``` and ```@GeneratedValue(strategy = GenerationType.AUTO)``` (MYSQL) for both ```Author``` and 
```Book``` classes
- In the ```Author``` class, map ```books``` with the annotation ```@manyToMany(mappedBy = "authors")```
- In the ```Book``` class, map ```authors``` with the annotation ```@manyToMany``` and ```@JoinTable(name="author_book", joinColumns = @JoinColumn(name = "book_id"), inverseJoinColumns = @JoinColumn(name = "author_id"))```
- Enable H2 database. Go to ```application.properties``` and:

```
spring.h2.console.enabled=true
```

Now you can: ```localhost:8080/h2-console``` 