qode is a new programming language with easy commands

how to run?:
in cmd you write "qode filename.qd"

#get -- command that imports an extension
There is args that does not need #get command

No #get list:
showtext("message") - Print text

input=("prompt") - Get user input

if true: ... end true - Infinite loops


#get list:
cmdact
lineage
gui
ynoption
maths
time
weblib
dimgr

cmdact is argument that works with batch files inside .qd file
example:
cmdact """
echo hello qode
"""
Output: hello qode

lineage is argument that doing visual install but not installing anything
set.line.long = Xs
where X stands for a number and going from 0 to 1000
example:
set.line.long = 5s
output:
=============-----50%

gui is windowed interface, in act() can be anything from other #get
example:

showtext("Creating GUI window...")
gui.create.window
gui.size(400x300)
gui.showtext("Welcome to Qode GUI!")
gui.showbutton("Exit Button")
gui.button.prop: showtext("Click to Exit")
gui.button.prop: act(exit)

gui.showbutton("Run Command")
gui.button.prop: act()


ynoption is y/n argument
if y written then app continue to work
if n written then app is not working
example:
ynoption: do you want to run this app?
output:
do you want to run this app?
y/n:

maths is arg that uses maths technologys
therefore, there's three args
example:
showcalc(basic)
output:
Write your number and sign: 2+2
result=4

example:
showcalc(extended)
output:
Extended Calculator Mode
Available operations: +, -, *, /, ** (power), sqrt (square root)
Example: 2**3 (2 to power of 3), sqrt(16) (square root of 16)
Powers: 2^3 (use **), 2^4, 2^5, etc.
Square root: sqrt(number)
Enter an extended mathematical expression:

example:
showcalc(gui.windowed)
output:
opens in gui window (powered by customtkinter)

time is arg that can stop time for a few or more m,s,h,etc
example:
sleep.for(5)

weblib is argument that allows to open or search in browser
you need to #get something from there, only two now available:
#from weblib get webbrowse --browse link
#from weblib get webcontrol -- opens browser
example: webbrowse.link: https://github.com

dimgr is download install manager
it install file in folder with code
as shown in example, we show .qd file buy it dont have to be .qd, it can be exe or other files
example:
dimgr.download.fl=https://example.com/filename.qd
output:
file appear in folder
example:
dimgr.install=filename.qd
dimgr.install.cf=filename.qd
output:
file opens
