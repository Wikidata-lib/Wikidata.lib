== PubSubHubbub ==

Two git repos? Not indicated which one is cannonical

* Not using composer
* Global notation
* __DIR__

lib/publisher

* not MW style
* ?>
* http_post should be injected service
** options not really part of that
** service never really different as optional arg in publish_update not used
* needs tests

== PropertySuggester ==

* Not using composer
* global scope assumptions
* __DIR__
* weird indenting

* uses both mw autoloading and include statements
* no tests
* files at random places
* no NS usage, not PSR-0 compliant

GetSuggestions.php

* not just a class! Also include and function
* direct access to StoreFactory

* big methods
* output argument in mergeWithTraditionalSearchResults
* mixed abstraction levels

* lots of stuff inside legacy API

GetMisfits.php

* not just a class! Also include and function
* one big method
* direct construction EntityId instead of ItemId
* weird indenting

Suggesters/SimpleMisfitSuggester

* no escaping in SQL construction! looks like no injection vector present
* database service pulled in
* suggestMisfitsByAttributList to big
* weird array_push usage

Suggesters/SimplePHPSuggester

* no escaping in SQL construction! looks like no injection vector present
* database service pulled in
* suggestionsByAttributeList to big
* unused $i, $key
* $deprecatedPropertyIds not injected

parser/

All python, probably do not want to have this in the PHP lib (new repo)

modules/

ext.PropertySuggester.EntitySelector.js

* tailing comma - please use a linting tool
* unused this._term

ext.PropertySuggester.js

* ext.PropertySuggester.js - global scope - needs review by JS person
* implicitly defined vars

== General suggestions ==

* Seperate concerns and abstraction levels on both method and class level
* Use namespaces and adhere to PSR-0
* Use Composer to manage dependencies
* Use linting tools for both PHP and JS and use a decent editor
* Do not put application or business logic into classes bound to legacy APIs (ie SpecialPage or Api)
* Test all non-glue code
* Add basic documentation in a README(.md) file

Relevant documents

https://www.mediawiki.org/wiki/Wikibase/Coding_conventions
https://www.mediawiki.org/wiki/Wikibase/Contribution_workflow

