# INCUBED

INCUBED = A trustless INcentivized remote Node Network = IN3

This is the Typescript-version of the incubed client.

[![Build Status](https://travis-ci.com/slockit/in3.svg?token=2HePjq6vsCVWSbiYxgEy&branch=master)](https://travis-ci.com/slockit/in3)

# Getting started

```
npm install --save in3
```

In your code:

```js

// import in3-Module
import In3Client from 'in3'
import * as web3 from 'web3'

// use the In3Client as Http-Provider
const web3 = new Web3(new In3Client({
    proof: true,
    signatureCount: 1,
    requestCount : 2,
    chainId: '0x01'
}))

// use the web3 
const block = await web.eth.getBlockByNumber('latest')
...


```


# Documentation

The following docuemntations are available:

- [API](https://github.com/slockit/in3/blob/master/doc/README.md) - Definition of Classes and available functions.
- [DataTypes](https://github.com/slockit/in3/blob/master/src/types/README.md) - Defintion of datastructures used inside the client.
- [Verification](https://github.com/slockit/in3/wiki/Ethereum-Verification-and-MerkleProof). A documentaion about the varification of proofs send by a IN3-Server.
- [Wiki](https://github.com/slockit/in3/wiki). A wiki with examples and explanations of the protocol.


# Tests

- Result of the last nightly tests for [in3](http://travis.slock.it/in3/) and [in3-server](http://travis.slock.it/in3-server/)
- [Code Coverage](http://travis.slock.it/in3-server/coverage/index.html) for client and server
