<div align="center">
<img src="https://media1.giphy.com/media/RkN0K0MEfEcc34HeZ4/giphy.gif" width="128" height="128"/>

# WhatsApp Bot

> Create a simple WhatsApp Bot using NodeJS
>
>
</div>
[![npm version](https://img.shields.io/npm/v/@open-wa/wa-automate.svg?color=green)](https://www.npmjs.com/package/@open-wa/wa-automate)
![node](https://img.shields.io/node/v/@open-wa/wa-automate)
<a href="https://discord.gg/dnpp72a"><img src="https://img.shields.io/discord/661438166758195211?color=blueviolet&label=discord&style=flat" /></a> ![WhatsApp_Web 2.2029.4](https://img.shields.io/badge/WhatsApp_Web-2.2029.4-brightgreen.svg)

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
