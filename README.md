# Obsidian Noor Plugin

[Noor](https://github.com/MKSherbini/obsidian-noor) is a plugin for [Obsidian.md](https://obsidian.md/). It aims to help muslims stay enlightened with Islam, Quran, Hadith, and Sunnah

[![Watch the video](https://img.youtube.com/vi/eKgS6iop58Q/maxresdefault.jpg)](https://youtu.be/eKgS6iop58Q)



## Features
- Insert a **Quran Quote** at the current location containing a random verse with recitation in Arabic, chosen translation language, and a hyperlink for more info.
- Insert a **Hadith Quote** at the current location containing a random hadith in chosen language and a hyperlink for more info.

## Usage
After enabling the plugin in the settings menu, you should see the added commands and the `noorJS` object.

- commands:
  - `Noor: Random Quran quote`: inserts a quote block at the current editor location containing a Quran Quote
  - `Noor: Random Hadith quote`: inserts a quote block at the current editor location containing a Hadith Quote
- scripting:
  - `noorJS.randomQuranQuote()`: this function returns a Quran Quote
  - `noorJS.randomHadithQuote()`: this function returns a Hadith Quote


## Integration with other plugins

obsidian plugins complement each other, here are some ideas
- **with [templater](https://github.com/SilentVoid13/Templater)**: use `<% noorJS.randomQuranQuote() %>` to insert the Quran quote into your notes (like the daily note to get a daily verse)
- **with [commander](https://github.com/phibr0/obsidian-commander)**: use it to create a button for the `Noor: Random Quran quote` command


## Settings

### Quran settings
- **Reciter**: choose your favorite reciter from the drop-down menu
- **Translation Language**: choose the second language to show next to Arabic
- **Translation Options**: choose your favorite translation from the ones available in selected **Translation Language**

### Hadith settings
- **Hadith language**: choose your preferred language to show the hadith in.


## Manually installing the plugin

- Copy over `main.js`, `manifest.json` to your vault `.obsidian/plugins/noor/`.
- Reload Obsidian to load the new version of your plugin.
- Enable plugin in settings window.


## Attributions

### AlQuran Cloud APIs

The Quran verses are retrieved from
- [alquran.cloud](https://alquran.cloud/api): An opensource Quran API made by the [Islamic Network](https://islamic.network/) ([github](https://github.com/islamic-network)) and respective [contributors](https://alquran.cloud/contributors).

### Hadith Encyclopedia APIs

The Hadith quotes are retrieved from

- [hadeethenc.com](https://hadeethenc.com/api-docs/): Encyclopedia of Translated Prophetic Hadiths.

## Contributions and suggestions
Please feel free to open a [pull request](https://github.com/MKSherbini/obsidian-noor/pulls) with suggested improvements and new feature requests
