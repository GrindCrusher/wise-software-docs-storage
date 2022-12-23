# Welcome to Your Gift

I've built a documentation website for you to use to document Pool Program 9, and other products.

# Features

- [x] **Almost 0 configuration.** Routes, group names, and page names are all file based. 
- [x] **Multiple environment support.** Keep separate products' documentation separate. Users can choose the current environment by clicking the text next to the Wise Software logo. Try clicking on Retail to see it in action.
- [x] **Markdown support.** Everything is written in Markdown. You can see everything this website currently supports on the [Elements](/enterprise/markdown/elements) page.
- [x] ***Extended* Markdown support.** There's already a few elements that are custom made, which you can see over on the [Custom Elements](/enterprise/markdown/custom-elements) page. You can directly embed YouTube videos (for stuff like video tutorials), or have callouts that display important information. 
- [x] **Extensible.** Being a custom site, I can add anything needed. Custom elements, etc.
- [x] **100% free.** All content is stored on a GitHub repository, while the website is hosted on the Cloud over at [Vercel](https://vercel.com/) for free.
- [x] **Super search support** (TBA)**.** I plan to add [Algolia](https://algolia.com) Search, which is free for up to about 10,000 searches a month. 
- [x] **Themes.** You can switch between System, Dark, and Light theme. Additionally, you can choose between a Serif or a Sans-Serif font.
- [x] **Mobile support.** Mobile is supported! Try this on your phone if you're not already on it.

## Basic Layout

You start out with an environment—a collection of groups and pages that relate to the same product. Each environment supports groups, which then contain pages. Groups and their respective pages are laid out to the side of the page (on your left). An environment would be a folder, and have its metadata (title, description, and image) defined in a central `structure.yml` file. There is no configuration other than that. Each environment has a homepage, which would map to the `index.md` file inside the environment folder. Each group in an environment would be another folder inside that environment folder, and each page would be a `page-name.md` file inside that group.

For instance, this page is under `enterprise/index.md`. 
