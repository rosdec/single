# Single node Hyperledge Sawtooth project
This repository contains a stripped down version of the repo [HelloWorld-Sawtooth](https://github.com/Kerala-Blockchain-Academy/HelloWorld-Sawtooth) from Kerala Blockchain Academy.

## Installation
Follow the stemps to run the simple demo.
1. clone the repo
2. use node 12 not the last, I know but some of the libraries are picky, at least under Windows
3. `npm i` to install dependencies
4. `docker-compose -f single-node.yaml up -d` to build and exacute the blockchain
5. `node interact.js` to run the simple interaction with the blockchain
6. Use `docker-compose -f single-node.yaml down` to safely shutdown the node

The expected output will be something like:
```
Storing at: 8ae6aec2879b0209cfa70c3f464ab38177341707edac6b2bc58e974141d2fd46b1d44a
Getting from: http://127.0.0.1:8008/state/8ae6aec2879b0209cfa70c3f464ab38177341707edac6b2bc58e974141d2fd46b1d44a
Wrote to blockchain the payload [Hello, world!]
Read from blockchain: [Hello, world!]
```
