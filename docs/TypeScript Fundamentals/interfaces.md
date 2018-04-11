Interfaces: to declare 

```typescript
interface Point{
    x : number,
    y: number
}

let drawPoint = (point: Point) =>{
    //...
}
drawPoint({1, 4}  )
```

Classes 
According to Cohesion Principle properties and functions should be part of single entity.

```typescript
class Point{
    x : number;
    y: number;
    draw() {
        console.log("X:" + this.x + " Y : " + this.y);
    }
}

/*Create Objects */
let point = new Point();
point.x = 5;
point.x = 6;
point.draw();
```

Constructors : method which is called when object is created.  
In type script we cannot have multiple constructors. However to work with variable number of
arguments we make then option using `?` operator.

```typescript
class Point{
    x : number;
    y: number;
    
    constructor(x : number, y ?:number){
        this.x = x;
        this.y = y;
    }
}

/*Create Objects */
let point = new Point(5);
let point2 = new Point(5, 6);
```

Access Modifiers : 
public : default 
private : only access by member functions 
protected : access to child classes

```typescript
class Point{
    private x : number;
    private y: number;
    
    constructor(x : number, y ?:number){
        this.x = x;
        this.y = y;
    }
}

/*Create Objects */
let point = new Point(5);
let point2 = new Point(5, 6);
```

Access modifier in constructor parameters, both these point classes are same.  

```typescript
class Point{
    constructor(private x : number, private y ?:number){
    }
}

class Point2{
    x : number;
    y: number;
    
    constructor(x : number, y ?:number){
        this.x = x;
        this.y = y;
    }
}
```

Properties
To read and set value of fields can be given by getter and setter methods. which 
can be used as fields from outside class. 

```typescript
export class Point2{
    x : number;
    y: number;
    
    constructor(x : number, y ?:number){
        this.x = x;
        this.y = y;
    }
    get X(){
        //now we can access x using object.x notiation
    }
    set X(value){
        
    }
}

let point = new Point2(1, 2);
/* access properties like this */ 
point.x = 5;
```

Modules 
use `export keyword` to expose class as module so other classes can use that class functionalities.
then can be import using relative path. 

import { Point } from './point';
