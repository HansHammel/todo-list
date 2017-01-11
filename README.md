# Todo-List [![Build Status](https://travis-ci.org/rameshvarun/todo-list.svg)](https://travis-ci.org/rameshvarun/todo-list)

Todo-list starts a server to find TODOs, FIXMEs, and NOTEs,
presenting them in an interface that lets you sort by assignee
and file. The server will also show code snippets.

[![NPM](https://nodei.co/npm/todo-list.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/todo-list/) 
[![NPM](https://nodei.co/npm-dl/todo-list.png?months=9&height=3)](https://nodei.co/npm/todo-list/)

[![npm version](https://img.shields.io/npm/v/todo-list.svg)](https://www.npmjs.com/package/todo-list)
[![npm license](https://img.shields.io/npm/l/todo-list.svg)](https://www.npmjs.com/package/todo-list)
[![npm download](https://img.shields.io/npm/dm/todo-list.svg)](https://www.npmjs.com/package/todo-list)
[![npm download](https://img.shields.io/npm/dt/todo-list.svg)](https://www.npmjs.com/package/todo-list)
[![Package Quality](http://npm.packagequality.com/shield/todo-list.svg)](http://packagequality.com/#?package=todo-list)
[![Inline docs](http://inch-ci.org/github/HansHammel/todo-list.svg?branch=master)](http://inch-ci.org/github/HansHammel/todo-list)
[![star this repo](http://githubbadges.com/star.svg?user=HansHammel&repo=todo-list&style=flat&color=fff&background=007ec6)](https://github.com/HansHammel/todo-list)
[![fork this repo](http://githubbadges.com/fork.svg?user=HansHammel&repo=todo-list&style=flat&color=fff&background=007ec6)](https://github.com/HansHammel/todo-list/fork)

[![david dependency](https://img.shields.io/david/HansHammel/todo-list.svg)](https://david-dm.org/HansHammel/todo-list)
[![david devDependency](https://img.shields.io/david/dev/HansHammel/todo-list.svg)](https://david-dm.org/HansHammel/todo-list)
[![david optionalDependency](https://img.shields.io/david/optional/HansHammel/todo-list.svg)](https://david-dm.org/HansHammel/todo-list)
[![david peerDependency](https://img.shields.io/david/peer/HansHammel/todo-list.svg)](https://david-dm.org/HansHammel/todo-list)
[![npms score](https://badges.npms.io/todo-list.svg)](https://www.npmjs.com/package/todo-list)
[![Known Vulnerabilities](https://snyk.io/test/github/HansHammel/todo-list/badge.svg)](https://snyk.io/test/github/HansHammel/todo-list)

![Imgur](http://i.imgur.com/c2PahkF.png)

# Using as an Application
Todo-list can be installed and used as an application.
```
npm install -g todo-list
```

Then navigate to your code directory, and run the following command.

```
todo-list
```

You should be able to navigate your browser to `http://localhost:3000/` and see the
results.

# Using as a Library
```javascript
var todolist = require("todo-list");
todolist.findMarks("// TODO(bob): This is a TODO assigned to bob.");
/*[{
	content: 'TODO(bob): This is a TODO assigned to bob.',
	line: 0,
	assignee: 'bob',
	type: 'TODOs'
}]*/
```
