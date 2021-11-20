### Welcome to my GitHub profile folks 👋

A bit about me
===

- :house_with_garden: Living in Melbourne, Australia :australia:
- :man_technologist: Senior Web Developer at Cassette Agency
- :artist: Web and Graphic Design background, which I bring to my development to help bring designs to life in a way that not only matches the designers intent to a very high level, but I aim to interpret and add value to the design through the responsive development process.
- Proud fur-dad :dog:
- I speak English :gb: and Thai :thailand:
- Lover of :coffee: :tumbler_glass: and :flight_departure:


:hammer_and_wrench: Tools of the trade
===
- Vue.js
- SCSS, CSS
- ES6 JavaScript, jQuery
- PHP
- HTML5
- Headless CMS
- Wordpress Custom Theme & Plugin Development

:memo: Code Style
===

I do a few things differently from the rest of the dev world, so before you :fire: me, let me explain why!

* `__` double underscores within class chains, such as `.parent-component__child-component`. I hate these personally, as underscores prevent you selecting along word boundaries in your IDE. Especially since the double underscores usually sit in the exact spot you *might* need to select on word boundaries in your templates (i.e. the child part of a class chain), to select and edit/replace part of a class name without using your mouse.  I use double dashes or `--` instead. Accomplishes the same separation of concerns as `__`, without impeding your dev workflow.
* Let's also talk about REM units. We all know they're the best units for type, but 1rem = 16px is not a useful conversion *at all*, and most of the workarounds for this that I've seen, frankly, suck. Mixins that convert pixel values in your SASS to arbitrary REM units in the compiled CSS impede dev QA because you're not tweaking the same units in the inspector. The only solution I've seen over the years that makes sense is `html { font-size: 62.5%; }`. This converts your REM units to **1rem = 10px**. A great starting point for sensible font size values that are identical in build and QA.
* Media Queries via mixins. I don't personally choose to do this, which some may find an out-of-date approach. The only reason for this is in case I need to chain media queries like (min-width) and (max-width), I'd then have to manually write that whole query. So instead, I just have shortcuts setup in my IDE (VScode), so that when I type `@<` or `@>` the IDE outputs `@media (min-width: $) {}` or `@media (max-width: $max-) {}` respectively.
