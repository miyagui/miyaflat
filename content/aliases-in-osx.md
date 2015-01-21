/*
Title: Aliases in OS X
Description: Create your own aliases in OS X
Author: Miya
Date: 2015/01/01
Robots: noindex,nofollow
Template: index
*/

Aliases, introduced to my by counter-strike…

    alias "rs" "sv_restart 5" 
Simple way to have to save time typing. We’re binding the whole sv_restart 5 command to just rs, that’s neat or what.

Same thing here on OSX world. Terminal has the same exact thing and you can even have your own library in case you want to back it up.

Your `~/.bash_profile` is your own little place for aliases. If you don’t have it yet you can type this on your terminal:

    touch ~/.bash_profile 
    
Now edit it with your favorite text editor. Right now I’m using brackets and sublime text and want them both aliased so for brackets for example.

    open ~/.bash_profile -a brackets 
    
This simple command will tell something like. Hey command you to open a file in the user’s home directory `~/`. There’s a file called `.bash_profile` (. makes the file hidden), using the application `-a brackets`. `-a` is an option for the open command that lets you use an application to open the file with.

Now all you need is to add your aliases to your     `~/.bash_profile`, mine is looking like this.

    alias st='open -a "Sublime Text"' 
    alias bra='open -a Brackets'

Refresh this newly created profile by using

    source ~/.bash_profile 
    
to try my aliases you could use st or bra on the terminal followed by the name of the file. At least for brackets it’s one of the few ways to get it down since it doesn’t have a command by it’s own. Sublime text does though I will implement it if I need to, probably I do since I’ve yet learned how to use nano. I’ll leave you with a nice function for your `.bash_profile`

    function cdl { cd $1; ls; } 

Salu2