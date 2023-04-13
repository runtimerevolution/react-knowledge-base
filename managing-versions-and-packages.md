# Managing versions and packages

## Table of contents
1. [Node Version Manager](#node-version-manager)
2. [Node Package Manager](#node-package-manager)
3. [Yarn](#yarn)

## Node Version Manager

During your journey React.js, you will probably work on many projects that use different versions of Node.js. That is where a version manager comes in handy.

[Node Version Manager](https://github.com/nvm-sh/nvm) (NVM) is a tool used to manage multiple active Node.js versions.

It allows you to locally download any of the remote Long Term Support (LTS) versions of Node.js with a simple command; easily switch between multiple versions of Node.js, right from the command line, and even set up aliases to switch between different downloaded versions of Node.js with ease.

### Installation

#### Remove existing versions
First, remove existing Node.js versions with the following commands. If this is your first time using Node.js and you don't have any versions installed yet you can just skip this step.

```
brew uninstall --ignore-dependencies node 
brew uninstall --force node 
```

#### Install NVM

Now, your system is ready for installation. You can follow the [official NVM documentation](https://github.com/nvm-sh/nvm#installing-and-updating) for the most updated way to install NVM locally.


### Installing a Node.js version with NVM

First of all, see what Node versions are available to install. To see available versions, type:

```
nvm ls-remote
```

Now, you can install any version listed in the above output. You can also use aliases names like `node` for latest version, `lts` for latest LTS version, etc.

```
nvm install node     # Installing Latest version 
nvm install 14       # Installing Node.js 14.X version 
```

After installing you can verify what is installed with:

```
nvm ls 
```

If you have installed multiple versions on your system, you can set any version as the default version at any time. To set the node 14.X as the default version, simply use:

```
nvm use 14
```

Similarly, you can install other versions like Node 12.X or Node 15 and switch between them.

## Node Package Manager

<img src="assets/npm.png" align="right" style="width: 200px; margin-left: 10px;"/>

[Node Package Manager](https://www.npmjs.com/) (NPM) is a popular package manager among JavaScript developers. It is the default package that is automatically installed whenever you install Node.js on your system.

It consists of three components: [the website](https://www.npmjs.com/) to manage various aspects of your npm experience, Command Line Interface (CLI) to interact with npm via the terminal, and registry to access an extensive public database of JavaScript software as well as publish your own. 

To install a package using NPM you can search for it on the website, select the package, for example, the [`react`](https://www.npmjs.com/package/react) package, and run the install command.

```
npm install <package name>
```

Uninstalling packages can be done by calling the npm uninstall command followed by the package name.

```
npm uninstall <package name>
```

## Yarn

[Yarn](https://classic.yarnpkg.com/en/) is another popular package manager for the JavaScript programming language. The intention behind creating Yarn was to address some of the performance and security shortcomings of working with `npm` (at that time).

Since then, `npm` has undergone several improvements to fix some of its inefficiencies. As a result, `npm` and `yarn` are now in a neck-to-neck race over which package manager trumps the other.

According to the official documentation, the recommended way to install Yarn in your project is through the node package manager using the following command:

```
# npm 6.x

npm install yarn --global
```

```
# npm 7+, extra double-dash is needed:

npm install yarn -- --global
```

To install a package using Yarn you can search for it on the website, select the package, for example, the [`react`](https://classic.yarnpkg.com/en/package/react) package, and run the install command.

```
yarn add <package name>
```

Uninstalling packages can be done by calling the yarn remove command followed by the package name.

```
yarn remove <package name>
```

And to uninstall it:
```
yarn remove react
```

## What package manager should you use
They both work well, so the choice between them is really up to you.

However, it's worth remembering that the intention behind developing yarn was to fix performance and security concerns with npm. Yarn is generally faster than npm, especially when it comes to installing packages.

Also, yarn generates a `yarn.lock` file that is generally considered more reliable that npm's `package-lock.json` when it comes to ensuring consistency across different machines.

That being said, if you want a bigger community, if you already know npm or prefer its commands, it's a great choice too. Ultimately, the decision between yarn and npm depends on your personal preference and the specific needs of your project.

[Here](https://www.geeksforgeeks.org/difference-between-npm-and-yarn/) is a cool article if you want to know more about the differences between the two of them.

[<< Back](/README.md)
