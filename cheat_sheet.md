# Java Interview Cheat Sheet

## Java Core
* StringBuffer - thread-safe, StringBuilder - not thread safe
* hashCode/equals methods of Object are goes in pair
* Exceptions
```
Object
    |
Throwable(CHECKED)
    |               \
Error(UNCHECKED)    Exception(CHECKED)
                      |                  \
            RuntimeException(UNCHECKED)   ...
```
* Java only supports pass by value. With objects, the object reference itself is passed by value and so both the original reference and parameter copy both refer to the same object.

## Java 8
* Stream API: map, filter, collect, count, limit
* Optional
* Lambda
* default method
* method reference
* static method in interface
* Improved date/time API

## Spring Framework
* Modules:
	* The Core container module
	* Application context module
	* AOP module (Aspect Oriented Programming)
	* JDBC abstraction and DAO module
	* O/R mapping integration module (Object/Relational)
	* Web module
	* MVC framework module
* Scopes:
	* singleton (single instance per Spring IoC container)
	* prototype (any number of object instances)
	* request (defined to an HTTP request, this scope is valid only in a web-aware Spring ApplicationContext)
	* session (scoped to an HTTP session, this scope is also valid only in a web-aware Spring ApplicationContext)
	* global-session (definition is scoped to a global HTTP session, this is also a case used in a web-aware Spring ApplicationContext)
* Autowiring:
	* no (default)
	* byName
	* byType
	* constructor
* Transactions		
	* Programmatic Transaction Management (should be used for few transaction operations)
	* Declarative Transaction Management (should be used for many transaction operations)

## Databases
### SQL
Joins:
* Inner Join
* Left Outer Join / Right Outer Join
* Full Outer Join
* Cross join
* Self Join
