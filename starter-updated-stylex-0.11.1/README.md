## Demonstration of Failure With Next.js Project with Version of StyleX Greater Than 0.2.0-beta.27

See discussion here: https://github.com/facebook/stylex/discussions/660

Versions of StyleX after 0.2.0-beta.27 need to have @babel/runtime installed.  

In the case of this project it is using version 0.11.1 of StyleX and does **not** have @babel/runtime installed.  The fix is to install @babel/runtime:

`npm install -D @babel/runtime`

For convenience there are two package.json examples, one with and one without @babel/runtime; these are `package-with-babel-runtime.json` and `package-without-babel-runtime.json` respectively