# Release Notes

## Version 3.1 (October 2024)

- Installatble with PHP 8.1+

## Version 3.0 (23 October 2021)

- Installable with 7.4+ (including PHP8)
- Typing added throughout
- PSR4 namespacing. Now in `Addwiki\Mediawiki\Datamodel`

## Version 2.8 (16 February 2021)

- Installable with 7.3+ (including PHP8)

## Version 2.7 (15 February 2021)

- No notable changes

## Version 2.6 (2 February 2021)

- Require PHP 7.2+
- Initial release from new development monorepo
- All addwiki libraries now have aligned version numbers

## Version 0.8 (30th July 2018)

* Add 'maxlag' as 4th parameter to EditInfo constructor
* Add `EditInfo`::`getMaxlag`

## Version 0.7.1 (10th January 2017)

* [T184567](https://phabricator.wikimedia.org/T184567) `User` objects can now be created with a `null` `$registration`.

## Version 0.7 (8th March 2017)

### New features

* Add NamespaceInfo class 

## Version 0.6 (2015-09-04)

### Compatibility  changes

* Log object now takes a PageIdentifier object instead of a Page object

### Deprecations

* Title::getTitle is deprecated

### New features

* Implemented File class
* Implemented Redirect class
* Title::getText introduced to replace getTitle
* Log now implements JsonSerializable
* LogList now implements JsonSerializable
* Title now implements JsonSerializable
* PageIdentifier now implements JsonSerializable

## Version 0.5 (2015-01-13)

### Compatibility  changes

* Revision objects now require a PageIdentifier object instead of a $pageId int
* Page objects now require a PageIdentifier objects instead of a $title and $pageId
* Content getNativeData renamed to getData
* Content constructor changed, now takes data and optional model
* Content has new method getModel in places of random constants
* Removed WikitextContent class. Content is no longer abstract.

### New features

* Implemented Log class
* Implemented LogList class
* Introduce PageIdentifier class
* Page objects can be constructed without a Revisions object

## Version 0.4 (2014-07-08)

* Page objects now ONLY accept a Title object for $title in their constructor.
* InvalidArgumentExceptions are now thrown when objects are constructed with the wrong types.
* User objects now split up implicitgroups and regular groups, thus $groups is now array[]

## Version 0.3 (2014-06-24)

### Compatibility  changes

* Revision objects now take a Content object as $content

### Additions

* Content class
* WikitextContent class
* Pages class


## Version 0.2 (2014-02-23)

### Compatibility  changes

* Revision enhanced to allow more flexibility, Constructor and public functions have changed
* contentmodel has been removed from the Page class

## Version 0.1 (2014-02-23)

Initial release with the following features:

* EditInfo
* Page
* Revision
* Revisions
* Title
* User
