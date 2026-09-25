---
layout: essay
type: essay
title: "Order and Chaos of being a Programmer"
# All dates must be YYYY-MM-DD format!
date: 2026-09-24
published: true
labels:
  - VScode
  - ESLint
  - Coding Standards
---


# Order and Chaos of being a Programmer


## Coding Standards: Why coding needs law and order, too.

Coding standards are important because they make code readable, clean, and easier to maintain. I also believe that coding standards can help someone learn a programming language. When I first started programming, my main goal was simply to make the code work. If the program ran without errors, I considered that a success. However, working code is not always good code. Coding standards have taught me that how the code is written also matters.
For example, TypeScript can be written in a messy way and still work:

```typescript
function greet(name:string){let message="Hello "+name;if(name=="Donald"){message="Welcome back "+name}return message}
console.log(greet("Donald"))
```

The computer may understand this code, but a human has to spend more time figuring out its structure. With coding standards and ESLint, the same code can be written more clearly:

```typescript
function greet(name: string): string {
  let message = `Hello ${name}`;

  if (name === 'Donald') {
    message = `Welcome back ${name}`;
  }

  return message;
}

console.log(greet('Donald'));
```

Both versions accomplish basically the same task, but the second version is much easier to read. The spacing, indentation, strict equality, consistent quotation marks, and clear return type make the structure easier to understand. This becomes even more important when working on a large project or when another programmer needs to read the code.

## ESLint, the order keeper.

After the week of using ESLint, I have found it both useful and annoying. ESLint sometimes feels like TypeScript with extra steps. Setting it up takes time, and some of its rules can feel strange when you first encounter them. For example, I had to get used to syntax such as `{ type }` instead of `{type}`. Other rules can feel extremely strict, such as complaining because I used double quotes instead of single quotes. Sometimes it feels like ESLint is saying, "Your program works, but I don't like how you typed it."

Despite that frustration, I can see why ESLint is useful. Repetition helps build good programming habits. If ESLint keeps reminding me to format something correctly, eventually I will start writing it correctly without thinking about it. The goal is not necessarily to create perfect code, because perfect code probably does not exist. Instead, coding standards help create code that is consistent and understandable.

## VScode, the battlefield.

I also like using VSCode as my main IDE. It may sometimes feel slower than simpler editors, but it is easy to understand and highly customizable through extensions. ESLint integration is especially useful because VSCode can point out problems while I am writing code instead of waiting until later. This gives me immediate feedback and helps me learn what I did wrong.

Overall, I agree that coding standards are one of the most useful software engineering techniques for improving code quality. They do not automatically make someone a good programmer, and following every rule can sometimes be annoying. However, they encourage habits that make code easier to read, debug, maintain, and share with other developers. My experience with ESLint has been a mixture of frustration and learning, but I think that frustration has a purpose. With enough repetition, I hope I will eventually write clean code naturally instead of having ESLint yell at me every five seconds.