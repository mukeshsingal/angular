We use declare variables using commands like 

```js 
var variableName 
```

In Javascript variable craeted with var keyword, scope to nearest function.


```js 
let variableName 
```

Using let keyword variable script to nearest block not function. Helps in catches issues earlier. 

### Type Annotation

```typescript
let a: number;
```
a = 5;           //valid
a = "Sum";      //invalid 

Types can be `number`, `boolean`, `string`, `any`, `number[]`, `enums`

Enums : to manage group of related constants 

```typescript
enum enumname = {key1 = value1, key2 = value2 };

let needKey1 = enumname.key1
```

### Type Assertion
Explict declaration of type. 
```typescript
let message;
message = 'abc';

//First way 
let endswithc = (<string> message).endsWith('C');
//second way 
let endswithC = (message as string).endsWith('C');
```
