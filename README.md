Website Performance Optimization portfolio project-4

The Goal of project-4 is optimize the given website to achieve a pagespeed of 90 in Google PageSpeed insights and for main.js to achieve 60 fps scrolling and 5ms load for size change.

Running the project
Part 1: Optimize PageSpeed Insights score for index.html
Copy the URL http://paramountmedia.us or backup http://paramountgroup.github.io/Project-4
go to the url https://developers.google.com/speed/pagespeed/insights/ and type in the above urls to see results http://paramountmedia.us

The project was uploaded paramountmedia.us and uses Cloudflare CDN services;

Cloudflare accomplishes the following tasks

minimizes css, js and HTML files
send files to browsers using compression
sets cache for static content
uses polish for faster image load time
rocket loader for improve js load
option to set browser caching 1 year

Images were optimized with photoshop and pagespeed insights recommended files

Eliminate render-blocking JavaScript and CSS in above-the-fold content:
style.css inlined in index.html.
print.css with the media=print tag.
Google Tag manager used to report Google Analytics and properly placed in body- as recommended
Load asynchronously the Google Fonts with a script in the footer.
load asynchronously perfmatters.js

Part 2a: Optimize resizing pizzas in pizza.html

Open the URL http://paramountmedia.us or the backup https://paramountgroup.github.io/Project-4 Chrome browser.
Open the Developer Tools and select Console.
Use the slider to resize the pizzas.
start and end time line trace. Observe console.log time
Optimizations:

Took the vars out of the for loop - as recommended by lesson 5
Used document.getElementsById for slider names
Part 2b: Optimize scrolling pizzas in main.js -

Removed the calculation of the items and count of items out of updatePositions so they were not calculated every time throughout the function.
generated the same five values which were always repeating in the longer loop and places them in `constArray`, which holds these five constant, repeating values 
Created global variables ‘items’ to create longer-lived scope..





