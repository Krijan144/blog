---
title: "Union in Typescript"
seoTitle: "union in typescript"
datePublished: Sat Jul 13 2024 04:22:57 GMT+0000 (Coordinated Universal Time)
cuid: clyjmfhsm000b09lag5pwewmh
slug: union-in-typescript
tags: typescript, union-type

---

Union in typescript allows the variable to hold more than one type of value. It is useful when variable can be of various types. It is defined by | operator between types.

```typescript
//Simple Union
let randomValue:string|number=12;
randomValue="John Doe";
//randomValue can either be string or number
```

Union Type with Function

```typescript
//Union Type with function
function randomFunc(params:string|number){
console.log(`Print ${params}`);
}
randomFunc("John");
randomFunc(12);
//Function accepts string or number as its parameter.
```

Union Type in Object

In the given example, variable Person can have object with type of Admin or Student.

```typescript
type Admin={
name:string;
role:string;
}
type Student={
name:string;
id:id
}
let Person : Admin|Student;
Person={
name:"Bob";
role:"Administrator"
}
Person={
name:"Leo",
id:1
} 
```

Union Type in Array

In the given example array can have string and number.

```typescript
let arrayValue:(string|number)[]=["John Doe",21,"Jason",1,23];
```

Union Type in Literal Values

In the given example variable requestStatus can have literal string value pending, success and error.

```typescript
let requestStatus:"pending"|"success"|"error"="pending";
requestStatus="pending";
requestStatus="error";
```