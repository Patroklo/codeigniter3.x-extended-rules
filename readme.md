# CodeIgniter extended rules

A set of useful form validation rules, focused on file uploading (and some more). English corrections and other languages are welcome.

Written by Joseba Juaniz ([@Patroklo](http://twitter.com/Patroklo)) and Jeroen van Meerendonk ([@jeroen_bz](http://twitter.com/jeroen_bz)).
Original code written by **devbro** (devbro@devbro.com).


## Requirements

Codeigniter 3.x 
Php 5.3 or above.


## Installation

Just put copy the files into your server using the same folder structure. If you already have an english language file,
open it and add the content of `/application/language/english/form_validation_lang.php`, and do the same with the other
languages.


## Rules

Use them as the other rules.

* `file_required` Checks if the a required file is uploaded.
* `file_size_max[size]` Returns FALSE if the file is bigger than the given size.
* `file_size_min[size]` Returns FALSE if the file is smaller than the given size.
* `file_allowed_type[type]` Tests the file extension for valid file types. You can put a group too (image, application, word_document, code, zip).
* `file_disallowed_type[type]` Tests the file extension for no-valid file types
* `file_image_maxdim[x,y]` Returns FALSE if the image is smaller than given dimension.
* `file_image_mindim[x,y]` Returns FALSE if the image is bigger than given dimension.
* `file_image_exactdim[x,y]` Returns FALSE if the image is not the given dimension.
* `is_exactly[list]` Check if the field's value is in the list.
* `is_not[list]` Check if the field's value is not permitted.


## Change Log

### 3.2
* Changed `valid_hour`rule to accept 24 and 12 hour format
* Changed `file_allowed_type` and `file_disallowed_type` to use Mime type when possible instead of extension file.
* Added more spanish and english translations.

### 3.1
* Add `valid_hour`rule.

### 3.0
* Upgraded and working with CodeIgniter 2.1.
* Separated the error messages from the library and move them to `/application/language`
* Added `is_exactly` and `is_not` rules.
* Added spanish translation.


### 2.1.0

* Fixed the issue: http://codeigniter.com/forums/viewthread/123816/P30/#629711 (by devbro)