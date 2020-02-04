- Write a `checkAuth` function under the approprate comment. Use the `cookie` module to parse the browser cookies and check the `isLogged` cookie. If it has a value, return `true` otherwise return `false`.

- Replace all uses of the `Route` component (inside of Switch) with `ProtectedRoute` EXCEPT for the "/login" route. We always want to be able to access that so leave it alone.

- Upon making the change to `ProtectedRoute` you should notice that you can no longer access any of the links in the navigation bar. They send you back to the login page because there is no cookie available. Let's make sure we set one when we log in.

- Go to the `Login` component (under `src/Login.js`) and look at the login function. There is a comment to add the cookie. Set the cookie equal to the following value: `loggedIn=true;max-age=60*1000`.

- Notice you can now login and access the pages appropriately. We've set an expiration time of one minute on the cookie so go do something else for a minute and then come back to this site. Refresh the page. Were you directed back to the login page?
