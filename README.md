# Pegasus

A content focused responsive theme for [Ghost](https://github.com/tryghost/ghost/), based on [Attila](https://github.com/zutrinken/attila).

## 📷 Screenshots

<table>
<tr>
<td valign="top">
<img src="https://raw.githubusercontent.com/christianchomiak/pegasus/master/src/screenshot-desktop.jpg" />
</td>
<td valign="top">
<img src="https://raw.githubusercontent.com/christianchomiak/pegasus/master/src/screenshot-mobile.jpg" />
</td>
</tr>
</table>

## ⭐️ Features

* Responsive layout
* Dark Mode & Theme Switch
* Search & Popular Tags
* Post reading progress
* Disqus support
* Member menu buttons
* Ghost accent color
* Code highlight support – [Prism.js](https://prismjs.com/) v1.23.0
* LaTeX support – [KaTeX](https://katex.org/) v0.13.10

## 🌍 Localization

🟩 Up to date  🟧 Missing strings

| Code | Flag | Language | Status | Translator |
| :--: | :--: | :------: | :----: | :--------: |
| `en` | 🇬🇧 | English | 🟩 | |
| `de` | 🇩🇪 | German | 🟩 | |
| `es` | 🇪🇸 | Spanish | 🟩 | [r1p](https://github.com/r1p) |
| `fr` | 🇫🇷 | French | 🟧 | [robink](https://github.com/robink) |
| `it` | 🇮🇹 | Italian | 🟧 | [fmaida](https://github.com/fmaida) |
| `no` | 🇳🇴 | Norwegian | 🟧 | [arthurnoerve](https://github.com/arthurnoerve), [oisann](https://github.com/oisann) |
| `zh` | 🇨🇳 | Chinese | 🟩 | [hao-lee](https://github.com/hao-lee), [izumiko](https://github.com/izumiko) |
| `id` | 🇮🇩 | Indonesian | 🟧 | [simplyeazy](https://github.com/simplyeazy) |
| `ro` | 🇷🇴 | Romanian | 🟧 | [cdorin93](https://github.com/cdorin93) |
| `ru` | 🇷🇺 | Russian | 🟧 | [schamberg97](https://github.com/schamberg97) |
| `tr` | 🇹🇷 | Turkish | 🟩 | [cgrgrbz](https://github.com/cgrgrbz), [electricalgorithm](https://github.com/electricalgorithm) |
| `sv` | 🇸🇪 | Swedish | 🟧 | [martenj77](https://github.com/martenj77) |
| `cs` | 🇨🇿 | Czech | 🟧 | [lunakv](https://github.com/lunakv) |
| `pt` | 🇵🇹 | Portuguese | 🟧 | [matheusvanzan](https://github.com/matheusvanzan) |
| `vi` | 🇻🇳 | Vietnamese | 🟧 | [JustHmmmm](https://github.com/justhmmmm) |
| `el` | 🇬🇷 | Greek | 🟧 | [thiodordelis](https://github.com/thiodordelis) |
| `dk` | 🇩🇰 | Danish | 🟧 | [jmayntzhusen](https://github.com/jmayntzhusen) |
| `ar` | | Arabic | 🟧 | [pop-eax](https://github.com/pop-eax) |
| `ca` | | Catalan | 🟧 | [arthurnoerve](https://github.com/arthurnoerve) |
| `lt` | 🇱🇹 | Lithuanian | 🟧 | [arthurnoerve](https://github.com/arthurnoerve) |
| `nl` | 🇳🇱 | Dutch | 🟧 | [gkdp](https://github.com/gkdp) |
| `pl` | 🇵🇱 | Polish | 🟩 | [filipolszewski](https://github.com/filipolszewski), [MrBoombastic](https://github.com/mrboombastic) |
| `eo` | | Esperanto | 🟧 | [ebanDev](https://github.com/ebanDev) |
| `ga` | | Galego | 🟩 | [r1p](https://github.com/r1p) |

## Show subscribe / account button in navigation

1. Go to `partials/navigation-meta.hbs`.
2. Remove comments on line `24`and `34`.

## 🔠 Setup custom google fonts

1. Go to [fonts.google.com](https://fonts.google.com/) and choose a font.
2. Choose __Embed__ and copy the `<link>` code.
3. Go to __Code injection__.  
4. Add this to __Blog Header__:  
````html
<link href="https://fonts.googleapis.com/css2?family=Mukta&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Crimson+Text&display=swap" rel="stylesheet">
<style>
  :root {
    --font-primary: 'Mukta', sans-serif;
    --font-secondary: 'Crimson Text', serif;
    --font-code: 'Roboto Mono', monospace;
  }
</style>
````

## 💬 Setup [Disqus](https://disqus.com/)

1. Go to __Code injection__.
2. Add this to __Blog Header__:
````html
<script>var disqus = 'YOUR_DISQUS_SHORTNAME';</script>
````

## 🔍 Setup search

1. Go to __Integrations__.  
2. Choose __Add custom integration__, name it `Search` and choose __Create__. Copy the generated Content API Key.  
3. Go to __Code injection__.  
4. Add this to __Site Header__:  
````html
<script>
  var gh_search_key = 'API_KEY';
  var gh_search_migration = 'v2';
</script>
````
## ⚙️ Development

Install [Grunt](https://gruntjs.com/getting-started/):
````bash
npm install -g grunt-cli
````
Install Grunt dependencies:
````bash
npm install [-g npm@latest]
````
Build Grunt project:
````bash
grunt build
````
The compress Grunt task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.
````bash
grunt compress
````
## ⚖️ Copyright & License

### Pegasus
Copyright (C) 2020-2021 Christian Chomiak - Released under the [MIT License](https://github.com/christianchomiak/pegasus/blob/master/LICENSE).

### Attila
Copyright (C) 2015-2021 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/attila/blob/master/LICENSE).
