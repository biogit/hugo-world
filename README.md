# Hugo World
## Hierarchical Website on Hugo
As a fast static site generator, [Hugo](https://gohugo.io/ "A fast and modern static website engine") is gaining well-deserved popularity. For generating a website with a traditional hierarchical structure of individual pages, however, popular themes and tutorials for *Hugo* unfortunately do not offer easily adaptable solutions, as they tend rather to focus on blogs (or other list-like features) accompanied by a few pages (About, Contact) in a flat structure. Hence, the aim of this project to explore and document the process of generating a multi-level hierarchical website using *Hugo*. This README file will serve to document the process, until the site itself is functional enough to present the information.
### Features
The main concept of this project is to use *Hugo* for generating pages with taxonomies, schema, alternate versions, and various other features of modern HTML and websites, because most of such features can be added via templates and partials to content specified in separate files. The following non-exhaustive list indicates a few of the principles and features that will be used, implemented, or pursued.
* [Barebones HTML5](https://html5bones.com "Barebones HTML5 Template") Template
* Default/minimal styling/formatting (CSS to be added later via themes)
* Mainly use [Markdown](https://daringfireball.net/projects/markdown/syntax "Markdown syntax reference") files
* Google-supported [markup](https://developers.google.com/search/docs/guides/intro-structured-data "Introduction to Structured Data")
* Generate [AMP HTML](https://developers.google.com/search/docs/guides/use-AMP-HTML "Accelerated Mobile Pages") versions of pages
* Use *GitHub* to deploy, host, and manage the source files for *Hugo*
* Use *Hugo* integration offered by *Netlify* to generate a static site

Some of these principles and features are related to future-proofing the site: modern features will enhance SEO and user experience, while site-generator approach would allow to transition the core of the site content, data, and structure to future versions of generators, in case some of the currently popular ones become stagnant or abandoned. Other aspects are more of logistical nature: the combination of *GitHub* and *[Netlify](https://www.netlify.com/ "Fast deployment and hosting of static sites")* would conceptually allow creating a site without the need for a local installation of either *Hugo* or *GitHub* software. *Hugo* is particularly chosen for this project because it is supported by *Netlify* and its speed should introduce only minimal delays in continuous deployment to a *Netlify* static site. 
#### Local Hugo installation
While some developers consider an option of having a local installation of *Hugo* to be beneficial, since the ultimate output is synced to *GitHub*, running *Hugo* locally should not be technically necessary. This would be particularly beneficial for a site where most pages are created once and rarely modified. Functionality related to creating "new" source files from templates would not be a big time-saver in such cases, for example, so some of the configuration and setup files could be omitted from the standard structure of *Hugo* source directories and files.
