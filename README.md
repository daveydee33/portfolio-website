# Description

Simple portfolio-style static website using HTML, SCSS, JavaScript. Responsive and mobile-friendly design.

# Notes

- Don't edit the `main.css` file directly. Only edit the files in `scss` directory and then run `npm run sass` to build the css directory and files using node-sass.

- To deploy this to GitHub pages:

```
npm run deploy
```

# To Do

- I think I may need to work on the transition a bit more so that it rotates the other direction - and then I'd also need to fix the positioning of them also so the X is correct and positioned correctly.

# Dev Part 1 - Creating initial files, and Sass workflow setup.

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

# Dev Part 2

- homepage and main Sass
- rotating menu button, animated with JavaScript and Sass.
- menu overlay and responsiveness
- About page with CSS grid
- Work/Projects page and Contact page

# Credits

- Example taken from Traversy Media [Responsive Portfolio Website](https://www.youtube.com/playlist?list=PLillGF-RfqbYoGoCjKoMOkVznV6aSXKzU) and [repo](https://github.com/bradtraversy/modern_portfolio)

- [background image](https://www.pexels.com/photo/aerial-photo-of-mountain-surrounded-by-fog-733174/)
