Mojibak
=======
Utility to recover garbled (mojibaked) text. Inspired by Ruby's [mojibake](https://github.com/dekellum/mojibake).

Installation
------------

    npm install mojibak

Usage
-----

    import {recover} from "mojibak";
    const sandwich = recover("â\u0080\u008BBigMac");

One liner

    NODE_PATH=$(npm root -g) node -e \
      'const {recover} = require("mojibak");console.log(recover("Itâ\u0080\u0099s cool"))'
