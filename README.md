# Google Translate via CLI

Translate texts using Google Translate from your terminal.

## Installation
```
npm install -g google-translate-cli-multi
```
## Usage overview
```
  Usage: translate-m [options] <text ...>

  Options:

    -h, --help               output usage information
    -V, --version            output the version number
    -a, --auto               Auto-detect source language
    -d, --details            View details
    -l, --list               List all available languages
    -s, --source [language]  Source language [en]
    -t, --target [language],[language],[language]  Target languages [es]

  Examples:

     $ translate-m 'I want to translate this text'
     $ translate-m -s es -t en,it 'Quiero traducir este texto'
     $ translate-m -s en -t es,de I want to translate this text
     $ translate-m -a 'Au revoir' -d
     $ pbpaste | translate # when text stored in Mac clipboard
```
Translations from English to Spanish by default.

## Examples
![Command examples](https://cloud.githubusercontent.com/assets/3829533/16347285/26f72b3e-3a4c-11e6-97e8-26ad3d02dc4f.png)

## Default options
Default languages supported by using environment variables (thanks to **@michaelsavich**):
```
export JA_GTC_SOURCE='en' # your preferred source language code
export JA_GTC_TARGET='es' # your preferred target language code
```
If those environment variables are not set then translations from English to Spanish by default.

## TODO
* ~~Add editable default options~~
* Add tests
