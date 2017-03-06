So you'd like to contribute? Woo!

Here's a checklist you might find helpful. Follow these points and your
code will find it easy to get merged into Highland.


Setup the Environment
---------------------

- npm install


Code changes
------------

1. If the change is big or might need discussion first, make an issue so we
   can talk it through
2. If you're picking an existing issue, add a comment saying your working
   on it so someone else doesn't jump in
3. Add tests for your code
4. Run 'grunt test' before sending a pull request - fix any lint errors
5. Do NOT rebuild dist/highland.js or docs/index.html (this happens when
   you run 'grunt' or 'grunt watch') - they'll just clutter up your pull
   request
6. Update `CHANGELOG.md` with some information about your change. A one line
   description with a link to the PR (and bug if applicable) will suffice.
7. Send a pull request \o/


Running the tests
------------

To run the linter and nodeunit tests in Node.js, use the grunt task:

    grunt test

To run tests in a browser, first build the browser-test bundle.

    grunt build-browser-tests
    # now visit test/browser.html in your browser

Editing docs
------------

- If you want to change something in the Intro/Examples sections, then
  take a look at `docs/templates/base.html`
- If you want to change API docs (after the Streams heading), they are
  generated from comments in the source code - click the 'source' link
  next to the function and it'll show you where in the file to edit
- To view your changes run `grunt docs` and open up `docs/index.html`
- When you send a pull request please DON'T include the generated
  `docs/index.html` file, it will just clutter up your pull request
