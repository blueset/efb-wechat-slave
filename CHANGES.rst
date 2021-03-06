=========
Changelog
=========

All notable changes to this project will be documented in this file.

The format is based on `Keep a Changelog`_, adapted for reStructuredText syntax.
This project adheres to `Semantic Versioning`_-flavored `PEP 440`_.

.. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
.. _PEP 440: https://www.python.org/dev/peps/pep-0440/
.. _Semantic Versioning: https://semver.org/spec/v2.0.0.html

Unreleased
==========

Added
-----

Changed
-------

Removed
-------
- Remove itchat from dependencies as we have already vendor-ed it

Fixed
-----

Known issue
-----------

2.0.4_ - 2020-12-22
===================

Fixed
-----
- Following the latest Bullet API change which caused setup wizard to crash


2.0.3_ - 2020-11-23
===================

Added
-----
- Step-by-step logging for session file and PUID mapping overwrite

Fixed
-----
- Attempt to fix issue where new chat is not properly recognised without
  verification (`#108`_)
- Yet another attempt to fix batch incoming files / videos duplication
- Hide quotation marks when ``max_quote_length`` is set to 0

2.0.2_ - 2020-07-09
===================

Changed
-------
- Some changes to the translation of WeChat emoticon to emoji.

Fixed
-----
- Files may appear with the same content when received at the same time from WeChat
- Wizard should return int instead of float

2.0.1_ - 2020-03-19
===================

Added
-----
- Safely overwrite session files to mitigate loss of data caused by improper
  termination of EWS
- ``text_post_processing`` experimental flag

Fixed
-----
- Experimental features config wizard breaks on multiple choices.
- Use the new 🧧 emoji for ``[红包]`` mapping.

Known issue
-----------

2.0.0_ - 2020-01-31
===================
First release.

.. _2.0.0: https://ews.1a23.studio/releases/tag/v2.0.0
.. _2.0.1: https://ews.1a23.studio/compare/v2.0.0...v2.0.1
.. _2.0.2: https://ews.1a23.studio/compare/v2.0.1...v2.0.2
.. _2.0.3: https://ews.1a23.studio/compare/v2.0.2...v2.0.3
.. _2.0.4: https://ews.1a23.studio/compare/v2.0.3...v2.0.4
.. _#108: https://github.com/ehForwarderBot/efb-wechat-slave/issues/108
