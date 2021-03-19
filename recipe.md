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
    1) Import BrowserRouter, Route, Switch from react-router-dom
    <code>import { BrowserRouter, Route, Switch } from 'react-router-dom';
       </code>
    BrowserRouter creates a base router. Anything outside of it will appear site-wide.
    Switch is like a switch statement and will activate the route typed in the url. Each url is represented by a Route
    with the url as "path" parameter.
    <code>
    \<BrowserRouter>
       \<Switch>
        \<Route path="/manatee">
            \<Manatee />
        \</Route>
         \</Switch>
    \</BrowserRouter>
    </code>
    2) Add "exact" prop to "Route" if you want page to show only if url completely matches
    3) Import Link from 'react-router-dom'. This components replaces \<a> element 
    to make sure that pages do reload on click.
    <code>
       \<li>\<Link to="/manatee">Manatee\</Link>\</li>
        \<li>\<Link to="/narwhal">Narwhal\</Link>\</li>
        \<li>\<Link to="/whale">Whale\</Link>\</li>
    </code>
3) Access Route Data with Hooks

    

    
