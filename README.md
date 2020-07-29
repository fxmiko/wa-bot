<div align="center">
<img src="https://media1.giphy.com/media/RkN0K0MEfEcc34HeZ4/giphy.gif" width="128" height="128"/>

# WhatsApp Bot
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
