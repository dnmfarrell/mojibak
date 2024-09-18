Mojibak
=======
Utility to recover garbled (mojibaked) text. Inspired by Ruby's [mojibake](https://github.com/dekellum/mojibake).

Installation
------------

    npm install mojibak

Usage
-----

    const {recover} = require("./mojibake.js");
    const sandwich = recover("â\u0080\u008BigMac");
