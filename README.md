# All the colours all the time

I was looking at the output "git log" one day and it dawned on me that it was using `less` and that it was showing colours. I'd never thought about less supporting colours before, but here we are.

I can't say how many times I've done `grep foo bar` and realized I want to page through the output, piped it through `less` and deep down felt a little sad that I no longer had the colours from `grep`s output. No more.

Also, same thing if I'm e.g. doing `grep this_one_thing | grep but_also_this_other_thing` and I lose the highlights from the first grep. So frustrating. No more.

I shove this script in $HOME/bin/grep, set `LESS=-R` in my `.bashrc` and now grep and less have all the colours at all the right times. And when I'm piping the output someplace else, we skip the colours. Cool, huh?
