---
layout: post
title:  "Great learning c++ article for Java developers"
date:   2017-05-25
categories: markdown
---
### [Moving from Java to C++][link]
- C++ object variables represents the values
 - Point a = b; // copies b to a
- Method can pass in arguments by reference: `int& a`
  - reference represents the physical location of the variable
  - use dot to call functions of a object variable
- Pointer is a kind of a variable used to point to an address of another object
  - `Employee* p = new Employee("alec", 29);`
  - `Employee* s = &boss;`
  - Use `->` to call functions for a pointer variable
    - `(*p).getSalary()` is the same with `p->getSalary()`

[link]: http://www.horstmann.com/ccj2/ccjapp3.html
