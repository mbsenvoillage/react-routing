1) Install React Router
<code>$ npm install react-router-dom</code>
   1) Create components directory
    <code>
      mkdir src/components/Manatee
      mkdir src/components/Narwhal
      mkdir src/components/Whale
      </code>
      
   2) Add Manatee.js, Whale.js, Narwhal.js
    When done, add Manatee.js in App.js and launch server
      
    3) Why React Router ?
        1) You could of course render components conditionally, using state
        2) However, anytime the page is refreshed, user's selection disappears
        3) Furthermore, bookmarking or sharing application state wouldn't be possible 
        4) Router will preserve state and give users a specific URL, that they can share, save etc.
    
2) Adding Routes

    
