# SASS

A v.lightweight SASS Framework to leverage SASS features whilst handling the cascade, working in partial files (and a style directory) as well as build a resource of objects.

Assumptions:

* main.scss compiles to main.css in the parent directory
* old-ie.scss imports main.scss up to a chosen breakpoint
* Library and Objects should only constitute framework-wide changes
* A developer updates the config partials then builds the site in styles partials
* font-icons.scss references a fonts folder in assets


## SCSS Directory Structure and Files

* **Library (untouched)**
    * Defaults
    * **Base**
        * Global
        * Headings
        * Paragraphs
        * Blockquotes
        * Images
        * Forms
        * Lists
        * Tables
    * Helpers
    * Print
    * Mixins
    * **Dependencies**
        * Normalise
        * MQ
        * Mixin-library
* **Objects**
     * nav
     * media
     * button
     * font-icons
* **Config** (project specific)
     * setup true:false
     * mq
     * variables (colours, fonts/font-icon-set)
* **Styles**
     * global (html, body, site objects)
     * header
     * navs
     * main
     * aside
     * footer
     * page-gallery (example)
     * block-accordian (example)
     * **Modules**
          * slider (example)
          * gallery (example)
* **Extensions** (extensions to library or objects that aren't content related)
     * ext-forms (example)
     * ext-button (example)
* **Themes** (colour themes)
     * site-themes
     * page-themes
     * module-themes
* **Overrides** (ie styles or similar)
     * make use of the cascade


## References

- https://github.com/csswizardry/inuit.css
- http://smacss.com/
