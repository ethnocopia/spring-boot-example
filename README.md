# code review for spring-boot-example
## functionality
Good:
- A user can add/update/remove/find customer information using their browser
- customer information is persisted to database

Bad:
- error handling and testing (unit/integration) are absent
- validation and security best practices are absent

## readability and maintainability
Good:
- naming convention is consistent and descriptive enough
- indentation and formatting
- code is easy to read

Bad:
- code organization and structure
- use of comments

## structure and design
Good:
- endpoints are RESTful
- dedicated repository layer is present
- model didn't use lombok libraries
- hashCode and equals methods were overridden
- data types are well assigned to model fields
- dependency injection is present
- good approach to customerId generation

Bad:
- business logic and controller logic were done in main class
- there is no way to get 'single' customer 
- logging is not implemented
- all controller methods are voided 

## recommendations
- make the code more maintainable by moving all business and controller logic from
main to their dedicated layers.
- implement unit and integration tests to raise test coverage to at least 80%
- implement error handling, logging, security and validation
- remove commented lines of code