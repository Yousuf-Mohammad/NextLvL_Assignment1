Blog1: What is type inference in TypeScript? Why is it helpful?

In simple words TypeScript guesses the type of your variables when you don’t tell it explicitly. This is know as Type inference

Example : let name = "Yousuf Mohammad";

even though I havent said anywhere in the code this is a string , but TypeScript will take the variable " name" as string .

whats more interesting is , We can not assign value of any other type but string .

Example : name = 27 ( this will through an error )
