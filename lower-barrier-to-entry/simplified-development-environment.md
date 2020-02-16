# 3. Simplified Development Environments
In the old days I could boot up a computer, open my IDE, write some code and click run/compile and see the result. It was wonderful! I could then distribute the compiled result to others. Things are rarely this simple anymore...with JavaScript being perhaps the most egregious example with its infinitely nested dependencies and variation tooling.

Note: I'm not saying JS is the only culprit. I've pulled my fair share of hair out working with other languages like Python and PHP as well.

Now we have reduced this problem for ourselves (somewhat) through the use of virtualization and containerization technologies. However, these technologies are almost uniformly unfriendly to the new developer and can still introduce significant complexities for more experienced developers. Not to mention that these environments almost always are command-line, non-UI driven and lack an integrated IDE experience.

We have been seeing some progress on this front with cloud based tools that package the environment and tooling together. Cloud9 was a personal favorite of mine and more recently Microsoft's Visual Studio Code has knocked off my socks with their beautiful editor/environment integrations (and Theia's work is also fascinating).

Still, there is much work to be done on this front. Ideally, all major languages and development stacks would have a bundled option that included an IDE and environment installed through a simple installer and that included straightforward methods for moving from development to production.

Thing of this as create-react-app, etc. with a GUI and on steroids.