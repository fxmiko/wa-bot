<div align="center">
<img src="https://raw.githubusercontent.com/open-wa/wa-automate-nodejs/master/resources/hotfix-logo.png" width="128" height="128"/>

# wa-automate-nodejs

> wa-automate-nodejs is the most advanced NodeJS library which provides a high-level API to control WA.
>
>

[![npm version](https://img.shields.io/npm/v/@open-wa/wa-automate.svg?color=green)](https://www.npmjs.com/package/@open-wa/wa-automate)
![node](https://img.shields.io/node/v/@open-wa/wa-automate)
[![Downloads](https://img.shields.io/npm/dm/@open-wa/wa-automate.svg)](https://www.npmjs.com/package/@open-wa/wa-automate)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/open-wa/wa-automate-nodejs.svg)](http://isitmaintained.com/project/open-wa/wa-automate-nodejs "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/open-wa/wa-automate-nodejs.svg)](http://isitmaintained.com/project/open-wa/wa-automate-nodejs "Percentage of issues still open")

<a href="https://discord.gg/dnpp72a"><img src="https://img.shields.io/discord/661438166758195211?color=blueviolet&label=discord&style=flat" /></a> ![WhatsApp_Web 2.2029.4](https://img.shields.io/badge/WhatsApp_Web-2.2029.4-brightgreen.svg)

[![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]
[![Consulting Request][consult-shield]][consult]

</div>

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
