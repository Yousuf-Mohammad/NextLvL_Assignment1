<!-- Full-width Banner Image -->
<p align="center">

  <img src="./Facebook Cover - What is Type Inference in TypeScript.png" alt="Type Inference in TypeScript - Yousuf Mohammad" width="100%" />
</p>

# 📝 Blog 1: What is Type Inference in TypeScript? Why is it Helpful?

In simple words, **TypeScript can guess the type of your variables even when you don’t explicitly tell it. This smart feature is called [Type Inference](https://www.typescriptlang.org/docs/handbook/type-inference.html).**

---

### 📦 Example:

```ts
let name = "Yousuf Mohammad";
```

Even though I didn’t specify that `name` is a string, TypeScript is smart enough to figure it out.

What’s more interesting? You can’t assign a value of a different type—even if you try:

```ts
name = 27; // ❌ This will throw an error
```

## Why is type Inference Helpful ?

### 1 . Less Typing , More Chilling 😎:

It saves you from typing every single type explicitly

```ts
let chill = 100; // instead of let chill : number = 100 ;
```

That’s more time to binge your favorite series! 😎

### 2. Better Auto Completion 🚀:

Just hover over the variable and—bam!—you’ll see the inferred type automatically. It’s super helpful when you're using the variable later

### 3. Still Fully Typed💪

:

Here’s the best part: your code is still strongly typed.
So you don’t have to compromise on type safety.
<br>

<br>

> "Type Inference in TypeScript is like autopilot for types.
> <br>
> It keeps your code safe, saves you time, and lets you focus on the fun parts of coding."

**So go on, happy coding! 🚀**

# 📝Blog2: `any` `unknown` and `never` Three Weirdos in _TypeScript_.

The very first I heard these name, I thought Who the Hell named this type :3 These name reflects extensial crysis of names

Lets Explore the wierd types of the Typescript togather.

## 1. `any` - The Uradhura Guy :

`any` in the TypeScript is like the careless person you know in your life may be more . Use `any` in on a variable or interface . and typescript will be like :

> TypeScript : " Do whatever you want , I dont care "

## Example:

```ts
let uradhura = "Yousuf";
uradhura = 123; // ok fine, I dont care
uradhura = true; //ok fine, I dont care
uradhura = { takaPoisha: "Nai" }; //Ok fine , I dont care ;
```

Using `any` is like My life My rule , which sounds fun ...until bugs find your way, and trust me they know where you are !!!

> <br>
> So `any` is  <br>
> ✅ Great for quick experiments.<br>
> ❌ Terrible for code safety.
> <br> <br>

<br>
<br>
<br>

## 2.`unknown` -TypeScript er misir ali

`unknown ` is a paranoid twin of `any` . Assign any value you like to an `unknown` it will accept . But , but , but Whenever you trying do anything to the value `unknown` will not do anything untill you prove it

`unknown ` in typescript be like:

> <br>
> dev : Here is a string keep it safe . <br><br>
> unknown: Ok sir<br><br>
> dev: Can you give me the length of the string in the unknown<br><br>
> unknown: You say it’s a string... but do you have proof, sir? (Poman dao)<br><br>

## Example:

```ts
let keuJaneNa: unknown = "Misir Ali ";

keuJaneNa.toUpperCase(); // ❌ Nope!
```

## So need to check type first

```ts
if (typeof keuJaneNa === "string") {
  console.log(keuJaneNa.toUpperCase());
}
```

## 3. `never` - the lalbagh kella surongo

`never ` is like a black hole anything comes here never returns.

### When does that happen ?

- A function that throws an error and never comes back
- A function that loops forever .

## Example:

```ts
function dontComeHere(): never {
  throw new Error("You are dead !!");
}
```

✅ It’s mostly for super precise typing or for catching impossible states in union types.<br>
🔒 Rarely written by hand, but used a lot behind the scenes.

## wrap up 
* Use `any` when you don’t care (but probably should).

* Use `unknown` when you care (and want safety).

* Use `never` when things should never happen (like your app going into a black hole).

And remember: TypeScript types are like seatbelts. Might feel annoying at first, but they save lives (and debugging hours).
