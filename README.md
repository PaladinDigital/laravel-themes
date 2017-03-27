# Laravel Themes

The Laravel Themes project aims to allow developers and designers the ability to create interoperable themes for the laravel 5 framework (from 5.4+).
Similar to how themes can be installed on WordPress this project includes a custom composer installer that can require a theme which can then be used in your application views as a master layout.

## Theme Conventions

All themes MUST have the following layouts:
- master.blade.php

All themes MUST make available the following yields:
 - "content"
 - "sidebar" (sidebar must be yielded however theme authors have discretion over where this is placed, eg: after content would be acceptable)
 
 All themes MUST make available the following stacks:
 - "scripts"
 - "styles"
 - "widgets"
