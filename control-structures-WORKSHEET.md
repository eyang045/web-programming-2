# Control Structures
In Web 1 you learned about the following **control structures**:
1. IF Statements (and all of their variations)
1. While Loops
1. For Loops

Now you will explore the control structures that are listed below. 
For each one, write a brief paragraph that describes the control
structure and the situations when you would use it.
Also, include a fun and imaginative code sample that demonstrates 
the control structure.

## Switch/Case Statement
A switch statement is another way to write multiple IF/ELSE IF statements when you're checking the same variable against different values. You would use Switch when you're
asking "Is this variable equal to option A? Option B? Option C? and so on". An example of using a switch would be when you're asked a question like "What would you like to
drink?". You would say "If they have Coke, I'll take Coke", If they have Sprite, I'll take Sprite", If they have Lemonade, I'll take Lemonade", "If they don't have any of 
these, I'll take water". A switch statement is like checking a menu of specific options. It takes one thing (your drink choice) and compares it against a list of possibilities.

```js
let drinkChoice = "Sprite";

switch(drinkChoice){
    case "Coke":
        console.log("Here's your Coke!");
        break;
    case "Sprite":
        console.log("Here's your Sprite!")
        break;
    case "Lemonade":
        console.log("Here's your Lemonade!")
        break;
    default:
        console.log("Sorry, we only have water!");
}
```

## For/In Loop
A For/In Loop is a tool that lets you look at everything inside a box (an object) one item at a time. Think of an object as a backpack. The backpack could have labeled pockets.
Pocket labeled "phone" which contains your phone, Pocket labeled "wallet" which contains money inside it, and Pocket labeled "keys" which contains your car keys. A For/In Loop goes through each pocket and tells you what the pocket is labeled and what is inside that pocket.

```js
let backpack = {
    phone: "iPhone",
    wallet: "$50",
    keys: "car keys"
};

for(let item in backpack){
    console.log("I found: " + backpack[item]);
}
```

## Conditional Operator (aka Ternary Operator)
A ternary operator is a shortcut way to write a simple IF/ELSE statement all in one line. It asks a question, and if the answer is true, it does one thing. If the answer is false, it does another thing. The syntax is "condition ? valueIfTrue : valueIfFalse", where the question mark "?" means "if true, use this," and the colon ":" means "otherwise, use this." You would want to use this when you have a simple IF/ELSE statement with only two outcomes, want to assign a value based on a condition, and when you want a more cleaner and more concise code for simple decisions.

```js
let age = 20;
let status = age >= 21 ? "Can enter the bars!" : "Cannot enter the bars yet!";
console.log(status);
```
