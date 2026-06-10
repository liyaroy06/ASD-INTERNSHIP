let products = [
{ name: "Monitor", price: 12000, quality: "Good" },
{ name: "Speaker", price: 3000, quality: "Low" },
{ name: "Printer", price: 15000, quality: "Good" },
{ name: "Pendrive", price: 700, quality: "Low" },
{ name: "Router", price: 4500, quality: "Low" }
];

// 1. Search Product by Name
let productName = "Monitor";

for(let i = 0; i < products.length; i++){
if(products[i].name == productName){
console.log(products[i]);
}
}

// 2. Search Product by Price
let productPrice = 15000;

for(let i = 0; i < products.length; i++){
if(products[i].price == productPrice){
console.log(products[i]);
}
}

// 3. Display Products Above ₹5000
for(let i = 0; i < products.length; i++){
if(products[i].price > 5000){
console.log(products[i]);
}
}

// 4. Display Products Below ₹5000
for(let i = 0; i < products.length; i++){
if(products[i].price < 5000){
console.log(products[i]);
}
}

// 5. Count Total Products
let count = 0;

for(let i = 0; i < products.length; i++){
count++;
}

console.log(count);

// 6. Most Expensive Product
let highestProduct = products[0];

for(let i = 0; i < products.length; i++){
if(products[i].price > highestProduct.price){
highestProduct = products[i];
}
}

console.log(highestProduct);

// 7. Cheapest Product
let lowestProduct = products[0];

for(let i = 0; i < products.length; i++){
if(products[i].price < lowestProduct.price){
lowestProduct = products[i];
}
}

console.log(lowestProduct);

// 8. Add New Product
let newProduct = {
name: "Webcam",
price: 2500,
quality: "Low"
};

products[products.length] = newProduct;

console.log(products);

// 9. Delete Product by Name
let removeProduct = "Speaker";

for(let i = 0; i < products.length; i++){
if(products[i].name == removeProduct){
products.splice(i, 1);
}
}

console.log(products);

// 10. Update Product Price by Name
let itemName = "Router";

for(let i = 0; i < products.length; i++){
if(products[i].name == itemName){
products[i].price = 5000;
}
}

console.log(products);

// 11. Display Only Product Names
for(let i = 0; i < products.length; i++){
console.log(products[i].name);
}

// 12. Display Only Product Prices
for(let i = 0; i < products.length; i++){
console.log(products[i].price);
}

// 13. Check Whether Product Exists
let searchItem = "Printer";
let status = "Not Found";

for(let i = 0; i < products.length; i++){
if(products[i].name == searchItem){
status = "Found";
}
}

console.log(status);

// 14. Good Quality and Low Quality Categories
console.log("Good Quality");

for(let i = 0; i < products.length; i++){
if(products[i].quality == "Good"){
console.log(products[i]);
}
}

console.log("Low Quality");

for(let i = 0; i < products.length; i++){
if(products[i].quality == "Low"){
console.log(products[i]);
}
}

// 15. Products Between ₹5000 and ₹50000
for(let i = 0; i < products.length; i++){
if(products[i].price >= 5000 && products[i].price <= 50000){
console.log(products[i]);
}
}

// 16. Sort Products by Price Ascending
for(let i = 0; i < products.length; i++){
for(let j = i + 1; j < products.length; j++){
if(products[i].price > products[j].price){
let temp = products[i];
products[i] = products[j];
products[j] = temp;
}
}
}

console.log(products);

// 17. Sort Products by Price Descending
for(let i = 0; i < products.length; i++){
for(let j = i + 1; j < products.length; j++){
if(products[i].price < products[j].price){
let temp = products[i];
products[i] = products[j];
products[j] = temp;
}
}
}

console.log(products);

// 18. Display Products with 18% GST
for(let i = 0; i < products.length; i++){
let totalPrice = products[i].price + (products[i].price * 18 / 100);

```
console.log(products[i].name + " = " + totalPrice);
```

}

// 19. Calculate Total Inventory Value
let inventoryAmount = 0;

for(let i = 0; i < products.length; i++){
inventoryAmount += products[i].price;
}

console.log(inventoryAmount);

// 20. Product Report
for(let i = 0; i < products.length; i++){
console.log(
"Product : " + products[i].name +
", Price : " + products[i].price +
", Quality : " + products[i].quality
);
}
