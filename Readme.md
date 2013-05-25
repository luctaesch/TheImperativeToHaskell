This are the sources for the book "The Imperative To Haskell".

You can benefit get involved at

## 0.Reading ##

- read the pdf in  [dist/the imperative to haskell.pdf](https://github.com/luctaesch/TheImperativeToHaskell/blob/master/dist/The%20Imperative%20to%20Haskell.pdf)
- if you would like to provide feedback , just email me at luc.taesch+tith@gmail.com

## 1. Commenting ##

- you become a regular reviewer ? 
	- use the list  the-imperative-to-haskell@googlegroups.com
	- subscribe to the list the-imperative-to-haskell+subscribe@googlegroups.com (tbc?)
	or 
	https://groups.google.com/d/forum/the-imperative-to-haskell

- you will be able to see others opinions, and share ideas with the group
- you will be mentionned as commenter in the book

## 2.  Reviewing ##

- you want to display your comment,  directly in a piece of text ?
 - get the Markdown fragment and mail it to the list, as attachement 
 	- get the Md from : https://github.com/luctaesch/TheImperativeToHaskell/tree/master/src/MdSync/Draft
 	- more info below 

 - you do this regularly , or with many files ?
     -  do a pull request 
     	- how : https://help.github.com/articles/creating-a-pull-request
     	- about: https://help.github.com/articles/using-pull-requests

- you will be mentionned as Reviewer in the book

## 3.  Contribute  ##

- you want to contribute examples, or complete pieces of text ?
- one off or occasionally  ? send it to the list as attachement

- regularly ? 
	- use github pull request as the reviewer

- you can pick some work from the plan ( and let us know on the list)
	- the plan is here ( tbd) 

- you will be mentionned as contributer in the book

## 4.  Contribute a Lot ##

- you want to contribute a full section, or several chapters ?

	- use github pull request as the reviewer

- you can pick some work from the plan 
	- the plan is here ( tbd) 
	
- you will be mentionned as co author in the book

## Content ##


Currently, the organisation is as follow:

- src/ : the source directory
	- the imperative to haskell.scriv : the Master file in [scriverner] 
	- mdsync / : the directory of txt source files, synced with the scriverner master . these are Markdown file 

- dist :  the output of the compiled scrivener file.
	- current generated format : PDF	

- build : should we need some auto build  ( from md/ xsl / whatever), this will be there.
	- 	empty for now.(tbd)

-  theRoadToTheImperativeToHaskell.taskpaper is a task list and journal of the making of (text file)

- the plan and work in progress is here (tbd)


---
## Status ##
- the status of the sections is in : tbd
- no plan has been established firmly
- as long I am the only active contributor, I progress ad-hoc
  the intro should get the general ideas.
	- when someone fancy joining, I'll put the synposis in approach and plan in written.

### Sync ###
- the master is the scrivener file (owned by luc taesch, however shared)
- the PDF is generated , generally at the end of every session (typically after my daily commute : 9 am , 8pm )
- the md is synced automatically at every open/close of scrivener . (which may stay open for one or two weeks:-) / . and on demand;
- the git sync  is currently manual. daily evening.

when contributors will become active, or request it, I'll sync to MD and git push bi daily. for now, this is ad hoc.

## Contribution ##

- whoever fancy contributing is welcome. 
you can contribute comments, detail reviews or content, new or updates.
- the mailist is there to share and provide archive. 
- the md directory enable to do direct modification of the content.
	- how: clone the github epo.
	- do the modif on your repo
	- push it to me	 


## Toolset

scrivener is used for the master assembly, and the plan management, 
( note :scrivener files can be viewed directly using [Marked] ( drop on it) ( is a directory packaged in fact).
scrivener generate the pdf , latex , MD, ...

you do not need scrivener to contribute. just read the pdf, of use the Markdown files


[Scrivener]: 
[Marked]: 

# Licence

This work , the imperative to haskell of Luc Taesch, is licensed under the Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-nd/3.0/ or send a letter to Creative Commons, 444 Castro Street, Suite 900, Mountain View, California, 94041, USA.