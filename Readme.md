# IBO (Ebo Mart Private Limited)

<div align="center">
---
---

### You have been given a list of products which is having property productName, quantity and description.

##### PROBLEM STATEMENTS:

###### 1. 1. you need to write a function say, getUniqueProductCount which should return count of each Product(as an object) present in the given list of Products considering Product Name as Key.?

###### Sample Output for the given listOfProducts will be :

```javascript
{
  "TV": 2,
  "AC": 2,
  "FAN": 1
}

```

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

Within the function, we first declare the `name` variable with the `var` keyword. This means that the variable gets hoisted (memory space is set up during the creation phase) with the default value of `undefined`, until we actually get to the line where we define the variable. We haven't defined the variable yet on the line where we try to log the `name` variable, so it still holds the value of `undefined`.

Variables with the `let` keyword (and `const`) are hoisted, but unlike `var`, don't get <i>initialized</i>. They are not accessible before the line we declare (initialize) them. This is called the "temporal dead zone". When we try to access the variables before they are declared, JavaScript throws a `ReferenceError`.

</p>
</details>

---
</div>