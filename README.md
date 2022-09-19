Filters

1 - Authorize Filter
2 - Resource Filter
3 - Action Filter
4 - Exception Filter
5 - Result Filter

** Async Await Operation
https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/#start-tasks-concurrently

** C# Reflection

** Sealed 
** Abstract
- An abstract class cannot be instantiated.
- An abstract class may contain abstract methods and accessors.
- It is not possible to modify an abstract class with the sealed modifier because the two modifiers have opposite meanings. The sealed modifier prevents a class from
being inherited and the abstract modifier requires a class to be inherited.
- A non-abstract class derived from an abstract class must include actual implementations of all inherited abstract methods and accessors.

** Abstract Method
- An abstract method is implicitly a virtual method.
- Abstract method declarations are only permitted in abstract classes.
Because an abstract method declaration provides no actual implementation, there is no method body; the method declaration simply ends with a semicolon and there are no curly braces ({ }) following the signature. 
For example:
public abstract void MyMethod();  
- The implementation is provided by a method override, which is a member of a non-abstract class.
- It is an error to use the static or virtual modifiers in an abstract method declaration.
- It is an error to use the abstract modifier on a static property.

** Override
** Virtual 
** Static


# The Repository pattern
- Repositories are classes or components that encapsulate the logic required to access data sources.
- They centralize common data access functionality, providing better maintainability and decoupling technology used to access the domain model layer 
- repository is nothing but a class definecd for that entity containing all possible operationson that specific entity
- For example, a repository for an entity Customer, will have basic CRUD operations and any other possible operations related to it.
# Unit of Work
- it's refered to as single transaction containing multiple operations (CRUD)
-  it means that for a specific user action (say registration on a website), all the transactions like insert/update/delete and so on \
are done in one single transaction, rather then doing multiple database transactions. 

# Data Access Object (DAO)
Class that usually has operations to save, update, delete
# Data Transfer Object (DTO).
It usually just holds the data
# Pagination:
