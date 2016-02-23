# IMPORTANT

This project is a proof of concept, for further discussions. See links below!

Feedback very welcome!!

# Major Goals

 - Use a build / test robot to automatically create and deploy the static site
 - Create a project, that can be easily cloned and used
 - Create a simple interface to achieve the basic tasks
 - Use tiddlywiki.js as a static site generator
 - Use a very simple CSS framework (purecss.io)
   - use just enough to get the page started
   - no js framework should be needed
 - The created content should be responsive
 - The workflow should be generic, so it can be re-used for several tasks. 
 - .. 
 
## Dependencies

 - For Windows users you should have installed [git for windows](https://git-scm.com/)
 - gitbash is expected to work atm. 
   - this dependency should be removed. It's only needed for `deploy-gh-pages.sh`

# Discussion Links

-todo-

# Languages
This repo contains a landing page for language specific TW documentation. Releases are independent to the core release cycle. The page layout is based on a blogging page. .. I thought, this would be a good fit.

## Structure

Existing language specific TWs cand be found at: 

 - tiddlywiki.com/languages/ ... this project ... autocreated by travis from branch `gh-pages`
 - tiddlywiki.com/languages/de-DE ... german Germany ... curated by @pmario
 - tiddlywiki.com/languages/de-AT ... german Austria ... curated by @pmario
 - tiddlywiki.com/languages/de-FR ... frensh France ... curated by @xcazin
 - tiddlywiki.com/languages/de-zh-Hans ... chinese simplified ... curated by @BramChen
 - tiddlywiki.com/languages/de-zh-Hant ... chinese traditional ... curated by @BramChen

## Important

The resulting page content can only be seen if you select the ["gh-pages" branch](https://github.com/TiddlyWiki/languages/tree/gh-pages).

## How to Contribute

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

List the possible commands: 

```
npm run
```

Run the whole development environment:

```
npm run dev
```

Build `static.html` and `static.css` once. The output directory is `/editions/index/output`

```
npm run build
```

The whole process was heavily inspired by the blog post: [How to Use npm as a Build Tool](http://blog.keithcirkel.co.uk/how-to-use-npm-as-a-build-tool/). I think it's worth a read, because you'll understand, why this project is as it is :)

There is a [`package.json`](https://github.com/TiddlyWiki/languages/blob/master/package.json) file, which creates several commands: 

 - "dev":
   - builds the static page version. 
   - starts a tiddlywiki server
   - starts a watch server to auto re-build the static version
   - starts a live reload server that watches the static files
 - "static": starts a small dev file server, that hosts static.html and local files 
 - "start": starts the tiddlywiki server
 - "watch": starts a watch process, that auto re-builds the static files
 - "test": -- no tests atm --
 - "build": Build the static files using TiddlyWiki
 - "deploy": build and deploys the whole stuff from CLI and with Travis
 - "livereload": triggers browser live-reload of the static content if it was changed

## Rules for Contributing 

Just to be sure. This is a proof of concept software, with a lot of room for improvements. So absolutely everything can and will be changed. ... All templates will be renamed!!

see: https://github.com/Jermolene/TiddlyWiki5/blob/master/contributing.md

## Licenses

see: https://github.com/Jermolene/TiddlyWiki5/tree/master/licenses

Important for documentation see: https://github.com/Jermolene/TiddlyWiki5/blob/master/licenses/cla-individual.md#23-outbound-license
