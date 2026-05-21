Here is what I know about software engineering, cyber security, and networking
from online resource #self-learn.

-Latex: I was curious how they write latex code, and with the feeling of 'I need
to keep up'. 
The first I did was search which version of latex isn't taking up my space,
which is a terminal-based latex. 
first we got to create a text using.

 nano x.tex 

(the x can be anything, but don't forget to at _ when trying to be
specific.)
then inside nano or editor. We need to write 

\documentclass{article} (article not articles, it is singular)
\usepackage{amsmath}
\begin{document}

\[
E = mc^2, \frac{ \sum_a^b a^2+b}{2a} 
\]
\end{document}

(I use backward slash \  not regular /)

after that save it with ctrl + o, click enter, then ctrl + x for exit.
Now you have edited x.tex with math equation in it. Second, enter the terminal:
pdflatex x.tex
after that
we got to open the .pdf now.
xdg-open x.pdf (notice that x.pdf isn't x.tex because it has been created
 by pdflatex ).

Making a shell script executation file is kinda cool?

firstly, when making an execution file, we need to change directory(cd) to some
folder. Make a file in the folder's terminal"touch log.txt" Then we got to editor, nano McDonald.sh (here MCDonald can be anything.
For example, super_dave_the_man.sh and sh stands for shell script.)

inside the editor: 
#!/bin/bash (#! is a special interpreter)
echo "=== You Shall You Thy Truth! ==="
echo "Hello, there - General Kenobi"

uname -a  (give the operating system information such as kernal, structure or 
architecture, version, and machine information.
 For example: Linux Jake 6.12.5-ubuntu x86_64/linux)

ping -c 3 google.com (From my experience, it listed out packets on internet
strength, connection strength measurement. And -c 3 limit the packets because 
if I didn't put that, then the thing will continue for a long~~time,
 non-stop until I press: ctrl + c to cancel it) 

Then ctrl + o, press enter, ctrl + x.

now we have McDonald.sh is now created or edited.

After that we need to give it a type and an access permission.
There are three type of file in chmod:

r: read, w: write, x: execute

chmod +x McDonald.sh (notice a positive sign, it means allow access to execute)

I try to change x to something else like y, z, cake, but I got a error from
 chmod, and the operator sign in front of the x, will execute that first.

./McDonald > log.txt (> means overwrite what is in the .txt, but >> append
 in .txt, meaning it won't overwrite, but continue what is in .txt

what is the difference between hostname and uname? 
Hostname shows your computer name or network name for example: 
your computer name is Gnorlia.

so when I type hostname, it will output mac123 because it is the name of the 
device or brand with numbers.

uname shows operating system software-based, if you are using Ubuntu linux or 
Kernal, then it will show the operating system name + information like
version, etc.
)

