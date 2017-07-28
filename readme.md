bdefaultsm css v2.0
==============

in my on-line wanderings i came across a github project called sakura made by a person name oxalorg. the idea being a classless css stylesheet to instantly give style to an html page that had nothing but vanilla html and no classes or ids or anything else

browsers all have this anyway. if you make an html document with text,your browser will style it according to its default values that have been assigned by the humans that make the browser

and i actually kind of like the default (default styles are basically the same from browser to browser)

sakura is an attempt to make a default style that looks a little bit better

the idea appeals to me. if i were developing my own browser and were able to make a default page containing all the typical html elements look however i want, how would i choose to make it look? how should a simple hello world! look?

bdefaultsm.css is my attempt at this

## version 3

i've decided to remove the normalize css file after reading (actually skimming, and maybe i shouldn't be this easily swayed by arguments or maybe it just means i never really liked the idea of using a normalize for this project in the first place and i just did because i thought i should because that's what people do) [this article](https://meiert.com/en/blog/stop-using-resets/)

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