# Laravel Themes

The Laravel Themes project aims to allow developers and designers the ability to create interoperable themes for the laravel 5 framework (from 5.4+).

Similar to how themes can be installed on WordPress this project includes a custom composer installer that can require a theme which can then be used in your application views as a master layout.

## Theme Conventions

All themes MUST have the following layouts:
- master.blade.php

All themes MUST make available the following yields:
- "content"
- "sidebar" (sidebar must be yielded however theme authors have discretion over where this is placed, eg: after content would be acceptable)

Themes may optionally make available the following yields:
- "breadcrumbs"
 
All themes MUST make available the following stacks:
- "scripts"
- "styles"
- "widgets"
- "head"
- "before-content"
- "after-content"
- "footer"

## Creating a Theme

To create a theme start by initialising a new composer package with the following properties:

     "type": "laravel-community-theme",     
     "require": {
       "paladindigital/laravel-theme-installer": "dev-master",
       "paladindigital/laravel-theme-loader": "dev-master"
     },
     "keywords": [
       "laravel-community-theme"
     ]

## Contributing

If you have idea's how we can improve this project please feel free to raise an issue, the goal is to give end users and developers access to a pool of themes that all work in the same way to prevent the need to reinvent the wheel repeatedly.
