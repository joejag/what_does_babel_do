Demo for playing with Babel and Webpack.

Try running each command then seeing what you get in the `build` directory.

- `rm -rf build && npx babel src --out-dir build`
- `rm -rf build && npx babel src --out-dir build --plugins=@babel/plugin-transform-arrow-functions`
- `rm -rf build && npx babel src --out-dir build --presets=@babel/preset-env`
- `rm -rf build && npx babel src --out-dir build --presets=@babel/preset-env,minify`
- `rm -rf build && npx webpack src/app.js -o build/bundle.js --mode=development`
- Add a dependency, use it, then rebuild with webpack