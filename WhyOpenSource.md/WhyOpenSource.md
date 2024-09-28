# TOC #

<!--TOC-->




----

# Initial Notes #


We’re here to create a little “book”, showing how to create the GitHub pages you will be reading when this is all done. This chapter starts at the beginning, though it may not wind up being the first page of the “book”.
I’ve just started with a blank Scrivener project, which I named “GitHub-Pages” and saved in Dropbox/Apps/Scrivener, where my shared Scrivener projects live.
Right now, what I see on the screen looks like this:


----

# Default Formatting #

Default Formatting
You set your initial font and paragraph info in Scrivener > Preferences, (command-comma). My info looks like this:
![][ScreenShot2018-06-15at35655AM]

To change that information, you can click the controls at the top of the paragraph, for example, to show the fonts panel:

![][ScreenShot2018-06-15at35933AM]

I could change the face from Arial if I wanted to. I don’t. I am going to turn off the Show Invisibles, however.
Note in the Formatting window above that the two paragraphs, the quotation and the name, are adjacent. When you’re on that window, you could use Format>Paragraph>Line and Paragraph Spacing to put some inter-paragraph spacing in place. I don’t do that, because Markdown requires explicit blank lines between paragraphs, so making fake ones would just confuse me. If this paragraph confuses you, pretend you didn’t read it.


----

# Styles #

Styles
Scrivener lets you assign “Styles” to paragraphs, and you can control how those styles get compiled into the output. So, in principle, I could set up a “Heading 2” style such that when I format a paragraph with Heading 2, it would look different in my editor, and (I believe) I could make it compile with the ## in front of it that signify H2 to Markdown. For now, I’m not going to do that: I’m going to type my own Markdown marks, because I’m used to it.
Perhaps we’ll come back to the topic of styles, for now, let’s move on …


----

# Sections #

Sections
Next, I’m going to set up my “book” chapter and section information. I have in mind a very simple structure: A document at the top level of Scrivener’s binder, like this one, will be a “chapter”, represented as a single GitHub page. In principle, that would be all you need.
However, Scrivener has this really nice cork board feature, where you can put virtual index cards down, each one representing a document, with the document title, and a synopsis, where you can write on the card what a proposed document will be about. You can see the card for this document in the top right of this picture:
![][ScreenShot2018-06-15at41513AM]

Because I plan to use the cork board to organize this little book, I want to allow for a bit more structure than just documents at the top. I’d like to organize a few cards into a chapter, so my rule will be that a folder at the top level also represents a chapter, and documents inside that folder represent text inside that chapter. So, if a chapter has three ideas in it, there might be three cards representing those ideas, and then each card’s document would have some paragraphs about that idea.
Why do we care? Well, we’re getting ahead of ourselves a bit, but I have learned enough about Scrivener’s compile to think that I’d like my chapters, when compiled, to automatically include the chapter Title from the binder, as their heading. But for ideas within the chapter, I expect not to include the card title, instead leaving the idea transition and any subtitling to manual editing.
I could do all the titling manually, and in the end I may prefer that. But I’m trying to give Scrivener every chance to work for me, so I’m planning to use that much structure.
Let’s talk about how that has to be set up.


----

# Documents, Sections, Layouts #

Documents, Sections, Layouts
Warning: I’m going to get the terms wrong here, but I’ll do my best to correct to Scrivener terms.
Each document in Scrivener is a “Section” and has a “Section Type” for compilation. Associated with each Section Type, there is a “Layout”, which tells Scrivener how to format the compiled output for that section. We’ll use that to control what comes out, to be fed into GitHub Pages.
You could do this incrementally, or later, but I think it’s best to set up our initial Section Types now. We’ll have two, initially, which I think I’ll call Section, and Sub-Section. We’ll set them up to be auto-assigned: top level documents and folders will get Section, documents at the next level down will get Sub-Section.
You set this up in Project > Project Settings, in the Sections tab:
![][ScreenShot2018-06-15at43151AM]

I’ll use the plus and minus buttons to create mine:
![][ScreenShot2018-06-15at43300AM]

Then we go over to Default Types by Structure to tell Scrivener about our folders and sub-documents. It starts like this:
![][ScreenShot2018-06-15at43419AM]

That’s not what we want, quite. We’ll use that +levels button to provide more levels for files, and fill that in:
![][ScreenShot2018-06-15at43550AM]

I think that should do the job for us. Root files is like where Scrivener’s Draft and Research folders are. Level 1 is documents like this, and Level 2 will be documents inside folders.
We’ll worry about layouts pretty soon. I want to think a bit now about what else to put in this little book, and how to organize it. I may even be regretting the simplistic section layouts we just did, but I know it’s easy to change.


----

# Regrets, I’ve had a few #

Regrets, I’ve had a few
Since I mentioned regrets, and since I always do “Programming in Public”, or in this case “Scrivening in Public”, here’s what’s on my mind. I’m going to start creating a few index cards on the cork board, to get a general idea of what might be in this little book. And it becomes clear right away that those ideas will fall into classifications, and some of them could be quite large.
For example, we may have some ideas about compiling to markdown. We may have some discussion about the details of layouts and prefixes and suffixes. We will surely talk about how to split the compiled document into bits, and we will probably do that manually at least once and then write a little script to do it and then embed that script into the Scrivener compilation.
I can imagine that this may mean that this little book will have sections, each section containing chapters, each chapter containing some kind of sub-documents like our current Sub-Sections. Maybe three levels instead of two.
We can change that setup at any time but it always seems best to get it right at the beginning, especially when we don’t know our way around the framework all that well. But I have enough experience with Scrivener to feel sure that we can’t get in too much trouble if we don’t do anything too radical. So we’ll let it ride. I do think I’ll create a folder and then test a compile.


[ScreenShot2018-06-15at35655AM]: ScreenShot2018-06-15at35655AM.png

[ScreenShot2018-06-15at35933AM]: ScreenShot2018-06-15at35933AM.png

[ScreenShot2018-06-15at41513AM]: ScreenShot2018-06-15at41513AM.png

[ScreenShot2018-06-15at43151AM]: ScreenShot2018-06-15at43151AM.png

[ScreenShot2018-06-15at43300AM]: ScreenShot2018-06-15at43300AM.png

[ScreenShot2018-06-15at43419AM]: ScreenShot2018-06-15at43419AM.png

[ScreenShot2018-06-15at43550AM]: ScreenShot2018-06-15at43550AM.png