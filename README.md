# better-twitch-dark
A better Twitch Dark optimization

# Steps
* Turn Twitch into dark mode (if not already the case)
* Put into the URL this snippet (Watch out, `javascript:` gets removed when copy/pasting) : 
`javascript:(function(){s=document.createElement('style');s.innerHTML=':root{--color-twitch-purple-1: #212126;} .tw-root--theme-dark .chat-room,.tw-root--theme-dark body{background-color: var(--color-twitch-purple-1);} .tw-root--theme-dark .side-nav{border-right: 1px solid #000000;} .tw-root--theme-dark .right-column{border-left: 1px solid #000000;}';document.body.appendChild(s);})()` and press `Enter`.

* Or execute this in the console:
`
function restyle(){s=document.createElement('style');s.innerHTML=':root{--color-twitch-purple-1: #212126;} .tw-root--theme-dark .chat-room,.tw-root--theme-dark body{background-color: var(--color-twitch-purple-1);} .tw-root--theme-dark .side-nav{border-right: 1px solid #000000;} .tw-root--theme-dark .right-column{border-left: 1px solid #000000;}';document.body.appendChild(s);}
restyle();
`
* Enjoy a more readable chat reading experience

