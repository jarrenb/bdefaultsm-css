bdefaultsm css v2.0
==============

in my on-line wanderings i came across a github project called sakura made by a person name oxalorg. the idea being a classless css stylesheet to instantly give style to an html page that had nothing but vanilla html and no classes or ids or anything else

browsers all have this anyway. if you make an html document with text,your browser will style it according to its default values that have been assigned by the humans that make the browser

and i actually kind of like the default (default styles are basically the same from browser to browser)

sakura is an attempt to make a default style that looks a little bit better

the idea appeals to me. if i were developing my own browser and were able to make a default page containing all the typical html elements look however i want, how would i choose to make it look? how should a simple hello world! look?

bdefaultsm.css is my attempt at this

## version 1 -> version 2

at first i thought i'd combine a normalize css sheet with my changes to the sakura css sheet. what i was left with would be an opinionated css reset

i don't think that's a good idea anymore as a reset or normalizer sheet has a different purpose than a classless style sheet. a normalizer is an attempt to fix default discrepencies between browsers, while a classless style sheet is an attempt to add some opinions to how html elements should look

i've decided now to use a normalizer sheet and then build bdefaultsm on top of it. that way, i get the benefits of a resetter or normalizer while keeping my own style opinions separate. this might also encourage anyone looking to do the same to go about it in the same way that i have. css reset work is important, and should probably be separate from establishing default html styles

## opinionated

this is an opinionated thing. i have opinions!

## page width and centering

there are two notable differences between bdefaultsm and sakura (another classless css sheet that caused me to do all this) and i assume other sheets like them

### page width

i've gone back and forth debating whether to implement basically a global max-width on the body or to just specify widths for each element specifically. i've decided to implement widths on elements specifically. i think this leaves documents more flexibility which is ultimately a better thing. for most elements that do have widths imposed, the width will usually be a max-width of 650px. a specific nice thing about not having a global width is that some elements can take up the entire width of the page which can be useful with background-colors or text placement that may need to be the width of the document rather than the width imposed on the body

### centering

this is another issue where bdefaultsm differs from other like sheets. while i do think a nice readable width centered on the page looks nice for many websites, i don't think that's how all websites need to look. i can also think of some reasons why one might want only certain parts of the site centered in the browser while other parts are outside of that centering. i've also seen non-centered sites that i like, and adding centering is not all that hard. just add width and auto margin to the body if you want it so bad. i'm leaving it out of bdefaultsm because i foresee situations in which i might not use it, and would like the choice

## html

the index.html page could also be an example of how i currently think a straightfoward html page should be structured

## typography

### font-size

### line-height

### space between elements