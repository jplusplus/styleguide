# Best practices and coding rules

This guide aims to define the rules and good practices of programming within
Journalism++ projects. The content of this guide is under MIT licence.

## <a name='TOC'>Table of Contents</a>
  1. [Projects installation](#installation)
    2. [README](#readme)
    2. [Configuration files](#configuration)
    2. [Dependencies](#dependencies)
  1. [Comments](#comments)
    2. [Be a storyteller](#storyteller)
    2. [Every developer is different](#different)
  1. [Text editor](#editor)
  1. [Languages](#languages)
    2. [Javascript](#javascript)
  1. [Issues : The boy who cried Wolf](#issues)


```                               
          .=.,   
         ;c =\   /_ Comment is free, but indents are sacred.
       __|  _/     
     .'-'-._/-'-._
    /..   ____    \
   /' _  [<_->] )  \
  (  / \--\_>/-/'._ )
   \-;_/\__;__/ _/ _/
    '._}|==o==\{_\/
     /  /-._.--\  \_
    // /   /|   \ \ \
   / | |   | \;  |  \ \
  / /  | :/   \: \   \_\
 /  |  /.'|   /: |    \ \
 |  |  |--| . |--|     \_\
 / _/   \ | : | /___--._) \
|_(---'-| >-'-| |       '-'
      /_/     \_\
```

## <a name='installation'>Projects installation</a>

You must always work under the assumption that your project will be open
source. The difference between a good programmer and bad programmer coming
from its capacity to work in a network. Your code must be addressed to the
community, systematically.

### <a name='readme'>README</a>

Every new projet **starts by the creation of a README file**. This file
details at least :

  - Installation process : any new developer should be able to install the project from scratch;
  - required environments variables;
  - required programmes and dependencies;
  - licence of the project.

### <a name='configuration'>Configuration files</a>

Most modern languages offer tools to manage different configuration files. Pay
attention to :

  - Split information that allow the programme to work from the credential values (such as authentication key, etc);
  - **place systematically files containing passwords into .gitignore** to avoid to communicate those to malicious people;
  - create templates files for these "ghost files".

### <a name='dependencies'>Dependencies</a>

Python and NodeJS both use very smart package managers. With smart tools,
smart practices come along :

  - Detail every dependencies into a file that your package manager can read (Pip, NPM, etc);
  - give the highest priority to the last version of a dependence;
  - never, ever, use a deprecated or poorly documented dependency;
  - if you are not sure to be able to maintain the project, use fixed version numbers rather than aliases to the last versions (Good : "2.0.1", Bad : "latest").

## <a name='comments'>Comments</a>

### <a name='storyteller'>Be a storyteller</a>

A beautiful algorithm is designed like a beautiful story. Unfortunately, it's
not always easy to distinguish every key events in a story, and it's even more
complicated when this story is written with code. Do not be just a good
author, be also a good storyteller.

### <a name='different'>Every developer is different</a>

Never forget that the developers won't be necessary at the same level of
knowledge than you:

  - Take the time to explain your choices; 
  - make sure to explain clearly when you use complex expressions;
  - insert links to documentation or Stack Overflow when you solve a problem that troubled you for hours.

## <a name='editor'>Text editor</a>

We are not offended if your prefer TextMate or Netbeans rather than the great
and unrivaled **Sublime Text 2**. Most important is that your project can be
opened with any text editor which is not yours and without prior configuration
(so most IDEs are out of the table).

  
From now, configure your editor to:

  - Use 4 spaces indentation (never mix up spaces and tabulations);
  - always save in UTF-8;
  - use UNIX line endings;
  - give priority to middlewares rather than executable pre-processors to compile your assets (like Less, SCSS, minfiiers, etc).
  - add two rulers to your editor. The first at 80 characters: try not to exceed it. The second at 100 characters: **never exceed it**.

## <a name='languages'>Languages</a>

### <a name='javascript'>Javascript</a>

Javascript just got out of a long and painful teenage angst. It is today at a
certain level of maturity that the good practices of programming maintain. To
avoid going backward, we have to be very rigorous with Javascript. The
language's permissiveness will not force you to do so, so you'll have to apply
yourself.

For theses reasons we encourage you to follow the comprehensive [Javascript
Style Guide](https://github.com/airbnb/javascript) provided by Airbnb.

## <a name='issues'>Issues : The boy who cried Wolf</a>

Do you know the fable of [The Boy Who Cried Wolf](https://en.wikipedia.org/wik
i/The_Boy_Who_Cried_Wolf) ? It's about a little boy who
amuses himself by crying "wolf" in order to see the panic he causes in its
village, but consequently does not get help when a real wolf appears and eats
half of a flock of sheep.

Do not cry wolf too if you want to see the true issues solved. You may also
follow the excellent [Issues Guidelines](https://github.com/necolas/issue-
guidelines) by Nicolas Gallagher.

