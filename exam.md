# Javascript/HTML/jQuery/NodeJS Test
## Sync
1. Which of the follow codes are **correct**?  **( B, D )**  

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
2. Which one of the follow results is correct ? **( B )**  
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
3. Which is better? **( B )**  

A.
```javascript
var lng = 0;
const oldDataLength = 10;
$.ajax('/api/productList', {...options}, (data)=>{
    lng = data.length;
})
$('#totle').text(lng + oldDataLength);
```
B.
```javascript
let lng = 0;
const oldDataLength = 10;
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
1. In the HTML page with the codes below, how many blanks(□) we can see in the browser between \`a\` and \`test\`?  **( 3 )**
```HTML
<div>
Hi, this is a□□&nbsp;□test.
</div>
```
2. The codes below is in the page with the URL "http://test.com/frontend/2017" **( C )**    
```HTML
<a href="ex1">ex1</a>
<a href="/ex2">ex2</a>
<a href="./ex3">ex3</a>
```
After clicking ex1, it will open the link: ______________________  
After clicking ex2, it will open the link: ______________________  
After clicking ex3, it will open the link: ______________________  
A. http://test.com/frontend/2017/ext1  
   http://test.com/frontend/2017/ext2  
   http://test.com/frontend/2017/ext3  
B. http://test.com/ext1  
   http://test.com/ext2  
   http://test.com/frontend/2017/ext3  
C. http://test.com/frontend/2017/ext1  
   http://test.com/ext2  
   http://test.com/frontend/2017/ext3  
D. http://test.com/ext1  
   http://test.com/frontend/2017/ext2  
   http://test.com/frontend/2017/ext3  
3. Which is correct ? **( A )**
```HTML
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
A. Set the initial zoom level when the page is first loaded  
B. Fix the zoom level when the page is first loaded  
C. Fix the zoom level when the page is refreshed  
D. Set the resolution at 960*480
## NodeJS
1. Which one of them can print the current path ?  **( C )**  
A. console.log(path.name)  
B. console.log(\_\_dirname\_\_)  
C. console.log(process.cwd())  
D. console.log('./')  

2. How to install Express with npm and add dependencies to package.json ? **( A )**  
A. npm install --save-dev express  
B. npm install express  
C. yum install express  
D. webpack -p express  
3. How to import the \`webpack\` library to use ? **( C )**  
A. const webpack = npm.webpack  
B. const webpack = import from 'webpack'  
C. const webpack = require('webpack')  
D. include webpack from 'webpack'  
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
1. Which of them can get the element? **( A, C )**  
A. $('.products > ul > li:first').find('span')  
B. $('.products > span:first')  
C. $('.products span:first')  
D. $('span').text('product 1').first()  
2. How to get the closest div of the specified span ? **( D )**  
A. $(...specified span...).find('div')  
A. $(...specified span...).parent('div')  
A. $(...specified span...).closest('div:first')  
A. $(...specified span...).closest('div')  
3. How to select odd \`li\` elements ? **( A )**  
A. $('.products li:odd')  
B. $('.products ul:odd').find('li')  
C. $('.products li').filter('odd')  
D. $('.products li').find('odd')  
4. How to search a specified value within an array with jQuery?  **( C )**  
A. $.sub(9, [2,83,99,9,27,283])  
B. $.indexOf(9, [2,83,99,9,27,283])  
C. $.inArray(9, [2,83,99,9,27,283])  
D. $.find(9, [2,83,99,9,27,283])  
