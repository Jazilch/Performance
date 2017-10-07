# Performance


This document is to due with Performance of our current jQuery Plugins. As you know we use multiple jQuery plugins. Match Heihgt, Isotope, Infinite Scroll. While these files seperately aren't very large files but once you start putting them together you might see some performance issues with your blog. 

In one blog we might be using Images Loaded to wait for all of our images to load. Then we could also be running Match Height in order to match the heights of all of our Post Items. Most of our layouts include Isotope in them so that bring us to three and then add in an infinite scroll into the page and it starts to be very heavy. 

How should we keep an eye on this. If the page becomes too heavy there are a couple items we can do in order to increase page speed. 

1. ) Make sure all JS files are minified
2. ) Combine multiple JS files into one. This will ensure we only have one file to load to reduce the amount of page requests. See my Webpack Concat Folder
3. ) Initialize plugins with Javascript vs. jQuery. Javacript is faster than jQuery as when most people are writing jQuery they tend to get sloppy and jQuery makes it easy to call DOM elements over and over. 
