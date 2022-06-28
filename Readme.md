# IBO (Ebo Mart Private Limited)

<div>

---

### You have been given a list of products which is having property productName, quantity and description.

```javascript
const listOfProducts = [{
    productName: "TV",
    quantity: 10,
    description: "television"
  },
  {
    productName: "AC",
    quantity: 5,
    description: "air conditioner"
  },
  {
    productName: "TV",
    quantity: 10,
    description: "television"
  },
  {
    productName: "AC",
    quantity: 5,
    description: "air conditioner"
  },
  {
    productName: "FAN",
    quantity: 10,
    description: "Ceiling Fan"
  }
];

```

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

### 2. you need to write a function say, getUniquePrducts which should return an array of objects by grouping the products based on the productName and summing up the quantity for the same products present in the given list of Products considering Product Name as Key.

###### Sample Output for the given listOfProducts will be :

```javascript
[{
    productName: "TV",
    quantity: 20,
    description: "television"
  },
  {
    productName: "AC",
    quantity: 10,
    description: "air conditioner"
  },
  {
    productName: "FAN",
    quantity: 10,
     description: "Ceiling Fan"
  }
]

```

<details><summary><b>Answer</b></summary>
<p>

#### Answer:

```javascript
const getUniquePrducts = (listOfProducts)=>{
    
    let arr = [];
    listOfProducts.filter((product)=>{
        if (arr.find((element)=> element.productName === product.productName)){
                arr.find((element) =>{
                    if (element.productName === product.productName) {
                        element.quantity += product.quantity;
                    }
                });
        }
        else{
            arr.push(product);
        }
    });
    return arr;
}

console.log(getUniquePrducts(listOfProducts));

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