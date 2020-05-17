# express-babel-template

This repo is meant to be cloned as a starter template for a new Express project. This is based entirely on [this guide](https://www.freecodecamp.org/news/how-to-enable-es6-and-beyond-syntax-with-node-and-express-68d3e11fe1ab/) to setting up Express with Babel for transpiling ES6. It includes nodemon for convenience, and Jest for testing if you so desire.

To start a new project using this repo:

1. Create a new repo in your own GitHub account.
2. Clone this repo.
3. At the root of this cloned repo, run `git remote set-url origin your.git.url/here`.
4. Verify that the new origin is set to your repo with `git remote -v` (should print your.git.url/here).
5. Run `npm i`.
6. Run `npm run`.
7. Open [http://localhost:3000/](http://localhost:3000/) and verify that you see the boilerplate html from [public/index.html](public/index.html).
8. Change the name of the project in package.json and package-lock.json from `express-babel-template` to `your-project-name`.
9. Add/commit/push and you have the makings of a new project, enjoy!

Notes:

-   You can remove or modify the .eslintrc file if you don't use eslint or you already have these options set globally.
-   I try to keep my stuff up to date, but can't promise this will always be vulnerability free. If you don't already know about [npm audit fix](https://docs.npmjs.com/cli/audit), check it out, it is a huge timesaver.
-   The Jest test script is optional, if you are not writing tests for your project, you can
    -   run `npm uninstall jest --save-dev` to remove the package from the project
    -   delete `"test": "jest"` from the package.json scripts,
    -   and delete these lines from package.json as well:

```json
"jest": {
    "testEnvironment": "node"
},
```
