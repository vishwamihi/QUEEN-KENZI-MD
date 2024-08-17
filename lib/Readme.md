#NEXUS-MD

NEXUS-MD is a powerful and versatile WhatsApp bot built using Node.js and the Baileys library. This bot offers a wide range of features and capabilities, making it an excellent choice for both personal and commercial use cases.

<img alt="NEXUS-MD" width="700" height="300" src="https://telegra.ph/file/c2ab0216f21a83c63ba3f.jpg">

🚀 Deploy yourNEXUS-MD on DigitalOcean and get $200 in free credits! Click the badge above to sign up and take advantage of this amazing offer. DigitalOcean's reliable and scalable cloud infrastructure ensures your bot runs smoothly, no matter how many users you have. Don't miss out on this opportunity to supercharge your WhatsApp experience!

QR AND PEYER CODE ✅

https://shuter-session-l1xx.onrender.com

<a href="https://session-genarator-by-rodda-97b9e77fccab.herokuapp.com/"><img src="https://img.shields.io/badge/GET-HERAKU DEPLOY-black" alt="NEXUS-MD" width="250"></a>

[![JOIN WHATSAPP CHANEL](https://raw.githubusercontent.com/Neeraj-x0/Neeraj-x0/main/photos/suddidina-join-whatsapp.png)](https://whatsapp.com/channel/0029VabteKy90x2pYTUqub3H)

## Table of Contents

- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Deploy on Any Shell (Including Termux)](#deploy-on-any-shell-including-termux)
- [Usage](#usage)
  - [Creating a Plugin](#creating-a-plugin)
  - [Sending Messages](#sending-messages)
    - [Replying](#replying)
    - [Media](#media)
    - [Sticker](#sticker)
  - [External Plugins](#external-plugins)
- [Community and Support](#community-and-support)
- [Credits](#credits)
- [License](#license)

## Installation

### Prerequisites

Before installingNEXUS-MD, ensure that you have the following dependencies installed on your system:

- FFmpeg
- Node.js

### Deploy on Any Shell (Including Termux)

To deployNEXUS-MD on any shell, including Termux, follow these steps:

1. Fork theNEXUS-MD repository
2. Edit the `config.js` file with your desired configuration details
3. Install the required dependencies by running the following commands:
   - `npm install`
   - `npm install qrcode-terminal`
   - `npm install pm2 -g`
4. To scan the QR code and start the bot, run `npm start`
5. To connect using a pairing code, run `npm run code`. After pairing, run `npm start` again and scan the QR code
6. country code is require for connecting via pairing code. If you are from India, you can use `91` as country code. If you are from any other country, you can use your country code.
7. To stop the bot, press `Ctrl+C`
8. To start the bot, run `npm start` 

## Usage

### Creating a Plugin

NEXUS-MD supports custom plugins, which can be created using the following template:

```javascript
const { command, isPrivate } = require("../../lib/");

command({
  pattern: "ping", // Command pattern
  fromMe: isPrivate, // Need to respond for everyone's message? true: only from sudo numbers, false: from everyone, isPrivate: same as false but will be considered as true if worktype is private
  desc: "To check ping", // Description of the command
  type: "user", // Command type
}, async (message, match) => {
  /* PLUGIN CONTENT HERE */
});
```

### Sending Messages

#### Replying

To reply to a message, use the following code:

```javascript
message.reply("Hi");
```

#### Media

To send media (image, audio, or video), use the following code:

```javascript
let content = "https://wallpaperaccess.com/full/5531321.jpg"; // Can also use a buffer
message.sendMessage(jid, content, {} /* options */, "image" /* change to 'audio' or 'video' when sending audio or video */);
```

#### Sticker

To send a sticker, use the following code:

```javascript
message.sendMessage(jid, "url or buffer of image or video (max 10 seconds)", { packname: config.PACKNAME, author: config.AUTHOR }, "sticker");
```

### External Plugins

NEXUS-MD supports external plugins. You can find more information about external plugins in the [Plugins wiki](https://github.com/ACHALA-ESHAN/QUUEN-ESHU-MD/blob/main/Readme.md).

## Community and Support

Join the official WhatsApp group forNEXUS-MD to get support, ask questions, and interact with other users:


## License

NEXUS-MD is licensed under the [MIT License](https://opensource.org/licenses/MIT):

```
MIT License

Copyright (c) 2023 X-Electra

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```