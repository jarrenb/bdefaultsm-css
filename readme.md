bdefaultsm css v3.0
==============

in my on-line wanderings i came across a github project called sakura made by a person name oxalorg. the idea being a classless css stylesheet to instantly give style to an html page that had nothing but vanilla html and no classes or ids or anything else

browsers all have this anyway. if you make an html document with text,your browser will style it according to its default values that have been assigned by the humans that make the browser

and i actually kind of like the default (default styles are basically the same from browser to browser)

sakura is an attempt to make a default style that looks a little bit better

the idea appeals to me. if i were developing my own browser and were able to make a default page containing all the typical html elements look however i want, how would i choose to make it look? how should a simple hello world! look?

bdefaultsm.css is my attempt at this

## colors

the browser has default colors and they're good, but they're not what i want

[clrs.cc](http://clrs.cc/) is a nice starting point for default colors. i will use them for now and update them as i see fit

## for a future version of this more useful than i expected tool

having a catch-all css stylesheet doesn't really make sense. i may not need or want form styles on my page if my page doesn't have any forms. i do like the idea of classless styles, but only when i need them. so i think for the next version of bdefaultsm, i'll try and implement some of the ideas that come from an attempt to make bdefaultsm more modular. i like the idea of if i add a p tag to some html, then maybe a bdefaultsm script automatically adds its p styles to my stylesheet; and vice versa: if i remove the last p tag from my html, bdefaultsm knows i don't need those sweet sweet p styles anymore and removes them automatically from my stylesheet. i may not have the skillz to implement this until much farther down the road, but it's a cool goal to set i think

## version 3

i've decided to remove the normalize css file after reading (actually skimming, and maybe i shouldn't be this easily swayed by arguments or maybe it just means i never really liked the idea of using a normalize for this project in the first place and i just did because i thought i should because that's what people do) [this article](https://meiert.com/en/blog/stop-using-resets/)

i've switched all "em" units and "px" units to rem and set the font-size of html to 18px because 18px is dope

## opinionated

this is an opinionated thing. i have opinions!

## page width and centering

before, i didn't have a maximum page width and centering. but now i do because after a certain width, it just feels right. maybe i'll get rid of it again in the future, but for now it's in

## html

the index.html page could also be an example of how i currently think a straightfoward html page should be structured

## typography

### font-size

### line-height

### space between elements

### lists

when i write lists by hand, i bullet them with a hyphen. the same goes for markdown. i've never taken the time to fill-in a little circle to make a bullet point when i make a list. so, since this is an opinionated stylesheet, i've decided to make unordered lists have a hyphen instead of a bullet point