# Rollup Boilerplate

I spent a Saturday night getting Rollup setup to start working through a tutorial to try building a game in JS. It took a little while to get setup, so when everything was working, I thought it would be good to keep a project in this state to quickly bootstrap future projects.

You shoudl be able to just clone this, rename it to whatever you want, and start writing your application.

## What's included (tooling)

* [rollup](http://rollupjs.org/)
* [babel](https://babeljs.io/)
* [eslint](http://eslint.org/)
* [postcss](http://postcss.org/)
	* _including the plugins_ `simplevars`, `nested`, `cssnext`
* [rollup-plugin-replace](https://github.com/rollup/rollup-plugin-replace) (for easy NODE_ENV)

## How it works

* `src` is the place for all your styles and JS
* `src/index.js` is the entry point for your JS
	* it also loads `src/styles/main.css`
* `npm run build` builds everything in `src` into `dist/bundle.js`
* `dist/index.html` loads `dist/bundle.js`

## Extras

* `npm run dev` runs `rollup-watch` and `livereload` so that changes are auto-reloaded in the browser (configured in `src/index.js`)