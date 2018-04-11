 Install TypeScript 

 ```node 
 npm install -g typescript
 ``` 

 To verify check version of TypeScript compiler 

 ```node
 tsc --version
 ```

 Let's create a program `main.ts`

 ```typescript
  function log(message){
     console.log(message);
 }

 var message = "Hello World!";

 log(message);
```
 node transpile in Javascript using command 

 ```node
 tsc main.ts 
 ```

 It will convert ts file into js file. Now we can run create js file using node.

 ```node
 node main.js
 
 ```
