#Scrambled Number Generator

- Plan your execution on white board before forking and cloning.
- Fork and clone the project.
- Set up your file structure.
  - [Folder] Scrambled-Number-Generator
    - [Folder] js
      - generator.js
    - [Folder] spec
      - generator-spec.js
- Install npm, mocha, and chai from your Scrambled-Number-Generator folder

 ```sh
  $ npm init
  $ npm install -D mocha chai
 ```
- Write unit tests for the generator in generator-spec.js. Commit!
  - Include either or both declations in your spec.js, depending on what syntax you want to use:
  ```sh
    var should = chai.should();
    var expect = chai.expect;
  ```
  - Also include
  ```sh
  var chai = require("chai");
  var generator = require("../js/generator.js");
  ```
  - Be logical and atomic in your unit tests.
- Run your tests by running mocha.
```sh
mocha ./spec
```
- Implement the generator in generator.js. Commit!
  - Function name : generate
  - Takes "amount", the amount of numbers to generate, counting from 0 to "amount" - 1
  - Returns an array containing the specified number of UNIQUE numbers.
  - Calling the function with the same parameter subsequent times will return the array of numbers in a new, random order.
    - For example, calling
    ```sh
    $ generate(1000)
    ```
    should return an array that contains 1000 unique numbers.
    - Calling it again should return the same numbers in random order.
    - Include
    ```sh
    module.exports = generate;
    ```
