## Basic introduction to `npm`, `nvm` and `yarn`
In order to make project setup easier or switching between projects less harmful, we use a version manager for Node.js (same as we have for ruby/python), this version manager is called RVM, with this manager you can have multiple node versions and using it’s CLI it’s very straightforward to switch between them.

To install this manager just run:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```
And to finish the setup, add the next block to your `bash` config.
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" 
```
After all this, installing a node version is just as easy as running:
```
nvm install 14.7.0 # or 16.3.0, 12.22.1, etc
```
And to use one of the installed versions on the project, just run:
```
nvm use 14.7.0
```
To access the community made packages like libraries, plugins or frameworks, we have NPM and Yarn, both of these are package managers, where you can search the package library and import it to your own project. We’ll focus on Yarn since it makes locking packages to a certain version much easier and without needing to have to configure locking options.

To install yarn just run:
```
brew install yarn
```
And then add its path to your `bash` config, with something like:
```
export PATH=”$PATH:/opt/yarn-[version]/bin”
```
To setup a new project, run:
```
yarn init
```
This will generate a package.json file and a yarn.lock file.
To add a new package, it's just as easy as:
```
yarn add react
```
And to uninstall it:
```
yarn remove react
```

Useful links:
- [NVM](https://github.com/nvm-sh/nvm)
- [NPM](https://docs.npmjs.com/)
- [Yarn](https://yarnpkg.com/getting-started)
- [More about this](https://medium.com/@hanke.liu/understand-node-js-npm-and-nvm-efc61dfd7ff8
)
