Mojibak
=======
Utility to recover garbled (mojibaked) text. Inspired by Ruby's [mojibake](https://github.com/dekellum/mojibake).

Installation
------------

    npm install mojibak

Usage
-----

    import {recover} from "mojibak";
    const sandwich = recover("â\\u0080\\u008BigMac");

One liner

    NODE_PATH=$(npm root -g) node -e \
      'const {recover} = require("mojibak");console.log(recover(" HACPâ\\u0080\\u0099s"))'

**N.B.** the input text to `recover` should include literal unicode escape sequences:

    recover("\\u0080"); // yes
    recover("\u0080");  // no
