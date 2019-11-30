# Welcome to the boilerplate repository for the Advent of Code! 

> :warning: This is a template repository. Edit as you seem fit.

## Brief description

This is a template repository to remove the chore of having to prepare each day before you can start to solve. This boilerplate gives you more time to focus on what you really want to do, solving a fun exercise themed by the festivities.

## Features

 - All of [`aoc-to-markdown`](https://github.com/antonio-ramadas/aoc-to-markdown)

Yup, this is just one application of that script for C++.

## This is set to C++. Is it required?

Nope. Just remove [CMakeLists.txt](CMakeLists.txt), change the contents of [code-boilerplate](code-boilerplate) and you are good to go. Optionally, customise [gitignore](.gitignore).

[`aoc-to-markdown`](https://github.com/antonio-ramadas/aoc-to-markdown) is language agnostic. No need to worry.

If you decide to stick with C++, it is set to C++14 with CMake.

## Organisation

Here is my pick:

```bash
aoc-to-markdown -b code-boilerplate -i -s
```

Copies [code-boilerplate](code-boilerplate) to the respective directory with the input and problem description. There are more options available and I recommend you to know the [available arguments and its usage](https://github.com/antonio-ramadas/aoc-to-markdown#-arguments).

Don't forget to export `SESSION_ID` with the session id you have on [Advent of Code](https://adventofcode.com/). Part 2 of the descriptions and some inputs (in case they are custom) require authentication. You can just copy that cookie. You [can check the source code of the script](https://github.com/antonio-ramadas/aoc-to-markdown/blob/master/aoc_to_markdown.py#L19) to see that nothing funny is being made (like solving the exercises before you do, muhahahah).

## Good luck message

Happy hacking!