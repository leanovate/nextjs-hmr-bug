# nextjs-hmr-bug

Project to demonstrate an error when clicking on a link in next.js in dev mode.

# How to reproduce

* `npm i`
* `npm run dev`
* navigate to http://localhost:3000/
* click on the link

Notice that after reloading the linked page once, the error is gone.

# Other branches

There are three other branches:
* `fix-by-removing-export` demonstrates that the bug can be avoided by removing an interface export in `src/types.ts`
* `fix-by-removing-sass-import` demonstrates that the bug can be avoided by removing the import of the `about.scss` file
* `break-by-removing-css-import` demonstrates that removing the import of `index.css` will break the link. Clicking will have no effect. Maybe it is related to the hmr bug.