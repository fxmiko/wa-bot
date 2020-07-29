<div align="center">
<img src="https://media1.giphy.com/media/RkN0K0MEfEcc34HeZ4/giphy.gif" width="128" height="128"/>

# WhatsApp Bot

> Create a simple WhatsApp Bot using NodeJS
>
>
</div>
[![npm version](https://img.shields.io/npm/v/@open-wa/wa-automate.svg?color=green)](https://www.npmjs.com/package/@open-wa/wa-automate)
![node](https://img.shields.io/node/v/@open-wa/wa-automate)

## Installation

```bash
> npm i --save @open-wa/wa-automate
```

## Usage

```javascript
// import { create, Client } from '@open-wa/wa-automate';
const wa = require('@open-wa/wa-automate');

wa.create().then(client => start(client));

function start(client) {
  client.onMessage(message => {
    if (message.body === 'Hi') {
      client.sendText(message.from, '👋 Hello!');
    }
  });
}
```
