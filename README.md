# [DEPRECATED] Screeps typescript skeleton project

## This skeleton is deprecated. You can find actively updated starter kit in here: https://github.com/screepers/screeps-typescript-starter


This is a Screeps' project skeleton for Typescript programmers. The skeleton is based on vanhouc's work: https://github.com/vanhouc/screeps. 

Screeps is MMO strategy open world game for programmers. You write real JavaScript (in this case Typescript) which controls your units autonomously.

Read more: https://screeps.com/

### Getting Started

This skeleton is cross platform. You can easily run the project with Jetbrains PHPStorm or use it in your VStudio. TS->JS compiling is done by TSProject.

Skeleton includes everything you need to get up and running as quickly as possible. 

* GULP script for automatic uploading the code to Screep's account
* TSProject transpiling from Typescript to Javascript
* TS interfaces for Screep's API
* TS interfaces for Lo-Dash API

#### Small sample project using this skeleton can be found here [GitHUB link](https://github.com/MarkoSulamagi/Screeps-typescript-sample-project)

> Screep API typescript type definitions are incuded as dependency. See their up to date status in here [GitHUB link](https://github.com/MarkoSulamagi/Screeps-Typescript-Declarations)

Discussion in [screep's community forum](http://support.screeps.com/hc/en-us/community/posts/207116485-Writing-Screep-bots-with-Typescript?page=1#)

### Prerequisities

Required dependencies:

```
NodeJS https://nodejs.org/en/
- `npm` command available in your CLI
```

Optional dependencies (only if you want to follow these installation instructions fully): 

```
GIT https://git-scm.com/
- `git` command available in your CLI (if you want to follow these instructions) 
```

### Installing

```
$ git clone git@github.com:MarkoSulamagi/Screeps-typescript-skeleton.git
$ cd Screeps-typescript-skeleton

$ npm install
```

### Configuring

```
Rename secrets.default.js file to secrets.js
Fill "username" and "password" properties in just renamed secrets.js file with your Screep's username and email. 

**NEVER COMMIT THIS FILE TO ANY VERSION CONTROL** 
```

### Coding and running the app

To run the compiler and uploader, navigate to your project folder and run this command

```
$ npm start
```

Now every time you edit your typescript files, main.js in ./dist folder is uploaded to your Screep scripts into "default" branch.

Project files are in ./src.

```
./src/main.ts - Application bootstrap. Don't change this file
./src/start/game-manager.ts - Your main module. This is where the program starts. There are instructive comments in the class file. 
./src/screeps.d.ts - Typescript interfaces for Screep's API. This includes autocomplete and data types to your project. This file can get outdated if Screep's team adds new functionality or changes something.

./dist - Your compiled files. This will be created automatically. No need to change anything in here.
./typings - Lo-Dash Typescript interfaces. Created automatically and no need to change anything.
```

#### How to extend Screeps prototypes?

https://github.com/MarkoSulamagi/Screeps-typescript-skeleton/issues/9

### Migrating your Javascript bot to Typescript

Unfortunately I haven't been able to create tutorial for this yet. Issue about it is here: [Documentation for migrating your bot to Typescript #4](https://github.com/MarkoSulamagi/Screeps-typescript-skeleton/issues/4)

Because Typescript compiler can also read Javascript, migrating should be possible with fairly few changes to your code.

### Running the tests

No tests. Testing can definitely be done, but it's out of this project's scope. 
You can use Jasmine and Karma to create unit tests. You might need to implement some dependency injection system. 

### Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

### Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/MarkoSulamagi/Screeps-typescript-skeleton/tags). 

### Authors

* **Marko Sulamägi** - *Converted Cameron's work to quickly installable TS skeleton app* - [MarkoSulamagi](https://github.com/MarkoSulamagi)
* **vanhouc** - *Screep project with TS functionality. His gulpfile and screep.d.ts was very useful.* - [vanhouc](https://github.com/vanhouc)

See also the list of [contributors](https://github.com/MarkoSulamagi/Screeps-typescript-skeleton/graphs/contributors) who participated in this project.

### License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

### Acknowledgments

* Special thanks to Screep's team for this awesome game and communit in webchat (https://webchat.freenode.net/?channels=#screeps). 

