Demo for playing with Babel and Webpack.

Try running each command then seeing what you get in the `build` directory.

- `rm -rf build && npx babel src --out-dir build`
- `rm -rf build && npx babel src --out-dir build --plugins=@babel/plugin-transform-arrow-functions`
- `rm -rf build && npx babel src --out-dir build --presets=@babel/preset-env`
- `rm -rf build && npx babel src --out-dir build --presets=@babel/preset-env,minify`

Now we move onto webpack, which takes multiple files and makes them into one

- `rm -rf build && npx webpack src/app.js -o build/bundle.js --mode=development`
- `rm -rf build && npx babel src --out-dir build --presets=@babel/preset-env && npx webpack build/app.js -o build/bundle.js --mode=development`
- Add a dependency to the project, require it, then rebuild the project with webpack