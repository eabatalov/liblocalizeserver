## Description

Lets you load dictionaries for several locales once and then don't care about detecting the suitable locale by hand. 
When you need a string the library will return it already localized.

## API
### init(options, callback)

Loads the dictionaries you need(you should specify them in `options` parameter), runs `callback` when finished. 
Should be called before the first use of `get` function.

### get(key, dynamicSubstringsDict, options)

Returns the localized string corresponding to the specified key. Dynamic substrings will be inserted where needed.

The locale of the returned string is determined depending on specified options
(there are several forms of `options` parameter supported).

## Install

`npm install git+https://git@github.com/LizaTretyakova/liblocalizeserver.git`
