# Sort for Codea

## Description
This project implements 5 different types of sorts using Lua in the Codea environment on iPad.

## Usage
On the iPad highlight and copy the contents of sort.codea. Open Codea and create a new project by press and holding on the `Add New Project` button and then select `Paste into new project`

Codea seemed like a really cool way to write some neat apps for iPad on the go. I had wanted to use it, and learn Lua in the process, for a while now but did not have a project in mind. Then I became inspired by [this](http://m.youtube.com/#/watch?v=t8g-iYGHpEA) YouTube video by andrut where he implemented a number of different sorts and maps sounds to each value.

Figuring it had been a while since I've practiced different sorting methods, I thought I'd take the chance to tackle all of this at once.

This project currently implements bubble, medean, insert, quick, and heap sort. It lets you choose a data set size and to randomize or completely reverse the ordering.

I could have implemented each sort as a class, and at first I did do that. But I was trying to come up with a method for drawing the column highlighting after each "step". That lead me to the coroutine feature of Lua, which seems perfectly designed for these kinds of graphical applications. The yields are placed on the code path in whichever function makes up the meat of the sort, and are intended to run everytime that function is executed.
