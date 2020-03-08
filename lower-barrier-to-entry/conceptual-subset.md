# A Conceptual Subset.
Look at any of the popular roadmaps for learning development technologies scattered across github and you'll see paths of significant complexity that look quite overwhelming to experienced developers. How much moreso to new developers and hobbyists?

For this reason I would suggest we create a standardized subset of concepts which are necessary for the creation of "normal" applications (I'm thinking here LOB, CRUD, etc.).

A starting place for this venture might be using some of the "State of x" surveys floating around the web to choose between important and unimportant topics.

- "Any fool can write code that a computer can understand. Good programmers write code that humans can understand." - Martin Fowler, Refactoring, 1999.

## A Few Examples of Simplified Concepts.
Here I'll make some crazy suggestions on ways in which we could simplify what we teach. I know what I'm saying is opinioniated and controversial. I'm very open to changing what concepts should be taught as long as it is a subset...and I suppose someone might convince me this is a bad idea altogether.

### Static Typing Only
- Doesn't matter whether we are working with a dynamic or static language, we are teaching a way of competently developing applications.
- This allows us to avoid early discussion of the competing concepts and it facilitates easily debugged code, something which is quite useful for all developers, but especially beginners.
- We can significantly simplify discussions of type coercion.

### Pass by Value Only
- I understand there is value in reference types BUT for the purposes of the new/casual/hobbyist developer and the applications they are likely to build it seems unnecessary overhead.
- This allows us to bypass the entire conversation of by value vs by reference.
- "It's sad to see how many Just JavaScript readers got confused by someone in the past who taught them about 'passing by value' and 'passing by reference'. These concepts don't map well to JavaScript and lead to all sorts of misconceptions. I wish people could forget them." - [Dan Abramov](https://twitter.com/dan_abramov/status/1226661266187595776).

### Only Some Data Types
- There are a number of powerful data types built into most languages and these are usually discussed fairly extensively when teaching coding. However, for the purpose of most applications the optimization of types beyond some basics is unnecessary.
- For example, in [C#](https://www.tutorialsteacher.com/csharp/csharp-data-types) we could consider using only six types and still be able to accomplish most tasks: bool, integer, decimal, object, string, and DateTime (six types). This eliminates ten types: byte, sbyte, short, ushort, uint, long, ulong, float, double, char.
### Use Parentheses Always for Precedence
An important topic in coding is operator precedence...but what if we taught everyone to use parentheses to set precedence? Now individuals no longer have to remember (at least from the get go) the relative order of precedence and instead can use what they know from basic math classes to ensure that calculations are performed in the correct order. (And I'd suggest, in general, it is better practice to use parentheses as this increases readability by humans and decreases the likelihood of accidental miscalculations due to incorrect ordering of operators).

## Rough, Half-Written, Half-Crazed Example Subsets.
- [CSS Subset](conceptual-subset-css.md).