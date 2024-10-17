---
layout: default
---

# Overall Introduction to the Course

In this course, I have explored the command-line environment of WSL (Windows Subsystem for Linux) and learned to use its many tools to streamline my work. Every week, I read and watched course materials to master different pieces of knowledge about the command line. By finishing weekly assignments, I am more familiar with the command line environment by hand-on practice.

In the following sections, I will introduce what I have learned each week in this course in detail.

# Week 1: Introduction to Command Line Environments

In the first week, I attended the introductory lecture where some basic knowledge is displayed. We watched a video about how computers work, and then learned about what an operating system is for. Computers can do multitasks at the same time because of the functionality of processes and CPU. Memory management and file systems are also introduced.

After setting up the command line environment, some basic tools are introduced in the course materials. For example, `cat some_file.txt` can display the content of a file, `mkdir KIK-LG221` creates the course folder, and `nano call_of_the_wild.txt` opens an file editor for users to do some text processing work.

This week's learning makes me more familiar to the setting up of an Linux environment in the Windows system. When I was previously introduced to Linux, I was taught to install an virtual machine in a complex way. In this course, if only the command line needed, WSL is a much convenient way to use Linux.

# Week 2: Navigating a UNIX System

In this week, I was taught to manage processes in Linux and to work on a remote machine via the commands `ssh` and `scp`. When running programs by default, the corresponding process will stay in the foreground. By adding an ampersand (&) after the command, the process then can run in the background. Background processes can be terminated by the command `$ kill -9 <BASH_PID>`.

This week's practice let me try to run programs on a remote server. CSC Puhti is a good platform to use when extra computing resources are needed.

# Week 3: Basic Corpus Processing

Text processing tools in Linux is introduced in this week. The most flexible tool used this part is regular expressions. By writing simple strings, complex and repetitive text segments can be matched for use. Here I list some core characters used in this tool.


| Symbol | Meaning |
| --- | --- |
| ^ | start of string |
| $ | end of string |
| * | 0 or more |
| + | 1 or more |
| ? | 0 or 1 |

The text processing tools involved this week is listed below:

- `tr`: translates or deletes characters;

- `head`: displays the beginning part of a file;

- `tail`: displays the ending part of a file;

- `grep`: searches for a specified string in files and returns the matching lines;

- `egrep`: extends the function of `grep` by supporting extended regular expressions when searching text;

- `wc`: counts the number of lines, words, and characters in a file.

The tools used this week need to be practiced more to get mastered, and I gradually handled them in the next few quizes.

# Week 4: Advanced Corpus Processing

Corpus processing is still this week's topic, and more tools are introduced, for example the command `sed`, which is a powerful tool that can perform various text manipulations such as searching, find-and-replace, inserting, and deleting.

When finishing the quiz of this week, the `diff` command is also used to see the differences between two files.

This week let me try to compose long commands by using the symbol `|` as the tube, which accepts the result of the previous tool and sends it to the next one as the input. This kind of progressive exercise is very helpful.

# Week 5: Scripting and Configuration Files

In this week, complex Linux scripts are learned by us. The following script takes one argument, an English adjective and prints its comparative form.

```
#!/bin/bash

# Check if an argument is provided
if [ -z "$1" ]
then
  echo "Please provide an adjective."
  exit 1
fi

adjective=$1

# Append 'er' to the adjective
comparative="${adjective}er"

# Print the comparative form
echo "$comparative"
```

The grammar of Linux scripts is similar to some programming language but much simpler.

The tool `chmod` is also introduced. It can control the permissions to read, write and execute files.

I think this part needs more practice after class because composing Linux scripts can be very useful when doing some automatic tasks.

# Week 6: Installing and Running Programs

`sudo apt-get` is used to install additional programs into our Linux environment. `make` is used for building other programs, libraries or other projects like corpus collections.

In the quiz part, the package `bllipparser` is quite interesting for converting a sentence into a grammar tree.

This week, I think the `make` command is very powerful to complete multiple tasks at one run.

# Week 7: Version Control

This week mainly focuses on the version control tool: git. Common commands about git is practiced, such as `git clone`, `git commit`, and `git push`. The most popular platform providing git tool support - GitHub - is also well introduced.

The following picture clearly shows the workflow of git:

<img src="https://preview.redd.it/nm1w0gnf2zh11.png?width=1080&crop=smart&auto=webp&s=f793be53fbc0246cecc4d865b2ea479d5ea57e94" width="80%" />

The most useful this week for me is the practice of git command line. In practical use, I often use graphical git tools and this week's quiz helps me to recap the command line version of git.

# Final Week: Building GitHub Pages

In the final week, GitHub Pages and the Jekyll tool is introduced to build a webpage. By using Jekyll, we can easily build a static webpage by writing markdown files.

In this week, the command `bundle exec jekyll serve` is the most frequently executed one because I need to check the result after editing.

This week, I also used Latex to compose a CV for myself, which is quite a good practice of practicing Latex grammar when making printable files.

