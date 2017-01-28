# Hugo World
## Hugo site incorporating Kube framework
The plan is to produce this site using *Hugo* static site generator, with styling from *Kube* CSS framework, and serve it via *Netlify* hooked into a *GitHub* repository.
Most of the files, including this one, will use [Markdown syntax](https://daringfireball.net/projects/markdown/syntax "Markdown syntax reference").
### Setting up on a Mac
Mac mini (Late 2014) with OS X 10.10.5 (Yosemite)
#### Install Homebrew
Instructions from [Homebrew](http://brew.sh/ "Homebrew: The missing package manager for macOS") homepage executed without any problems or error messages, `brew update` reported *up-to-date* status.
#### Install Hugo
Following instructions to [install Hugo](https://gohugo.io/tutorials/installing-on-mac/ "Hugo: Installing on a Mac"), ran `brew install hugo`, with successful install reported. Three tests of the Hugo install location and version produced output as described in the instructions.
### Minimal Hugo site
The hope in this project is to produce a functional and responsive website while minimizing dependencies on large external frameworks or other resources that have to be loaded externally. A partial motivation for this approach is to maximize the benefits of static hosting on *Netlify*.

Create a new site called "slug":

	$ hugo new site slug

#### Blank Hugo theme
The [blank](https://github.com/vimux/blank/ "Blank — starter Hugo theme for developers") theme seems like a good starting point for creating a Hugo site that will be subsequently styled via a minimalistic CSS framework. Downloaded the source ZIP and extracted it in `slug/themes` directory as `blank`. 
#### First page: About
Try to make a page and a section, since every site needs an *About* page, it is a good place to start. The tutorial does not yet explain how index pages work, so this version of the page will be named `about`:

	hugo new about/about.md

After editing the MD file to add a title and a line of text as content, the site can be served:

	hugo server --theme=blank --buildDrafts

And it appears at `http://localhost:1313/`
