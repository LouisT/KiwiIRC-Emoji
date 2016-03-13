# Kiwi IRC Emoji Plugin

This plugin uses [Twemoji]! Would you prefer [EmojiOne]? Check out [KiwiIRC-Emoji-EmojiOne]!

This plugin now uses [Twemoji] 2.0; For 1.0 see the [twemoji-1.0] branch.

[Twemoji] has a CDN hosted version, provided by MaxCDN.
Therefore you can run [emoji-plugin.cdn.html](emoji-plugin.cdn.html) without any changes.

![Example](https://github.com/LouisT/KiwiIRC-Emoji-Twemoji/blob/master/assets/KiwiIRC-Emoji-Twemoji.gif)

Usage
-
Place [emoji-plugin.cdn.html](emoji-plugin.cdn.html) in `/client/assets/plugins/` and edit `config.js` to include it in your plugins list.

```javascript
conf.client_plugins = [
    // "http://server.com/kiwi/plugins/myplugin.html"
    "/kiwi/assets/plugins/emoji-plugin.cdn.html",
    "/kiwi/assets/plugins/textstyle.html"
];
```

Plugin Generation
-
If you would prefer to host a copy of the [Twemoji] files yourself, you can build a copy of the plugin using `./build-plugin.js --local`. If you wish to change the location of [Twemoji] files you can do so with `--baseurl=<URL or Path>`; useful if your Kiwi IRC install is not at `http://domain.tld/kiwi/` or you want to use a different CDN.

In order to build the plugin, you will need to clone the [Twemoji] repository relative to `build-plugin.js` using `git clone https://github.com/twitter/twemoji.git`

License
-
Copyright 2016 Louis T.

Code licensed under the MIT License: http://opensource.org/licenses/MIT

See https://creativecommons.org/licenses/by/4.0/ for [Twemoji] graphics license.


[Twemoji]: https://github.com/twitter/twemoji
[twemoji-1.0]: https://github.com/LouisT/KiwiIRC-Emoji-Twemoji/tree/twemoji-1.0
[EmojiOne]: https://github.com/Ranks/emojione
[KiwiIRC-Emoji-EmojiOne]: https://github.com/LouisT/KiwiIRC-Emoji-EmojiOne
