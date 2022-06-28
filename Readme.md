# IBO (Ebo Mart Private Limited)

<div>
---
---

### You have been given a list of products which is having property productName, quantity and description.

##### PROBLEM STATEMENTS:

### 1. you need to write a function say, getUniqueProductCount which should return count of each Product(as an object) present in the given list of Products considering Product Name as Key.?

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

#### Answer:

```javascript
let obj = {};

for(let i=0; i<listOfProducts.length;i++){
    obj[listOfProducts[i].productName]?obj[listOfProducts[i].productName] +=1: obj[listOfProducts[i].productName] = 1;
}

console.log(obj)


```
###### output:

```javascript
{
  AC: 2,
  FAN: 1,
  TV: 2
}


```

</p>
</details>

---
</div>