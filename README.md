# Unexpected Behavior When Directly Modifying Instance Variables in Ruby

This repository demonstrates a potential bug in Ruby code related to directly modifying instance variables using `instance_variable_set`.  Direct manipulation of instance variables can bypass encapsulation and lead to unexpected results, especially in larger, more complex applications.

The `bug.rb` file shows an example of this issue. The `bugSolution.rb` demonstrates how to use methods to update instance variables and maintain better code structure and maintainability. 

**Problem:** Modifying instance variables directly breaks the principle of encapsulation, making the code harder to maintain and debug. It can also create inconsistencies if other parts of the code rely on methods to update the state of the object.

**Solution:** The recommended approach is to always update instance variables through methods. This allows you to implement validation, maintain consistency, and control access to your object's internal state.