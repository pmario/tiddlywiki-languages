# IMPORTANT

This repo is for test purposes only. ... Feedback welcome!!

# Languages
This repo contains a proof of concept landing page for language specific TW documentation. Releases are independent to the core release cycle.

## Structure

Existing language specific TWs cand be found at: 

 - tiddlywiki.com/languages/ ... todo landing page ... autocreated by github from branch `gh-pages`
 - tiddlywiki.com/languages/de-DE ... german Germany ... will be curated by @pmario
 - tiddlywiki.com/languages/de-AT ... german Austria ... will be curated by @pmario
 - tiddlywiki.com/languages/de-FR ... frensh France ... curated by @xcazin
 - tiddlywiki.com/languages/de-zh-Hans ... chinese simplified ... curated by @BramChen
 - tiddlywiki.com/languages/de-zh-Hant ... chinese traditional ... curated by @BramChen

## Important

The resulting page can only be seen if you select the "gh-pages" branch: https://github.com/TiddlyWiki/languages/tree/gh-pages 

## Contribute to Languages Repo

 - Fork this repo

```
git clone ... 
cd <to working directory>
npm install
npm run dev
```

`localhost:3000/static.hmtl` .. shows the static files and auto-reloads if changed
`localhost:8080` .. serves the default tiddlywiki (no autoreload here atm!)

### Prepare a pull request

- Fork this repo
- Make sure you know the "Rules for Contribugint"

```
git clone <from your github repo>

git checkout -b <your feature branch here>
git add .
git commit -m "some useful text here"
git push origin <your feature branch here>

# create a pull request
```

## Command Line Interface

There is a [`package.json`](https://github.com/TiddlyWiki/languages/blob/master/package.json) file, which creates several commands: 

 - "dev": builds the static page version. 
   - starts a tiddlywiki server
   - starts a watch server to auto re-build the static version
   - starts 
 - "static": starts a small dev file server, that hosts static.html and local files 
 - "start": starts the tiddlywiki server
 - "watch": starts a watch process, that auto re-builds the static files
 - "test": -- no tests atm --
 - "build": Build the static files using TiddlyWiki
 - "deploy": build and deploys the whole stuff from CLI and with Travis
 - "livereload": triggers browser live-reload of the static content if it was changed

## Rules for Contributing 

see: https://github.com/Jermolene/TiddlyWiki5/blob/master/contributing.md

## Licenses

see: https://github.com/Jermolene/TiddlyWiki5/tree/master/licenses

Important for documentation see: https://github.com/Jermolene/TiddlyWiki5/blob/master/licenses/cla-individual.md#23-outbound-license
