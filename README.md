# SCSS Project Starter

This starter contains a folder structure that i normally use when starting a new project. This is not a framework, but more of a style guide. The architecture used is a variation of the 7-1 pattern (https://sass-guidelin.es/#architecture), with the BEM (block__element--modifier) methodology used for styling (http://getbem.com/). 


## Getting Started

Just copy the styles folder in your project.


### Folder Structure

* The pattern consits of 7 folders with partials and one main file where all are imported;
* The 7 folders are: abstracts, base, components, layout, pages, themes and vendors;

```
styles/
|
|– abstracts/
|   |– _variables.scss      # Sass Variables
|   |– _functions.scss      # Sass Functions
|   |– _mixins.scss         # Sass Mixins
|   |– _placeholders.scss   # Sass Placeholders
|   |– _extends.scss        # Sass Extends
|   |– _media.scss          # Media breakpoints
|
|– base/
|   |– _reset.scss          # Reset/normalize
|   |– _typography.scss     # Typography rules
|   …                       # Etc.
|
|– components/
|   |– _buttons.scss        # Buttons
|   |– _carousel.scss       # Carousel
|   |– _cover.scss          # Cover
|   |– _dropdown.scss       # Dropdown
|   …                       # Etc.
|
|– layout/
|   |– _navigation.scss     # Navigation
|   |– _grid.scss           # Grid system
|   |– _header.scss         # Header
|   |– _footer.scss         # Footer
|   |– _sidebar.scss        # Sidebar
|   |– _forms.scss          # Forms
|   …                       # Etc.
|
|– pages/
|   |– _home.scss           # Home specific styles
|   |– _contact.scss        # Contact specific styles
|   …                       # Etc.
|
|– themes/
|   |– _theme.scss          # Default theme
|   |– _admin.scss          # Admin theme
|   …                       # Etc.
|
|– vendors/
|   |– _bootstrap.scss      # Bootstrap
|   |– _jquery-ui.scss      # jQuery UI
|   …                       # Etc.
|
|- _shame.scss              # Shame file
|– main.scss                # Main Sass file
```


* The styles/ folder will also consist of a shame file, ```_shame.scss```; the concept was made popular by Harry Roberts, Dave Rupert and Chris Coyier, 
and it consists of putting all CSS declarations, hacks and things we are not proud of in this file;
* The main.scss file will only consist of imports and comments; the contents of this file will be compiled into a main.css that will be added in the project;
* When importing partials in the main.scss file, it is recommended to keep the order of the folders:

![Main_scss](/main_scss.png)


## Utility Last

I also included a folder / file for utility classes, that still follow the BEM methodology / semanthics (--hidden, --align-left, --justify-center, etc.); these modifiers can be added as you would normally do on your classes, but since they need to overwrite the block styling they need to be imported in the bottom / end of the main.scss file.




## Acknowledgements

The folder architecture was mostly based on the Sass Guidelines, written by Hugo Giraudel, but there were also other articles / repositories that played a part in inspiring this structure:

- [Sass Guidelines](https://sass-guidelin.es/#architecture), by [Hugo Giraudel](https://hugogiraudel.com/)
- [Architecture for a Sass Project](http://www.sitepoint.com/architecture-sass-project/), by [Hugo Giraudel](https://hugogiraudel.com/)
- [Structuring your Sass Projects](https://itnext.io/structuring-your-sass-projects-c8d41fa55ed4), by [Timothy Robards](https://itnext.io/@timothyrobards)
- [Sass Structure](https://github.com/Ignia/Sass-Structure), by [Ignia](https://github.com/Ignia)
