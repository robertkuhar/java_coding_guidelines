# java_coding_guidelines

Repo supporting the WingDing Winter 2017 iteration covering "JavaTM Coding 
Guidelines:  75 Recommendations for Reliable and Secure Programs" by Fred Long,
Dhruv Mohindra, Robert C. Seacord, Dean F. Sutherland, David Svoboda

https://www.cert.org/secure-coding/publications/books/java-coding-guidelines.cfm

## Build

    ./gradlew

# Tentative Schedule

| Date    | Chapter | Pages | Moderator |
|---------|---------|-------|-----------|
|Jan 25   |CH01:  Security, Guidelines 1 through 9|30|Bob|
|Feb 8    |CH01:  Security, Guidelines 9 through 21|52|Stuart M|
|Feb 22   |CH02:  Defensive Programming, Guidelines 22 through 28|27|Eric|
|Mar 8    |CH02:  Defensive Programming, Guidelines 29 through 36|23|Doug|
|Mar 22   |CH03:  Reliability, Guidelines 37 through 49|33|Jeff Braun|
|April 12 |CH04:  Program Understandability, Guidelines 50 through 65|42|Daniel Kirkdorffer|
|April 26 |CH05:  Programmer Misconceptions, Guidelines 66 through 75|36|Linus|
|May 10   |?|?|?|
|May 24   |?|?|?|
|June 14  |Summer Break|

# Guideline Index
| Guideline                   | Chapter | Date |
|-----------------------------|---------|---------|
|  1. Limit the lifetime of sensitive data | CH01:  Security | Jan 25 |
|  2. Do not store unencrypted sensitive information on the client side | CH01:  Security | Jan 25 |
|  3. Provide sensitive mutable classes with unmodifiable wrappers | CH01:  Security | Jan 25 |
|  4. Ensure that security-sensitive methods are called with validated arguments | CH01:  Security | Jan 25 |
|  5. Prevent arbitrary file upload | CH01:  Security | Jan 25 |
|  6. Properly encode or escape output | CH01:  Security | Jan 25 |
|  7. Prevent code injection | CH01:  Security | Jan 25 |
|  8. Prevent XPath injection | CH01:  Security | Jan 25 |
|  9. Prevent LDAP injection | CH01:  Security | Jan 25 |
| 10. Do not use the clone() method to copy untrusted method parameters | CH01:  Security | Feb 8 |
| 11. Do not use Object.equals() to compare cryptographic keys | CH01:  Security | Feb 8 |
| 12. Do not use insecure or weak cryptographic algorithms | CH01:  Security | Feb 8 |
| 13. Store passwords using a hash function | CH01:  Security | Feb 8 |
| 14. Ensure that SecureRandom is properly seeded | CH01:  Security | Feb 8 |
| 15. Do not rely on methods that can be overridden by untrusted code | CH01:  Security | Feb 8 |
| 16. Avoid granting excess privileges | CH01:  Security | Feb 8 |
| 17. Minimize privileged code | CH01:  Security | Feb 8 |
| 18. Do not expose methods that use reduced-security checks to untrusted code | CH01:  Security | Feb 8 |
| 19. Define custom security permissions for fine-grained security | CH01:  Security | Feb 8 |
| 20. Create a secure sandbox using a security manager | CH01:  Security | Feb 8 |
| 21. Do not let untrusted code misuse privileges of callback methods | CH01:  Security | Feb 8 |
| 22. Minimize the scope of variables | CH02:  Defensive Programming | Feb 22 |
| 23. Minimize the scope of the @SuppressWarnings annotation | CH02:  Defensive Programming | Feb 22 |
| 24. Minimize the accessibility of classes and their members | CH02:  Defensive Programming | Feb 22 |
| 25. Document thread-safety and use annotations where applicable | CH02:  Defensive Programming | Feb 22 |
| 26. Always provide feedback about the resulting value of a method | CH02:  Defensive Programming | Feb 22 |
| 27. Identify files using multiple file attributes | CH02:  Defensive Programming | Feb 22 |
| 28. Do not attach significance to the ordinal associated with an enum | CH02:  Defensive Programming | Feb 22 |
| 29. Be aware of numeric promotion behavior | CH02:  Defensive Programming | Mar 8 |
| 30. Enable compile-time type checking of variable arity parameter types | CH02:  Defensive Programming | Mar 8 |
| 31. Do not apply public final to constants whose value might change in later releases | CH02:  Defensive Programming | Mar 8 |
| 32. Avoid cyclic dependencies between packages | CH02:  Defensive Programming | Mar 8 |
| 33. Prefer user-defined exceptions over more general exception types | CH02:  Defensive Programming | Mar 8 |
| 34. Try to gracefully recover from system errors | CH02:  Defensive Programming | Mar 8 |
| 35. Carefully design interfaces before releasing them | CH02:  Defensive Programming | Mar 8 |
| 36. Write garbage collection–friendly code | CH02:  Defensive Programming | Mar 8 |
| 37. Do not shadow or obscure identifiers in subscopes | CH03:  Reliability | Mar 22 |
| 38. Do not declare more than one variable per declaration | CH03:  Reliability | Mar 22 |
| 39. Use meaningful symbolic constants to represent literal values in program logic| CH03:  Reliability | Mar 22 |
| 40. Properly encode relationships in constant definitions | CH03:  Reliability | Mar 22 |
| 41. Return an empty array or collection instead of a null value for methods that return an array or collection| CH03:  Reliability | Mar 22 |
| 42. Use exceptions only for exceptional conditions| CH03:  Reliability | Mar 22 |
| 43. Use a try-with-resources statement to safely handle closeable resources| CH03:  Reliability | Mar 22 |
| 44. Do not use assertions to verify the absence of runtime errors| CH03:  Reliability | Mar 22 |
| 45. Use the same type for the second and third operands in conditional expressions| CH03:  Reliability | Mar 22 |
| 46. Do not serialize direct handles to system resources | CH03:  Reliability | Mar 22 |
| 47. Prefer using iterators over enumerations | CH03:  Reliability | Mar 22 |
| 48. Do not use direct buffers for short-lived, infrequently used objects | CH03:  Reliability | Mar 22 |
| 49. Remove short-lived objects from long-lived container objects | CH03:  Reliability | Mar 22 |
| 50. Be careful using visually misleading identifiers and literals | CH04:  Program Understandability | April 12 |
| 51. Avoid ambiguous overloading of variable arity methods | CH04:  Program Understandability | April 12 |
| 52. Avoid in-band error indicators | CH04:  Program Understandability | April 12 |
| 53. Do not perform assignments in conditional expressions | CH04:  Program Understandability | April 12 |
| 54. Use braces for the body of an if, for, or while statement | CH04:  Program Understandability | April 12 |
| 55. Do not place a semicolon immediately following an if, for, or while condition | CH04:  Program Understandability | April 12 |
| 56. Finish every set of statements associated with a case label with a break statement | CH04:  Program Understandability | April 12 |
| 57. Avoid inadvertent wrapping of loop counters | CH04:  Program Understandability | April 12 |
| 58. Use parentheses for precedence of operation | CH04:  Program Understandability | April 12 |
| 59. Do not make assumptions about file creation | CH04:  Program Understandability | April 12 |
| 60. Convert integers to floating-point for floating-point operations | CH04:  Program Understandability | April 12 |
| 61. Ensure that the clone() method calls super.clone() | CH04:  Program Understandability | April 12 |
| 62. Use comments consistently and in a readable fashion | CH04:  Program Understandability | April 12 |
| 63. Detect and remove superfluous code and values | CH04:  Program Understandability | April 12 |
| 64. Strive for logical completeness  | CH04:  Program Understandability | April 12 |
| 65. Avoid ambiguous or confusing uses of overloading | CH04:  Program Understandability | April 12 |
| 66. Do not assume that declaring a reference volatile guarantees safe publication of the members of the referenced object | CH05:  Programmer Misconceptions | April 26 |
| 67. Do not assume that the sleep(), yield(), or getState() methods provide synchronization semantics | CH05:  Programmer Misconceptions | April 26 |
| 68. Do not assume that the remainder operator always returns a nonnegative result for integral operands | CH05:  Programmer Misconceptions | April 26 |
| 69. Do not confuse abstract object equality with reference equality | CH05:  Programmer Misconceptions | April 26 |
| 70. Understand the differences between bitwise and logical operators | CH05:  Programmer Misconceptions | April 26 |
| 71. Understand how escape characters are interpreted when strings are loaded | CH05:  Programmer Misconceptions | April 26 |
| 72. Do not use overloaded methods to differentiate between runtime types | CH05:  Programmer Misconceptions | April 26 |
| 73. Never confuse the immutability of a reference with that of the referenced object | CH05:  Programmer Misconceptions | April 26 |
| 74. Use the serialization methods writeUnshared() and readUnshared() with care | CH05:  Programmer Misconceptions | April 26 |
| 75. Do not attempt to help the garbage collector by setting local reference variables to null | CH05:  Programmer Misconceptions | April 26 |

