# nextjs-hmr-bug

Project to demonstrate an error when clicking on a link in next.js in dev mode.

# How to reproduce

* `npm i`
* `npm run dev`
* navigate to http://localhost:3000/
* click on the link

In this branch, the export `SomeType` has been removed from `src/types.ts`, which results in the bug not occuring.
