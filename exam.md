# Javascript/HTML/jQuery/NodeJS Test
## Sync
1. Which of the follow codes are **correct**?

A. 
```javascript
new Promise((reolve,reject)=>{
    fetch('/api/productList', function(data) {
        resolve(data);
    });
});
```
B.
```javascript
new Promise((resolve, reject)=>{
    fetch('/api/productList').then(data=>{
       resolve(data); 
    });
})
```
C.
```javascript
let response = Promise.resolve(fetch('/api/productList'));
response(function(data){
    // deal with data
})
```
D.
```javascript
let response = Promise.resolve(fetch('/api/productList'));
response.then(function(data){
    // deal with data
})
```
2. Which of the follow results is correct (  )
```javascript
 for(var i =1; i <= 5; i ++){
 	setTimeout(function(){ console.log(i) }, 1000)
 }
 ```
 A. 0 1 2 3 4  
 B. 5 5 5 5 5  
 C. 4 3 2 1 0 
 D. 0 0 0 0 0    
 E. Random integers between 1 and 5  
3. Which is better?

A.
```javascript
var lng = 0;
var oldDataLength = 10;
$.ajax('/api/productList', {...options}, (data)=>{
    lng = data.length;
})
$('#totle').text(lng + oldDataLength);
```
B.
```javascript
let lng = 0;
let oldDataLength = 10;
$.ajax('/api/productList', {...options}, (data)=>{
    lng = data.length;
    $('#totle').text(lng + oldDataLength);
})
```
C.
```javascript
const lng = 0;
const oldDataLength = 10;
$.ajax('/api/productList', {...options}, (data)=>{
    lng = data.length;
    $('#totle').text(lng + oldDataLength);
})
```
D.
```javascript
const lng = 0;
const oldDataLength = 10;
$.ajax('/api/productList', {...options}, (data)=>{
    lng = data.length;
})
$('#totle').text(lng + oldDataLength);
```
## HTML
1. In the HTML page with the codes below, how many blanks(□) we can see in the browser between \`a\` and \`test\`?
```HTML
<div>
Hi, this is a□□&nbsp;□test.
</div>
```
2. The codes below is in the page with the URL "http://test.com/frontend/2017"  
```HTML
<a href="ex1">ex1</a>
<a href="/ex2">ex2</a>
<a href="./ex3">ex3</a>
```
After clicking ex1, it will open the link: ______________________
After clicking ex2, it will open the link: ______________________
After clicking ex3, it will open the link: ______________________

3. Which is correct ?
```HTML
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
A. Set the initial zoom level when the page is first loaded  
B. Fix the zoom level when the page is first loaded  
C. Fix the zoom level when the page is refreshed  
D. Set the resolution at 960*480

## NodeJS
1. How to print the current path ?

2. How to install Express with npm and add dependencies to package.json ?

3. How to import the  \`webpack\` library ?

## jQuery
```HTML
 <div class="orders">
    <ul>
        <li>order 1</li>
        <li>order 2</li>
        <li>order 3</li>
    </ul>
</div>
 <div class="products">
    <ul>
        <li>
            <span>product 1</span>  <!-- how to get this span? -->
        </li>
        <li>
            <span>product 2</span>
        </li>
    </ul>
    <hr />
    <ul>
        <li>
            <span>product 3</span>
        </li>
        <li>
            <span>product 4</span>
        </li>
    </ul>
</div>
 ```
1. How to get the element with jQuery?

2. How to get the closest div of the specified span ?

3. How to select odd \`li\` elements ? How to select last \`li\` element ?

5. How to search a specified value within an array with jQuery?
