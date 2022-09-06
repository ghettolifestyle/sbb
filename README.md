# Background

This is a Bash port of `srb`, my static blog generator originally written in Ruby. It exists because of a moment of clarity I experienced during a train ride. The tools you choose for solving a given problem are as important as designing the solution itself. Or more precisely, the tools are part of the solution, and picking the right ones is essential. While this might already be obvious to you, I have always gravitated towards using less-suited tools I love over more-suited ones I don't like quite as much. And while Ruby certainly is delightful to use, I noticed that it would probably be a bit more straight forward and less complex to generate static sites using Bash.

~~This port has shaved off about 80 lines of code, which seems to support the thesis that Bash is the more suitable language.~~ Most of the lines of code that were shaved off were comments and obsolete code, so whether this is actually the more efficient script, I have no idea. Regardless, due to the easy-to-use nature of the shell, I was actually able to rewrite some especially ugly hacks still existing in the original, mostly by making proper use of file mtime manipulation. Discovering the details will be left to your trained eye.

In conclusion, this coding exercise has led to a new-found appreciation for the good old Bourne-again shell on my part, and I look forward to the next wave of inspiration.

# Dependencies

+ rsync
+ imagemagick (not needed if blog won't host images)
+ ssh/scp
+ pandoc
