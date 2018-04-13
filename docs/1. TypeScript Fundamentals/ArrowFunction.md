 ### How to Install TypeScript 

>  npm install -g typescript

To verify check version of TypeScript compiler 
 
 > tsc --version
 
 Let's create a program `main.ts`

 ```typescript
  function log(message){
     console.log(message);
 }

 var message = "Hello World!";

 log(message);
```
 Node transpile in Javascript using command 


> tsc main.ts 


 It will convert ts file into js file. Now we can run create js file using node.


>  node main.js
 
### How to write lembda function in TypeScript

```typescript
/* In JavaScript function is defined like this */ 
let log = function(message) {
  console.log(message);
}
```


In TypeScript function can be defined like lemda Expressions.
```typescript
let variable = (parameters) =>{ /*do Something*/ };
````
Example.. 

```typescript
let doLog = (message) => console.log(message);    

```
