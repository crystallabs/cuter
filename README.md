**Build status**: [![Build Status](https://travis-ci.com/crystallabs/cuter.svg?branch=master)](https://travis-ci.com/crystallabs/cuter)
[![Version](https://img.shields.io/github/tag/crystallabs/cuter.svg?maxAge=360)](https://github.com/crystallabs/cuter/releases/latest)
[![License](https://img.shields.io/github/license/crystallabs/cuter.svg)](https://github.com/crystallabs/cuter/blob/master/LICENSE)

**Project status**: `[X] Being developed  [ ] Usable  [ ] Functionally complete`

Crystime is an "overlay" for Papierkorb's [cute](https://github.com/Papierkorb/cute) which modifies some of its built in behavior. Specifically, it changes or adds the following:

* blocks return Bool instead of nil
* signals know their @parent
* signals support one-time trigger via @listeners1
* every emit() also emits signal "event"
* every on() emits signal new_listener unless new_listener itself is added
* every off() emits signal remove_listener
* emit() and emit2() mimick _emit() and emit() from Blessed

And some other changes are included or are coming up.

In essence, this is a specialized module aiming to duplicate [Blessed](https://github.com/chjj/blessed)'s event model, and is probably not usable outside of it, due to specific and contextualized behavior.