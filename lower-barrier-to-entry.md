# Lowering the Barrier to Entry for Development

# Introduction
My first computer was a Commodore 64 that upon boot dropped me to a command prompt that ran BASIC. Soon thereafter I'd find my way to the Apple II series which offered the same experience. Microsoft DOS didn't offer it at the terminal but some variant of basic (most famously QBasic) came bundled with the system and with later Windows systems as well.

When I became a (relatively) early internet adopter the ISP I used (AOL) bundled web hosting with internet access and creating pages that others would actually read could be accomplished in straight HTML. Over time tidbits of CSS and JavaScript became useful too.

The barrier to entry was low, the tools were free, and the time to visible and pleasing results was minimal. Not anymore.

# Don't Want to Go Back
I'm not stuck in a nostalgic past, I don't want to return to those old ways because the "things" we created (applications, pages, etc.) were much more limited than those we can build today.

That said, I do think we have a real issue with being approachable. While we have more powerful systems with more rapid tools for development and more resources from which to learn this has not made:

(a) it easier for individuals to get started in development
or
(b) allow hobbyists/casual developers to create more innovative solutions

We need a simpler way to introduce individuals to development and to facilitate the implementation of hobbyist ideas by individuals with constrained resources (especially time).

# What to Do?
There are several ways in which we could simplify the barriers to new/casual developers. At one time I thought the path forward might be a new development stack, or at least a DSL within an existing development stack. But the proliferation of languages and tools has made me doubt the wisdom of this approach.

Instead I would like to propose three potential ways forward.

## 1. A Conceptual Subset
Look at any of the popular roadmaps for learning development technologies scattered across github and you'll see paths of significant complexity that look quite overwhelming to experienced developers, much less to new or casual ones.

For this reason I would suggest we create a standardized subset of concepts which are necessary for the creation of "normal" applications.

(See Appendix A for examples of what this subset might look like)

## 2. A Bidirectional Transpilation Tool
I'm sure I'll lose some readers right here, but I'll say it anyways: **I find anonymous functions, at least when used extensively, quite annoying due to the decreased readability (imho) of the code.**

Harold Abelson said, "Programs must be written for people to read, and only incidentally for machines to execute." Now if I'm honest I'll admit I've never read SICP (I'd like to) and as such I may be misusing/abusing Abelson's quote...but even if that is the case, I think the statement standing alone, without context or understanding of the original author's intent is still true.

There is so much of our code that is not readable except by someone who has spent a significant amount of time coding. Sometimes this is necessary but oftentimes it seems to be about preference OR slight expediency for the coder.

I'm not going to suggest we stop using more condensed/expedient/preferred methods of coding as I think that would be a non-starter. However, I would suggest that a simple transpilation tool which could take code written in a specific language and translate it into a more verbose form would be useful.

For each project one could set a "preferred" code mode - verbose or concise, emphasize readability or productivity. When an individual opened a project their editor would be set to a "preferred" mode. If the preferred mode differed from the project's preferred mode, the editor (or a language server, transpiler) would translate the code into the preferred method almost instantaneously. When the individual saved the project back to the shared source code repository (we are using version control, right? right?!) the editor would ensure that the saved code cofnormed to the "preferred" project mode.

In this way newer developers could work alongside more experienced developers more productively...and it could serve as a powerful learning tool. One could choose, for example to have the two code forms appear side by side and be able to see at a glance what the more verbose code looked like underlying some concise code. This could help individuals bridge the gap between their more basic understanding and a more "advanced" understanding.

I realize there would be some difficulties with this approach. For example, when making anonymous functions verbose what would one call them? They are anonymous! But this is not an insurmountable obstacle though I won't address it further here atm in order to avoid this proposal becoming quite lengthy.

## 3. Simplified Development Environments
In the old days I could boot up a computer, open my IDE, write some code and click run/compile and see the result. It was wonderful! I could then distribute the compiled result to others. Things are rarely this simple anymore...with JavaScript being perhaps the most egregious example with its infinitely nested dependencies and variation tooling.

Note: I'm not saying JS is the only culprit. I've pulled my fair share of hair out working with other languages like Python and PHP as well.

Now we have reduced this problem for ourselves (somewhat) through the use of virtualization and containerization technologies. However, these technologies are almost uniformly unfriendly to the new developer and can still introduce significant complexities for more experienced developers. Not to mention that these environments almost always are command-line, non-UI driven and lack an integrated IDE experience.

We have been seeing some progress on this front with cloud based tools that package the environment and tooling together. Cloud9 was a personal favorite of mine and more recently Microsoft's Visual Studio Code has knocked off my socks with their beautiful editor/environment integrations (and Theia's work is also fascinating).

Still, there is much work to be done on this front. Ideally, all major languages and development stacks would have a bundled option that included an IDE and environment installed through a simple installer and that included straightforward methods for moving from development to production.

Thing of this as create-react-app, etc. with a GUI and on steroids.

# Conclusion
I'm not married to these particular methods of simplifying development but I do think we owe it to the community to provide better ways to learn and create without the necessity of full-time education or employment in the field.

# Appendix A. Examples of a Potential Conceptual Subset.
Here I'll make some crazy suggestions on ways in which we could simplify what we teach. I kept these to the end not only to avoid being too lengthy but also because I know what I'm saying is opinioniated and controversial. I'm certainly open to going in the exact opposite direction of what I'm proposing...although my ideas are best. ;-) But, seriously, the real goal is to provide a subset, a way to do things before demonstrating all ways.

Lets take a brief look at data types which are so fundamental to our code and which we often see extensively covered at the beginning of courses/books/articles on coding.

Here are my crazy suggestions:

1. Static Typing Only - Doesn't matter whether we are working with a dynamic or static language, we are teaching a way of competently developing applications.
   - This allows us to avoid early discussion of the competing concepts and it facilitates easily debugged code, something which is quite useful for all developers, but especially beginners.
   - This will also allow stripping down what needs to be taught about type coercion.
2. Pass by Value Only - I understand there is value in reference types BUT for the purposes of the new/casual/hobbyist developer and the applications they are likely to build it seems unnecessary overhead.
   - This allows us to bypass the entire conversation of by value vs by reference.
3. Only Some Data Types - There are a number of powerful data types built into most languages and these are usually discussed fairly extensively when teaching coding. However, for the purpose of most applications the optimization of types beyond some basics is unnecessary.
   - For example, in [C#](https://www.tutorialsteacher.com/csharp/csharp-data-types) we could consider using only six types and still be able to accomplish most tasks: bool, integer, decimal, obect, string, and DateTime. This eliminates ten types: byte, sbyte, short, ushort, uint, long, ulong, float, double, char.
   
Let me give one more brief example and I'll leave it there for now. An important topic in coding is operator precedence...but what if we taught everyone to use parentheses to set precedence? Now individuals no longer have to remember (at least from the get go) the relative order of precedence and instead can use what they know from basic math classes to ensure that calculations are performed in the correct order. (And I'd suggest, in general, it is better practice to use parentheses as this increases readability by humans and decreases the likelihood of accidental miscalculations due to incorrect ordering of operators).

Signing off my heretical thoughts, send me back your snide remarks or kudos!

