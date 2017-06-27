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

## html

the index.html page could also be an example of how i currently think a straightfoward html page should be structured