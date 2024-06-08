<h1 align="center">
	<br>
	<br>
	<img width="320" src="https://github.com/patrtorg/aut-velit/blob/main/media/CodePolishLogo.png" alt="CodePolish">
	<br>
	<br>
	<br>
</h1>

# CodePolish.js

<h3 align = "center">
Beautify your code, Elevate your projects
</h3>
A npm package written on node to beautify your code be it any tech specific, be it JSON, JS, YAML, Python or JAVA extension files.

# Installation
You can install CodePolish using:

`npm i @patrtorg/aut-velit`

or

`npm install @patrtorg/aut-velit`

# Usage

# Basic Usage 

Now, let's say we have a file: sample.js

```javascript
// sample.js
function greet(name) {
return `Hello, ${name}!`;
}console.log(greet('Ankit Guria'));
```

Some dependencies maybe required, like:

`npm install yaml`

As the package also supports .yaml files.
Now just head to the directory of this file and run this command on the console:

`node -e "require('@patrtorg/aut-velit').beautifyJS('sample.js')"`

Similarly, a sample.json

```JSON
// sample.json
{"name":"Ankit Guria","age":25,"city":"India"}
```
Now just head to the console:

`node -e "require('@patrtorg/aut-velit').beautifyJSON('sample.json')"`

And the below screenshot can be seen as it is on the console:

![consoleprompt](https://github.com/patrtorg/aut-velit/blob/main/media/consoleprompt.png)

# (Examples)

# Test1: Playing with Python files, beautifying .py

![OutputImage1](https://github.com/patrtorg/aut-velit/blob/main/media/earlierPY.png)


`node -e "require('@patrtorg/aut-velit').beautifyPython('sample.py')"`

# Output:

![OutputImage12](https://github.com/patrtorg/aut-velit/blob/main/media/formattedPY.png)

# Test2: Playing with JS files, beautifying .js

![OutputImage1](https://github.com/patrtorg/aut-velit/blob/main/media/earlierJS.png)

`node -e "require('@patrtorg/aut-velit').beautifyJS('sample.js')"`

# Output:

![OutputImage12](https://github.com/patrtorg/aut-velit/blob/main/media/formattedJS.png)

# Test3: Playing with JAVA files, beautifying .java

![OutputImage1](https://github.com/patrtorg/aut-velit/blob/main/media/earlierJAVA.png)

`node -e "require('@patrtorg/aut-velit').beautifyJava('sample.java')"`

# Output:

![OutputImage12](https://github.com/patrtorg/aut-velit/blob/main/media/formattedJAVA.png)

# Test4: Playing with JSONs, beautifying JSON Linters

![OutputImage1](https://github.com/patrtorg/aut-velit/blob/main/media/earlierJSON.png)

`node -e "require('@patrtorg/aut-velit').beautifyJSON('sample.json')"`

# Output:

![OutputImage12](https://github.com/patrtorg/aut-velit/blob/main/media/formattedJSON.png)


# Dependencies

`npm install require `
and 
`npm install js-yaml `

# Steps for a layman(Playground)
1. Create a new project: 

`npm init`

This command will create a package.json dependencies for your test file.

```json
// package.json
{
  "name": "@patrtorg/aut-velit",
  "version": "1.0.2",
  "description": "Beautify your code, Elevate your projects",
  "main": "index.cjs",
  "type": "commonjs",
  "directories": {
    "lib": "lib"
  },
  "scripts": {
    "test": "node --experimental-modules test.cjs  "
  },
  "funding": {
    "type": "individual",
    "url": "https://github.com/sponsors/ankit142"
  },
  "repository": {
    "type": "git",
    "url": "https://github.com/patrtorg/aut-velit.git"
  },
  "bugs": {
    "url": "https://github.com/patrtorg/aut-velit/issues"
  },
  "homepage": "https://github.com/patrtorg/aut-velit#readme",
  "author": "Ankit Guria",
  "license": "MIT",
  "dependencies": {
    "js-yaml": "^4.1.0",
    "require": "^2.4.20"
  }
}

```

2. A new file like - "test.cjs" to be created. 
Here is the sample code:
```javascript
// test.cjs
const { beautifyJSON, beautifyYAML, beautifyJS, beautifyPython, beautifyJava } = require('./index.cjs');


// Paths to the unformatted example files
const filePathJSON = './test/example.json';
const filePathYAML = './test/example.yaml';
const filePathJS = './test/example.js';
const filePathPython = './test/example.py';
const filePathJava = './test/example.java';

// Test beautify functions
beautifyJSON(filePathJSON);
beautifyYAML(filePathYAML);
beautifyJS(filePathJS);
beautifyPython(filePathPython);
beautifyJava(filePathJava);

console.log('Beautification completed successfully!');

```
3. Now run this file, and here you go.
`node --experimental-modules test.cjs`

4. Play and enjoy more with custom console log statements or something else.
The output should be something like this: 

![OutputImage13](https://github.com/patrtorg/aut-velit/blob/main/media/output.png)
# Contributing
Feel free to contribute by opening issues or submitting pull requests on [GitHub](https://github.com/patrtorg/aut-velit).

# License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/patrtorg/aut-velit/blob/main/LICENSE) file for details.