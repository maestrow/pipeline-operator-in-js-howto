## How to use `|>` proposal operator

To use [pipeline](https://github.com/tc39/proposal-pipeline-operator) operator now there are two options: 

1. `@babel/plugin-proposal-pipeline-operator` plugin
2. `@babel/preset-stage-1` preset

In both options we use `babel`. Babel options comes in `.babelrc`.


## Linting in VS Code

1. Install ESLint extension
2. Create `.eslintrc.json` (see it in project dir). 
3. `.babelrc` with options must exists.
4. Install packages `eslint`, `babel-eslint`.
5. In VS Code settings disable javascript validation (`"javascript.validate.enable": false`), eslint validation must be enabled by default after install extension. See `.vscode/settings.json`


## Go test it!

`git clone https://github.com/maestrow/pipeline-operator-in-js-howto`

If you want only `|>` operator plugin (1st option), then go to first commit (`git checkout 8d13384052ca7500bc08ac48c7eb05c777c20510`).
If you want all stage 1 proposals (2nd option), it comes from second commit.

    npm i      # install all dependencies
    npm start  # it runs `pipe.js` (full command see in `package.json`)

See `6` in output.

Open `pipe.js` and make sure that linter doesn't report an error.
