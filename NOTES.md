- using VSCode extension LiveServer for development
- following Traversy playlist - [Responsive Portfolio Website](https://www.youtube.com/playlist?list=PLillGF-RfqbYoGoCjKoMOkVznV6aSXKzU)
- image credits:
  - [background](https://www.pexels.com/photo/aerial-photo-of-mountain-surrounded-by-fog-733174/)

creating initial files.

- dist/index.html
- scss/main.scss

And in order for Sass to work - we we can get node-sass from NPM.

So...

`npm init`

and then

`npm install node-sass`

and also add a script to our `package.json` so we can use the `sass` command to execute `node-sass` and build our regular `.css` files in our `/dist` folder which is what we'll actually deploy. None of the node_modules will get deployed with the website - we're only using it in dev for the Scss compiler.

`package.json`

```
    "sass": "node-sass -w scss/ -o dist/css/ --recursive"
```
