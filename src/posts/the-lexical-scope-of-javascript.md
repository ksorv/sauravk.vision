---
layout: layouts/post.njk
title: The Lexical Scope of Javascript!
metaTitle: The Lexical Scope of Javascript!
metaDesc: To understand why sometimes 'this' is undefined and sometimes things
  just work, You need to understand The Lexical Scope.
date: 2020-07-18T12:05:00.459Z
tags:
  - Javascript
  - Scope
  - Hard parts
  - Lexical
---
Have you ever wondered why sometimes, `this` was undefined, while you thought it was there and that sometimes your functions work in weird ways. Well, then you're at the right spot. We'll be discussing **Lexical Scopes**, in this post.

- - -

## What is Lexical Scope?

Javascript is basically a compiled language, The code you write is first compiled to AST then to a efficient binary, which is later executed by the JS Engine. All the variables and scopes are placed on their positions after declaration, So that they can be used by the engine while executing the program. All the declarations at the time of compilation are done in different scopes, For example:

```js
var call = "Mr."

const Greet = function(name){
    const greeting = "Good Morning";
    console.log(`${greeting}, ${call} ${name}`)
}

Greet("Saurav")
```

So, What is lexical scope in here! Let's break it down.

* Compiler first declares the `var call`, in global scope(No problemo).
* Compiler then, declares a `const Greet` and assigns it the func we defined, in Global scope.
* Then, Compiler goes inside the function we defined(New Scope Manager for the function), and checks(consults the global scope manager) if there is a greeting variable already defined in the upper scope(i.e, Global scope), if not, then it goes ahead and declares greeting.

  * The Compiler checks in with current Scope Manager(of function), if there is a `greeting` declaration.
  * Then, Compiler checks for call, but 

    The functions Scope Manager says: I don't know bruh, Who's this? Ask big brother global Scope Manager!

    Compiler asks global Scope manager, it replies with **Yes!, I've call already declared**.

    This is lexing, The `call` declaration is available to function's Scope Manager through `lexical scope`.
  * **Lexical Scope** is nothing too complicated(assume it!), It is just the Scope that is determined during the compilation and is available from outer to inner scopes. e.g, Global scope is available to every scope, so on and so forth.
* Compiler then comes to the `Greet("Saurav")` statement. Checks Greet, it's declared and Compilers compiles the code to AST.

**Execution takes place after this.**

There are more steps, but let's not discuss them now. I think you get what lexical scope is?

If still, You've got some doubts? Let's discuss them, Tweet [@sauravkhdoolia](https://twitter.com/sauravkhdoolia)

### Resources: 

\- [Scopes](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/scope-closures/ch1.md)

\---

You're reading this post on The Vision project. Please report any issues [here](https://github.com/sauravkhdoolia/sauravk.vision/issues/new)