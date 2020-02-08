# Pegasus

A content focused responsive theme for [Ghost](https://github.com/tryghost/ghost/), based on [Attila](https://github.com/zutrinken/attila).

## Screenshots

<table>
<tr>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/attila/master/src/screenshot-desktop.jpg" />
</td>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/attila/master/src/screenshot-mobile.jpg" />
</td>
</tr>
</table>

## Features

* Responsive layout
* Dark Mode – In `style.scss`, replace `prefers-color-scheme: no-preference` with `prefers-color-scheme: dark`
* Search
* Post reading progress
* Code highlight including line numbers
* Disqus support
* LaTeX support using [KaTeX](https://katex.org/)

## Backlog

* Dark Mode toggling

## Localization

* __English__
* __German__
* __Spanish__
* __French__ by [robink](https://github.com/robink)
* __Italian__ by [fmaida](https://github.com/fmaida)
* __Norwegian__ by [arthurnoerve](https://github.com/arthurnoerve)
* __Chinese__ by [hao-lee](https://github.com/hao-lee)
* __Indonesian__ by [simplyeazy](https://github.com/simplyeazy)
* __Romanian__ by [cdorin93](https://github.com/cdorin93)
* __Russian__ by [schamberg97](https://github.com/schamberg97)
* __Turkish__ by [cgrgrbz](https://github.com/cgrgrbz)
* __Swedish__ by [martenj77](https://github.com/martenj77)

## Setup [Disqus](https://disqus.com/)

1. Go to __Code injection__.
2. Add this to __Blog Header__:
````
<script>var disqus = 'YOUR_DISQUS_SHORTNAME';</script>
````

## Setup search

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
## Development

Install [Grunt](https://gruntjs.com/getting-started/):

	npm install -g grunt-cli

Install Grunt dependencies:

	npm install

Build Grunt project:

	grunt build

The compress Grunt task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

	grunt compress

## Copyright & License

### Pegasus
Copyright (C) 2020 Christian Chomiak - Released under the [MIT License](https://github.com/christianchomiak/pegasus/blob/master/LICENSE).

### Attila
Copyright (C) 2015-2020 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/attila/blob/master/LICENSE).
