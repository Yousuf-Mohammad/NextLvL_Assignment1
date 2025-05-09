<!-- Full-width Banner Image -->
<p align="center">

  <img src="./Facebook Cover - What is Type Inference in TypeScript.png" alt="Type Inference in TypeScript - Yousuf Mohammad" width="100%" />
</p>

# 📝 Blog 1: What is Type Inference in TypeScript? Why is it Helpful?

In simple words, **TypeScript guesses the type of your variables when you don’t tell it explicitly. This magical feature is known as [Type Inference](https://www.typescriptlang.org/docs/handbook/type-inference.html).**

---

### 📦 Example:

```ts
let name = "Yousuf Mohammad";
```

Even though I haven’t mentioned anywhere that name is a string, TypeScript is smart enough to figure it out.

What’s more interesting is I cannot assign a value of any other type to it even if I want to :

```ts
name = 27; // ❌ This will throw an error
```

## Why is type Inference Helpful ?

### 1 . Less Typing , More Chilling:

Reduce the stressful typing for every single variable.

```ts
let chill = 100; // instead of let chill : number = 100 ;
```

Saves time to watch another episode of your favorite TV series .

### 2. Better Auto Completion:

Just hover over the variable and see the magic . It will show the type automatically . helps in upcoming uses of the variable .

### 3. Still Fully Typed:

The best part is the code is still typed . so you dont have to worry on the type safety of your code .
<br>

<br>

> "Type Inference in TypeScript is like auto-pilot for types .
> <br>
> It keeps your code type safe , saves time ,and lets you focus on the fun part of coding ."

**So go on, happy coding! 🚀**


