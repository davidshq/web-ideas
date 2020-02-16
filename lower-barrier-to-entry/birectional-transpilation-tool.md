# 2. A Bidirectional Transpilation Tool
I'm sure I'll lose some readers right here, but I'll say it anyways: **I find anonymous functions, at least when used extensively, quite annoying due to the decreased readability (imho) of the code.**

Harold Abelson said, "Programs must be written for people to read, and only incidentally for machines to execute." Now if I'm honest I'll admit I've never read SICP (I'd like to) and as such I may be misusing/abusing Abelson's quote...but even if that is the case, I think the statement standing alone, without context or understanding of the original author's intent is still true.

There is so much of our code that is not readable except by someone who has spent a significant amount of time coding. Sometimes this is necessary but oftentimes it seems to be about preference OR slight expediency for the coder.

I'm not going to suggest we stop using more condensed/expedient/preferred methods of coding as I think that would be a non-starter. However, I would suggest that a simple transpilation tool which could take code written in a specific language and translate it into a more verbose form would be useful.

For each project one could set a "preferred" code mode - verbose or concise, emphasize readability or productivity. When an individual opened a project their editor would be set to a "preferred" mode. If the preferred mode differed from the project's preferred mode, the editor (or a language server, transpiler) would translate the code into the preferred method almost instantaneously. When the individual saved the project back to the shared source code repository (we are using version control, right? right?!) the editor would ensure that the saved code cofnormed to the "preferred" project mode.

In this way newer developers could work alongside more experienced developers more productively...and it could serve as a powerful learning tool. One could choose, for example to have the two code forms appear side by side and be able to see at a glance what the more verbose code looked like underlying some concise code. This could help individuals bridge the gap between their more basic understanding and a more "advanced" understanding.

I realize there would be some difficulties with this approach. For example, when making anonymous functions verbose what would one call them? They are anonymous! But this is not an insurmountable obstacle though I won't address it further here atm in order to avoid this proposal becoming quite lengthy.
