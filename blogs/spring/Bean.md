---
title: spring中的Bean
date: 2022-1-21
---
## Bean与BeanDefinition的区别

>   Bean的本质是java对象，只是这个对象的生命周期由spring管理
>   BeanDefinition--Bean的定义，根据配置，生成用来描述Bean的BeanDefinition,常用属性

- 作用范围scope(@Scope)
- 懒加载lazy-init(@Lazy):决定Bean的实力是否延迟加载
- 首选primary(@primary):设置为true的bean会是优先的实现类
- factory-bean和factory-method(@configration和@Bean)

## BeanFactory和Application的区别

>   BeanFactory相当于发动机,Application相当于汽车

## 初始化容器主要做的事情

- 将配置信息读取到内存中;
- 内存中会将一个个配置文件当成Resource对象;
- Resource对象解析成BeanDefinition实力;
- 注册到Spring容器中;

## 术语

### 主键扫描

> 自动发现容器中需要扫瞄的bean

### 自动装配

> 自动满足bean之间的依赖（anturire注解）

## ApplicationContext与BeanFactory

> BeanFactory相当于发动机,application相当于汽车

## refresh()方法：可以看作成IOC容器的启动操作

- 容器初始化、配置解析

- BeanfactoryPostProcessor和BeanPostProcessor的注册和激活

- 国际化配置

## BeanDefinitonReader(利器的使用者)

### 读取BeanDefiniton

- 将配置信息解析成一个个BeanDefinition
- BeanDefinitionRegistry(注册器)将BeanDefiniton注册到容器中

### Document

​	将xml配置文件解析成Document对象

## BeanDefinitionReader学习过程中的关键字

- location

- BeanDefinitionReader

- Resource

- BeanDefinitonRegistry

- Resourceloader

- DefaultListableBeanFactory







