Motivation
==========
The current method of retrieving updates involves the MediaWiki extension [OAIRepository](http://www.mediawiki.org/wiki/Extension:OAIRepository) and the OAI-PMH protocol.
Since the deployment of the extension is supposed to be phased out soon, we need a replacement.
Our idea is to use PubSubHubbub instead, which uses a pushing mechanism, instead of requiring subscribers to use [polling](http://code.google.com/p/pubsubhubbub/wiki/WhyPollingSucks).

Links
=====
- [Reference project of PubSubHubbub](http://code.google.com/p/pubsubhubbub/)
- [Protocol specs](https://pubsubhubbub.googlecode.com/git/pubsubhubbub-core-0.4.html)
- [Hub implementations](http://code.google.com/p/pubsubhubbub/wiki/Hubs)

Implementation
==============
- MediaWiki extension
- Publishes arbitrary changes to a predefined "Hub"