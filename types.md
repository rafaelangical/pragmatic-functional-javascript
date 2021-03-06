# Types

JavaScript by default doesn't provide support for static type or even runtime type checking. By having type coercion, all the syntactic valid programs are accepted and type errors will only be caught in runtime. For the sake of sanity, there are good tools we can use to make JavaScript code safer and identify most of the runtime errors of a program before they happen, I mean at compile time, like Flow or even TypeScript, the JavaScript superset.

## Why types matter

Do we really need types? At first, this should be an obligation of the compiler; it should be its responsability to ensure that your program is correct and let you worry only about the logic, but this is not what happens on the most popular programming languages. You might not need static type checking, but, for sure, having it will help you writing programs that are more correct and safer, avoiding a lot of possible errors that would only happen in specific situations when executing your program. In fact, static type checking will not replace unit tests at all, but will replace the sort of them that are applied to inputs of invalid types.

When talking about type checking, most people remember about Java, but this is definitely a terrible example of how a type system should be. Seriously, the type system implemented in Java forces you to declare things that the compiler already knows and accepts invalid programs because it is not well designed to deal with a thing we will call _subtyping_. In the section 12, "A bit of theory", we will give you a gentle introduction to type theory; we will not focus specifically on Java, but in systems that can be implemented in the subset of functional languages and explain how type inference works and why most of the languages have awful type systems that make a lot of people hate static typing. If you say you hate static typing, I'm 99% sure you don't hate static typing, but having to write type signature for obvious things and having to waste timing making the work that the compiler should do.

## Flow is your friend

Hopefully, to save us from the world of badly-typed programs, we have Flow.



