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
* Dark Mode
* Search & Tag archive
* Post reading progress
* Disqus support
* Code highlight support – [Prism.js](https://prismjs.com/) v1.21.0
* LaTeX support – [KaTeX](https://katex.org/) v0.12.0

## 🕶 About **Dark Mode**

In `style.scss`:
  * To make it up to the browser, use `dark` in all `prefers-color-scheme`. This is the default behaviour.
  * To disable it, use `no-preference` in all `prefers-color-scheme`.
  * To enforce it, extract all properties within `@media (prefers-color-scheme: ...)`.

## 🌍 Localization

* __English__
* __German__
* __Spanish__
* __French__ by [robink](https://github.com/robink)
* __Italian__ by [fmaida](https://github.com/fmaida)
* __Norwegian__ by [arthurnoerve](https://github.com/arthurnoerve), [oisann](https://github.com/oisann)
* __Chinese__ by [hao-lee](https://github.com/hao-lee)
* __Indonesian__ by [simplyeazy](https://github.com/simplyeazy)
* __Romanian__ by [cdorin93](https://github.com/cdorin93)
* __Russian__ by [schamberg97](https://github.com/schamberg97)
* __Turkish__ by [cgrgrbz](https://github.com/cgrgrbz)
* __Swedish__ by [martenj77](https://github.com/martenj77)
* __Czech__ by [lunakv](https://github.com/lunakv)
* __Portuguese__ by [matheusvanzan](https://github.com/matheusvanzan)
* __Vietnamese__ by [JustHmmmm](https://github.com/justhmmmm)
* __Greek__ by [thiodordelis](https://github.com/thiodordelis)
* __Danish__ by [jmayntzhusen](https://github.com/jmayntzhusen)
* __Arabic__ by [pop-eax](https://github.com/pop-eax)
* __Catalan__ by [arthurnoerve](https://github.com/arthurnoerve)
* __Lithuanian__ by [arthurnoerve](https://github.com/arthurnoerve)
* __Dutch__ by [gkdp](https://github.com/gkdp)
* __Polish__ by [filipolszewski](https://github.com/filipolszewski)

## 🎨 Setup custom color

1. Go to __Code injection__.  
2. Add this to __Blog Header__:  
````
<style>
  :root {
    --color-primary: #D95736;
    --color-primary-active: #BF4526;
  }
</style>
````

## 🔠 Setup custom google fonts

1. Go to [fonts.google.com](https://fonts.google.com/) and choose a font.
2. Choose __Embed__ and copy the `<link>` code.
3. Go to __Code injection__.  
4. Add this to __Blog Header__:  
````
<link href="https://fonts.googleapis.com/css2?family=Mukta&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Crimson+Text&display=swap" rel="stylesheet">
<style>
  :root {
    --font-primary: 'Mukta', sans-serif;
    --font-secondary: 'Crimson Text', serif;
  }
</style>
````

## 💬 Setup [Disqus](https://disqus.com/)

1. Go to __Code injection__.
2. Add this to __Blog Header__:
````
<script>var disqus = 'YOUR_DISQUS_SHORTNAME';</script>
````

## 🔍 Setup search

The search function is build with [ghostHunter](https://github.com/jamalneufeld/ghostHunter):

1. Go to __Integrations__.  
2. Choose __Add custom integration__, name it `ghostHunter` and choose __Create__. Copy the generated Content API Key.  
3. Go to __Code injection__.  
4. Add this to __Blog Header__:  
````
<script>
  var ghosthunter_key = 'PASTE_THE_GENERATED_KEY_HERE';
  //optional: set your custom ghost_root url, default is "/ghost/api/v2"
  var ghost_root_url = '/ghost/api/v2';
</script>
````
## ⚙️ Development

Install [Grunt](https://gruntjs.com/getting-started/):

	npm install -g grunt-cli

Install Grunt dependencies:

	npm install [-g npm@latest]

Build Grunt project:

	grunt build

The compress Grunt task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

	grunt compress

## ⚖️ Copyright & License

### Pegasus
Copyright (C) 2020 Christian Chomiak - Released under the [MIT License](https://github.com/christianchomiak/pegasus/blob/master/LICENSE).

### Attila
Copyright (C) 2015-2020 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/attila/blob/master/LICENSE).
