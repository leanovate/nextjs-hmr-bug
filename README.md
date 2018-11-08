# nextjs-hmr-bug

Project to demonstrate an error when clicking on a link in next.js in dev mode.

# How to reproduce

* `npm i`
* `npm run dev`
* navigate to http://localhost:3000/
* click on the link

In this branch the import of `index.css` (and the corresponding loader) have been removed, which results in the bug not occuring. This also breaks the link. Clicking on it will have no effect.
