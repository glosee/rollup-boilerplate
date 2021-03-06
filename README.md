# Rollup Boilerplate

I spent a Saturday night getting Rollup setup to start working through a tutorial to try building a game in JS. It took a little while to get setup, so when everything was working, I thought it would be good to keep a project in this state to quickly bootstrap future projects.

You shoudl be able to just clone this, rename it to whatever you want, and start writing your application.

## What's included (tooling)

* [rollup](http://rollupjs.org/)
* [babel](https://babeljs.io/)
* [eslint](http://eslint.org/)
* [postcss](http://postcss.org/)
	* _including the plugins_ `simplevars`, `nested`, `cssnext`
* [http-server](https://github.com/indexzero/http-server)
* [rollup-plugin-replace](https://github.com/rollup/rollup-plugin-replace) (for easy NODE_ENV)

## How it works

* `src` is the place for all your styles and JS
* `src/index.js` is the entry point for your JS
	* it also loads `src/styles/main.css`
* `npm run build` builds everything in `src` into `dist/bundle.js`
* `dist/index.html` loads `dist/bundle.js`

## Tasks

* `npm run dev` runs `rollup-watch`, `livereload`, and `http-server`. You can go to `http://localhost:8080` in the browser to view your app. Any changes to files in `/src` or `/dist` will automatically rebuild and/or reload.
