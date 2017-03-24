# Exam
## Promise
1. Which of them **are** right?  
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

##HTML
1. In this HTML page, how many blanks(□) we have between \`a\` and \`test\`?
```HTML
<div>
Hi, this is a□□&nbsp;□test.
</div>
```
2. We have codes in the page with the URL: http://test.com/frontend/2017,
```HTML
<a href="ex1">ex1</a>
<a href="/ex2">ex2</a>
<a href="./ex3">ex3</a>
```
After clicking ex1, it will open the link ______________________  
After clicking ex2, it will open the link ______________________  
After clicking ex3, it will open the link ______________________  
3. 

#NodeJS

