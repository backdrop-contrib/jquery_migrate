# jQuery Migrate Helper

Bundles [jQuery Migrate](https://github.com/jquery/jquery-migrate), a tool
to debug and fix compatibility problems with newer jQuery versions in legacy
projects.

This module's supposed to be used by Backdrop CMS module maintainers to
identify problems in their modules.

See also: https://github.com/backdrop/backdrop-issues/issues/6404

Note that in its current state, this is a dev module only and is not
supposed to be turned on on production sites.
It potentially nags a lot into the browser console.

## What jquery-migrate can do for you

If you maintain a module with legacy code, and you're not sure, if it will
work with the upcoming jQuery 4 version, install this module on your dev
instance, make sure you switch to jQuery v3
(on admin/config/development/jquery) and click through what your module provides.

While doing that, keep an eye on the browser console. jQuery migrate will
provide helpful log info like for example `JQMIGRATE: jQuery.fn.bind() is
deprecated` or `JQMIGRATE: jQuery.isFunction() is deprecated`.
The console trace will help you to find, where those deprecated functions are
used.

Additional info about what to do to fix it can be found in the official
[jQuery API documentation](https://api.jquery.com/category/deprecated/)

## Installation

- Install this module using the official [Backdrop CMS instructions](https://docs.backdropcms.org/documentation/extend-with-modules)

## Issues

Bugs and feature requests should be reported in the [Issue Queue](https://github.com/backdrop-contrib/jquery_migrate/issues)

## Current Maintainers

- [Indigoxela](https://github.com/indigoxela)

## Credits

jQuery Migrate uses a [custom license](https://github.com/jquery/jquery-migrate/blob/main/LICENSE.txt)
and is maintained on GitHub by the same team that also maintains jQuery.

## License

This project is GPL v2 software. See the LICENSE.txt file in this directory for complete text.
