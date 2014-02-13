#luvit-test
The [Lua](http://www.lua.org/) test runner from [Luvit](http://luvit.io/), in a modular package

##Install
- Download and install [Node.js](http://nodejs.org/download/). Then you have `npm`
- In the root of your Luvit project, `npm install luvit-test`

##Usage
- In a tests directory, create tests in lua files.
At the top of each test file,
```lua
require("luvit-test/helper")
```
Then `assert()` things you want to test.
- Create an `init.lua` file in the tests directory, with just the line
```lua
require("luvit-test/runner").run(__dirname)
```
- Run the tests with: `luvit init.lua`

##Example
```
npm install luvit-set
npm test luvit-set
```

##License
LGPL+; see the `LICENSE` file
