challenge
=========

I have posted this code at [http://standardguy.net/lsc/ls_deal.html] http://standardguy.net/lsc/ls_deal.html

Discussion
----------
I decided to use JQuery and a very reduced Bootstrap for this exercise.  This was a tough decision for me.  I understand that a page as simple as this does not require the overhead both of these libraries bring with them, but I also suspect that part of this exercise is to illustrate some familiarity with common frameworks used today.  I have decided to use the minified version of the widely available code frameworks I have implemented, but to keep my custom JS and CSS uncompressed for your reading pleasure.

I used HTML5, but again the simplicity of this page does not require a sophisticated DOM.  I included meta tags for SEO, as well as semantic and valid markup to aid in basic accessibility. I assigned some ARIA roles to the major DOM elements, in an attempt to provide clarity for screen readers, but I am sure more could be done here.

I used straight CSS, though my preference is to use either SASS or LESS. For the custom CSS that I wrote validation errors will show due to references to proprietary browser features (i.e. -moz-border-radius).

My testing included IE7+, chrome, safari and firefox.  I checked for graceful degradation and worked towards keeping my markup dry by using AJAX calls to dynamically populate the view with content from the static fallback pages I put together.

I tried to keep the overall page footprint small by creating a image sprite for layout images and a moderately compress jpeg for the background. I also tried to load addition content to the main view only when it was requested. Each tab and link will generate an AJAX call that will deliver content from fallback pages. Naturally, I grouped my all the CSS and JS into one file to reduce the number of server calls.
