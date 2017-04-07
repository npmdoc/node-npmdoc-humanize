# api documentation for  [humanize (v0.0.9)](https://github.com/taijinlee/humanize)  [![npm package](https://img.shields.io/npm/v/npmdoc-humanize.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-humanize) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-humanize.svg)](https://travis-ci.org/npmdoc/node-npmdoc-humanize)
#### Javascript string formatter for human readability

[![NPM](https://nodei.co/npm/humanize.png?downloads=true)](https://www.npmjs.com/package/humanize)

[![apidoc](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-humanize_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-humanize/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tai-Jin Lee",
        "email": "taijin@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/taijinlee/humanize/issues"
    },
    "dependencies": {},
    "description": "Javascript string formatter for human readability",
    "devDependencies": {
        "jshint": "0.7.1",
        "mocha": "1.0.3",
        "should": "0.6.3"
    },
    "directories": {},
    "dist": {
        "shasum": "1994ffaecdfe9c441ed2bdac7452b7bb4c9e41a4",
        "tarball": "https://registry.npmjs.org/humanize/-/humanize-0.0.9.tgz"
    },
    "engines": {
        "node": "*"
    },
    "homepage": "https://github.com/taijinlee/humanize",
    "keywords": [
        "util",
        "client",
        "browser"
    ],
    "main": "humanize.js",
    "maintainers": [
        {
            "name": "taijin",
            "email": "taijin@gmail.com"
        }
    ],
    "name": "humanize",
    "optionalDependencies": {},
    "readme": "# humanize #\n\nJavascript data formatter for human readability.\n\nIdea, name, and initial code blatently stolen from [milanvrekic/JS-humanize](http://github.com/milanvrekic/JS-humanize)\n\nCan be loaded via AMD or in node directly.\n\n## Installation ##\n\n    npm install humanize\n\n## Usage: ##\n'''javascript\nvar humanize = require('humanize');\nhumanize.date('Y-m-d'); // 'yyyy-mm-dd'\nhumanize.filesize(1234567890); // '1.15 Gb'\n'''\n\n## Functions available: ##\n\n####humanize.noConflict()####\nGive control of the \"humanize\" variable back to its previous owner. Returns a reference to the humanize object.\n\n####humanize.time()####\nRetrieves the current time in seconds\n\n####humanize.date(format [, timestamp / JS Date Object = new Date()])####\nThis is a port of [php.js date](http://phpjs.org/functions/date:380) and behaves exactly like [PHP's date](http://php.net/manual/en/function.date.php)\n\n####humanize.numberFormat(number [, decimals = 2, decPoint = '.', thousandsSep = ','])####\nFormat a number to have decimal significant decimal places, using decPoint as the decimal separator, and thousandsSep as thousands separater\n\n####humanize.naturalDay(timestamp [, format = 'Y-m-d'])####\nReturns 'today', 'tomorrow' or 'yesterday', as appropriate, otherwise format the date using the passed format with humanize.date()\n\n####humanize.relativeTime(timestamp)####\nReturns a relative time to the current time, seconds as the most granular up to years to the least granular.\n\n####humanize.ordinal(integer)####\nConverts a number into its [ordinal representation](http://en.wikipedia.org/wiki/Ordinal_number_\\(linguistics\\)).\n\n####humanize.filesize(filesize [, kilo = 1024, decimals = 2, decPoint = '.', thousandsSep = ',']) ####\nConverts a byte count to a human readable value using kilo as the basis, and numberFormat formatting\n\n####humanize.linebreaks(string)####\nConverts a string's newlines into properly formatted html ie. one new line -> br, two new lines -> p, entire thing wrapped in p\n\n####humanize.nl2br(string)####\nConverts a string's newlines into br's\n\n####humanize.truncatechars(string, length)####\nTruncates a string to length-1 and appends '…'. If string is shorter than length, then no-op\n\n####humanize.truncatewords(string, numWords)####\nTruncates a string to only include the first numWords words and appends '…'. If string has fewer words than newWords, then no-op\n",
    "readmeFilename": "README.md",
    "repository": {
        "type": "git",
        "url": "git://github.com/taijinlee/humanize.git"
    },
    "scripts": {
        "test": "./node_modules/jshint/bin/hint humanize.js; find specs -type f -a -name *.spec.js -exec ./node_modules/mocha/bin/mocha --globals requirejsVars -R list --require should {} \\;"
    },
    "version": "0.0.9"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module humanize](#apidoc.module.humanize)
1.  [function <span class="apidocSignatureSpan">humanize.</span>date (format, timestamp)](#apidoc.element.humanize.date)
1.  [function <span class="apidocSignatureSpan">humanize.</span>filesize (filesize, kilo, decimals, decPoint, thousandsSep, suffixSep)](#apidoc.element.humanize.filesize)
1.  [function <span class="apidocSignatureSpan">humanize.</span>intword (number, units, kilo, decimals, decPoint, thousandsSep, suffixSep)](#apidoc.element.humanize.intword)
1.  [function <span class="apidocSignatureSpan">humanize.</span>linebreaks (str)](#apidoc.element.humanize.linebreaks)
1.  [function <span class="apidocSignatureSpan">humanize.</span>naturalDay (timestamp, format)](#apidoc.element.humanize.naturalDay)
1.  [function <span class="apidocSignatureSpan">humanize.</span>nl2br (str)](#apidoc.element.humanize.nl2br)
1.  [function <span class="apidocSignatureSpan">humanize.</span>noConflict ()](#apidoc.element.humanize.noConflict)
1.  [function <span class="apidocSignatureSpan">humanize.</span>numberFormat (number, decimals, decPoint, thousandsSep)](#apidoc.element.humanize.numberFormat)
1.  [function <span class="apidocSignatureSpan">humanize.</span>ordinal (number)](#apidoc.element.humanize.ordinal)
1.  [function <span class="apidocSignatureSpan">humanize.</span>pad (str, count, padChar, type)](#apidoc.element.humanize.pad)
1.  [function <span class="apidocSignatureSpan">humanize.</span>relativeTime (timestamp)](#apidoc.element.humanize.relativeTime)
1.  [function <span class="apidocSignatureSpan">humanize.</span>time ()](#apidoc.element.humanize.time)
1.  [function <span class="apidocSignatureSpan">humanize.</span>truncatechars (string, length)](#apidoc.element.humanize.truncatechars)
1.  [function <span class="apidocSignatureSpan">humanize.</span>truncatewords (string, numWords)](#apidoc.element.humanize.truncatewords)
1.  object <span class="apidocSignatureSpan"></span>humanize



# <a name="apidoc.module.humanize"></a>[module humanize](#apidoc.module.humanize)

#### <a name="apidoc.element.humanize.date"></a>[function <span class="apidocSignatureSpan">humanize.</span>date (format, timestamp)](#apidoc.element.humanize.date)
- description and source-code
```javascript
date = function (format, timestamp) {
  var jsdate = ((timestamp === undefined) ? new Date() : // Not provided
                (timestamp instanceof Date) ? new Date(timestamp) : // JS Date()
                new Date(timestamp * 1000) // UNIX timestamp (auto-convert to int)
               );

  var formatChr = /\\?([a-z])/gi;
  var formatChrCb = function (t, s) {
    return f[t] ? f[t]() : s;
  };

  var shortDayTxt = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
  var monthTxt = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', '
December'];

  var f = {
<span class="apidocCodeCommentSpan">    /* Day */
</span>    // Day of month w/leading 0; 01..31
    d: function () { return humanize.pad(f.j(), 2, '0'); },

    // Shorthand day name; Mon..Sun
    D: function () { return f.l().slice(0, 3); },

    // Day of month; 1..31
    j: function () { return jsdate.getDate(); },

    // Full day name; Monday..Sunday
    l: function () { return shortDayTxt[f.w()]; },

    // ISO-8601 day of week; 1[Mon]..7[Sun]
    N: function () { return f.w() || 7; },

    // Ordinal suffix for day of month; st, nd, rd, th
    S: function () {
      var j = f.j();
      return j > 4 && j < 21 ? 'th' : {1: 'st', 2: 'nd', 3: 'rd'}[j % 10] || 'th';
    },

    // Day of week; 0[Sun]..6[Sat]
    w: function () { return jsdate.getDay(); },

    // Day of year; 0..365
    z: function () {
      return (f.L() ? dayTableLeap[f.n()] : dayTableCommon[f.n()]) + f.j() - 1;
    },

    /* Week */
    // ISO-8601 week number
    W: function () {
      // days between midweek of this week and jan 4
      // (f.z() - f.N() + 1 + 3.5) - 3
      var midWeekDaysFromJan4 = f.z() - f.N() + 1.5;
      // 1 + number of weeks + rounded week
      return humanize.pad(1 + Math.floor(Math.abs(midWeekDaysFromJan4) / 7) + (midWeekDaysFromJan4 % 7 > 3.5 ? 1 : 0), 2, '0');
    },

    /* Month */
    // Full month name; January..December
    F: function () { return monthTxt[jsdate.getMonth()]; },

    // Month w/leading 0; 01..12
    m: function () { return humanize.pad(f.n(), 2, '0'); },

    // Shorthand month name; Jan..Dec
    M: function () { return f.F().slice(0, 3); },

    // Month; 1..12
    n: function () { return jsdate.getMonth() + 1; },

    // Days in month; 28..31
    t: function () { return (new Date(f.Y(), f.n(), 0)).getDate(); },

    /* Year */
    // Is leap year?; 0 or 1
    L: function () { return new Date(f.Y(), 1, 29).getMonth() === 1 ? 1 : 0; },

    // ISO-8601 year
    o: function () {
      var n = f.n();
      var W = f.W();
      return f.Y() + (n === 12 && W < 9 ? -1 : n === 1 && W > 9);
    },

    // Full year; e.g. 1980..2010
    Y: function () { return jsdate.getFullYear(); },

    // Last two digits of year; 00..99
    y: function () { return (String(f.Y())).slice(-2); },

    /* Time */
    // am or pm
    a: function () { return jsdate.getHours() > 11 ? 'pm' : 'am'; },

    // AM or PM
    A: function () { return f.a().toUpperCase(); },

    // Swatch Internet time; 000..999
    B: function () {
      var unixTime = jsdate.getTime() / 1000;
      var secondsPassedToday = unixTime % 86400 + 3600; // since it's based off of UTC+1
      if (secondsPassedToday < 0) { secondsPassedToday += 86400; }
      var beats = ((secondsPassedToday) / 86.4) % 1000;
      if (unixTime < 0) {
        return Math.ceil(beats);
      }
      return Math.floor(beats);
    },

    // 12-Hours; 1..12
    g: function () { return f.G() % 12 || 12; },

    // 24-Hours; 0..23
    G: function () { return jsdate.getHours(); },

    // 12-Hours w/leading 0; 01..12
    h: function () { return humanize.pad(f.g(), 2, '0'); },

    // 24-Hours w/leading 0; 00..23
    H: function () { return humanize.pad(f.G(), 2, '0'); },

    // Minutes w/leading 0; 00..59
    i: function () { return humanize.pad(jsdate.getMinutes(), 2, '0'); },

    // Seconds w/leading 0; 00..59
    s: function () { return humanize.pad(jsdate.getSeconds(), 2, '0'); },

    // Microseconds; 000000-999000
    u: function () { return humanize.pad(jsdate.getMillis ...
```
- example usage
```shell
...
## Installation ##

    npm install humanize

## Usage: ##
'''javascript
var humanize = require('humanize');
humanize.date('Y-m-d'); // 'yyyy-mm-dd'
humanize.filesize(1234567890); // '1.15 Gb'
'''

## Functions available: ##

####humanize.noConflict()####
Give control of the "humanize" variable back to its previous owner. Returns a reference to the humanize object.
...
```

#### <a name="apidoc.element.humanize.filesize"></a>[function <span class="apidocSignatureSpan">humanize.</span>filesize (filesize, kilo, decimals, decPoint, thousandsSep, suffixSep)](#apidoc.element.humanize.filesize)
- description and source-code
```javascript
filesize = function (filesize, kilo, decimals, decPoint, thousandsSep, suffixSep) {
  kilo = (kilo === undefined) ? 1024 : kilo;
  if (filesize <= 0) { return '0 bytes'; }
  if (filesize < kilo && decimals === undefined) { decimals = 0; }
  if (suffixSep === undefined) { suffixSep = ' '; }
  return humanize.intword(filesize, ['bytes', 'KB', 'MB', 'GB', 'TB', 'PB'], kilo, decimals, decPoint, thousandsSep, suffixSep);
}
```
- example usage
```shell
...

    npm install humanize

## Usage: ##
'''javascript
var humanize = require('humanize');
humanize.date('Y-m-d'); // 'yyyy-mm-dd'
humanize.filesize(1234567890); // '1.15 Gb'
'''

## Functions available: ##

####humanize.noConflict()####
Give control of the "humanize" variable back to its previous owner. Returns a reference to the humanize object.
...
```

#### <a name="apidoc.element.humanize.intword"></a>[function <span class="apidocSignatureSpan">humanize.</span>intword (number, units, kilo, decimals, decPoint, thousandsSep, suffixSep)](#apidoc.element.humanize.intword)
- description and source-code
```javascript
intword = function (number, units, kilo, decimals, decPoint, thousandsSep, suffixSep) {
  var humanized, unit;

  units = units || ['', 'K', 'M', 'B', 'T'],
  unit = units.length - 1,
  kilo = kilo || 1000,
  decimals = isNaN(decimals) ? 2 : Math.abs(decimals),
  decPoint = decPoint || '.',
  thousandsSep = thousandsSep || ',',
  suffixSep = suffixSep || '';

  for (var i=0; i < units.length; i++) {
    if (number < Math.pow(kilo, i+1)) {
      unit = i;
      break;
    }
  }
  humanized = number / Math.pow(kilo, unit);

  var suffix = units[unit] ? suffixSep + units[unit] : '';
  return humanize.numberFormat(humanized, decimals, decPoint, thousandsSep) + suffix;
}
```
- example usage
```shell
...
 * If value is 123456789, the output would be 117.7 MB.
 */
humanize.filesize = function(filesize, kilo, decimals, decPoint, thousandsSep, suffixSep) {
  kilo = (kilo === undefined) ? 1024 : kilo;
  if (filesize <= 0) { return '0 bytes'; }
  if (filesize < kilo && decimals === undefined) { decimals = 0; }
  if (suffixSep === undefined) { suffixSep = ' '; }
  return humanize.intword(filesize, ['bytes', 'KB', 'MB', 'GB', 'TB', 'PB'], kilo, decimals, decPoint, thousandsSep, suffixSep);
};

/**
 * Formats the value like a 'human-readable' number (i.e. '13 K', '4.1 M', '102', etc).
 *
 * For example:
 * If value is 123456789, the output would be 117.7 M.
...
```

#### <a name="apidoc.element.humanize.linebreaks"></a>[function <span class="apidocSignatureSpan">humanize.</span>linebreaks (str)](#apidoc.element.humanize.linebreaks)
- description and source-code
```javascript
linebreaks = function (str) {
  // remove beginning and ending newlines
  str = str.replace(/^([\n|\r]*)/, '');
  str = str.replace(/([\n|\r]*)$/, '');

  // normalize all to \n
  str = str.replace(/(\r\n|\n|\r)/g, "\n");

  // any consecutive new lines more than 2 gets turned into p tags
  str = str.replace(/(\n{2,})/g, '</p><p>');

  // any that are singletons get turned into br
  str = str.replace(/\n/g, '<br />');
  return '<p>' + str + '</p>';
}
```
- example usage
```shell
...

####humanize.ordinal(integer)####
Converts a number into its [ordinal representation](http://en.wikipedia.org/wiki/Ordinal_number_\(linguistics\)).

####humanize.filesize(filesize [, kilo = 1024, decimals = 2, decPoint = '.', thousandsSep = ',']) ####
Converts a byte count to a human readable value using kilo as the basis, and numberFormat formatting

####humanize.linebreaks(string)####
Converts a string's newlines into properly formatted html ie. one new line -> br, two new lines -> p, entire thing wrapped in p

####humanize.nl2br(string)####
Converts a string's newlines into br's

####humanize.truncatechars(string, length)####
Truncates a string to length-1 and appends '…'. If string is shorter than length, then no-op
...
```

#### <a name="apidoc.element.humanize.naturalDay"></a>[function <span class="apidocSignatureSpan">humanize.</span>naturalDay (timestamp, format)](#apidoc.element.humanize.naturalDay)
- description and source-code
```javascript
naturalDay = function (timestamp, format) {
  timestamp = (timestamp === undefined) ? humanize.time() : timestamp;
  format = (format === undefined) ? 'Y-m-d' : format;

  var oneDay = 86400;
  var d = new Date();
  var today = (new Date(d.getFullYear(), d.getMonth(), d.getDate())).getTime() / 1000;

  if (timestamp < today && timestamp >= today - oneDay) {
    return 'yesterday';
  } else if (timestamp >= today && timestamp < today + oneDay) {
    return 'today';
  } else if (timestamp >= today + oneDay && timestamp < today + 2 * oneDay) {
    return 'tomorrow';
  }

  return humanize.date(format, timestamp);
}
```
- example usage
```shell
...

####humanize.date(format [, timestamp / JS Date Object = new Date()])####
This is a port of [php.js date](http://phpjs.org/functions/date:380) and behaves exactly like [PHP's date](http://php.net/manual
/en/function.date.php)

####humanize.numberFormat(number [, decimals = 2, decPoint = '.', thousandsSep = ','])####
Format a number to have decimal significant decimal places, using decPoint as the decimal separator, and thousandsSep as thousands
 separater

####humanize.naturalDay(timestamp [, format = 'Y-m-d'])####
Returns 'today', 'tomorrow' or 'yesterday', as appropriate, otherwise format the date using the passed format with humanize.date
()

####humanize.relativeTime(timestamp)####
Returns a relative time to the current time, seconds as the most granular up to years to the least granular.

####humanize.ordinal(integer)####
Converts a number into its [ordinal representation](http://en.wikipedia.org/wiki/Ordinal_number_\(linguistics\)).
...
```

#### <a name="apidoc.element.humanize.nl2br"></a>[function <span class="apidocSignatureSpan">humanize.</span>nl2br (str)](#apidoc.element.humanize.nl2br)
- description and source-code
```javascript
nl2br = function (str) {
  return str.replace(/(\r\n|\n|\r)/g, '<br />');
}
```
- example usage
```shell
...

####humanize.filesize(filesize [, kilo = 1024, decimals = 2, decPoint = '.', thousandsSep = ',']) ####
Converts a byte count to a human readable value using kilo as the basis, and numberFormat formatting

####humanize.linebreaks(string)####
Converts a string's newlines into properly formatted html ie. one new line -> br, two new lines -> p, entire thing wrapped in p

####humanize.nl2br(string)####
Converts a string's newlines into br's

####humanize.truncatechars(string, length)####
Truncates a string to length-1 and appends '…'. If string is shorter than length, then no-op

####humanize.truncatewords(string, numWords)####
Truncates a string to only include the first numWords words and appends '…'. If string has fewer words than newWords, then no-op
...
```

#### <a name="apidoc.element.humanize.noConflict"></a>[function <span class="apidocSignatureSpan">humanize.</span>noConflict ()](#apidoc.element.humanize.noConflict)
- description and source-code
```javascript
noConflict = function () {
  root.humanize = previousHumanize;
  return this;
}
```
- example usage
```shell
...
var humanize = require('humanize');
humanize.date('Y-m-d'); // 'yyyy-mm-dd'
humanize.filesize(1234567890); // '1.15 Gb'
'''

## Functions available: ##

####humanize.noConflict()####
Give control of the "humanize" variable back to its previous owner. Returns a reference to the humanize object.

####humanize.time()####
Retrieves the current time in seconds

####humanize.date(format [, timestamp / JS Date Object = new Date()])####
This is a port of [php.js date](http://phpjs.org/functions/date:380) and behaves exactly like [PHP's date](http://php.net/manual
/en/function.date.php)
...
```

#### <a name="apidoc.element.humanize.numberFormat"></a>[function <span class="apidocSignatureSpan">humanize.</span>numberFormat (number, decimals, decPoint, thousandsSep)](#apidoc.element.humanize.numberFormat)
- description and source-code
```javascript
numberFormat = function (number, decimals, decPoint, thousandsSep) {
  decimals = isNaN(decimals) ? 2 : Math.abs(decimals);
  decPoint = (decPoint === undefined) ? '.' : decPoint;
  thousandsSep = (thousandsSep === undefined) ? ',' : thousandsSep;

  var sign = number < 0 ? '-' : '';
  number = Math.abs(+number || 0);

  var intPart = parseInt(number.toFixed(decimals), 10) + '';
  var j = intPart.length > 3 ? intPart.length % 3 : 0;

  return sign + (j ? intPart.substr(0, j) + thousandsSep : '') + intPart.substr(j).replace(/(\d{3})(?=\d)/g, '$1' + thousandsSep
) + (decimals ? decPoint + Math.abs(number - intPart).toFixed(decimals).slice(2) : '');
}
```
- example usage
```shell
...

####humanize.time()####
Retrieves the current time in seconds

####humanize.date(format [, timestamp / JS Date Object = new Date()])####
This is a port of [php.js date](http://phpjs.org/functions/date:380) and behaves exactly like [PHP's date](http://php.net/manual
/en/function.date.php)

####humanize.numberFormat(number [, decimals = 2, decPoint = '.', thousandsSep = ','])####
Format a number to have decimal significant decimal places, using decPoint as the decimal separator, and thousandsSep as thousands
 separater

####humanize.naturalDay(timestamp [, format = 'Y-m-d'])####
Returns 'today', 'tomorrow' or 'yesterday', as appropriate, otherwise format the date using the passed format with humanize.date
()

####humanize.relativeTime(timestamp)####
Returns a relative time to the current time, seconds as the most granular up to years to the least granular.
...
```

#### <a name="apidoc.element.humanize.ordinal"></a>[function <span class="apidocSignatureSpan">humanize.</span>ordinal (number)](#apidoc.element.humanize.ordinal)
- description and source-code
```javascript
ordinal = function (number) {
  number = parseInt(number, 10);
  number = isNaN(number) ? 0 : number;
  var sign = number < 0 ? '-' : '';
  number = Math.abs(number);
  var tens = number % 100;

  return sign + number + (tens > 4 && tens < 21 ? 'th' : {1: 'st', 2: 'nd', 3: 'rd'}[number % 10] || 'th');
}
```
- example usage
```shell
...

####humanize.naturalDay(timestamp [, format = 'Y-m-d'])####
Returns 'today', 'tomorrow' or 'yesterday', as appropriate, otherwise format the date using the passed format with humanize.date
()

####humanize.relativeTime(timestamp)####
Returns a relative time to the current time, seconds as the most granular up to years to the least granular.

####humanize.ordinal(integer)####
Converts a number into its [ordinal representation](http://en.wikipedia.org/wiki/Ordinal_number_\(linguistics\)).

####humanize.filesize(filesize [, kilo = 1024, decimals = 2, decPoint = '.', thousandsSep = ',']) ####
Converts a byte count to a human readable value using kilo as the basis, and numberFormat formatting

####humanize.linebreaks(string)####
Converts a string's newlines into properly formatted html ie. one new line -> br, two new lines -> p, entire thing wrapped in p
...
```

#### <a name="apidoc.element.humanize.pad"></a>[function <span class="apidocSignatureSpan">humanize.</span>pad (str, count, padChar, type)](#apidoc.element.humanize.pad)
- description and source-code
```javascript
pad = function (str, count, padChar, type) {
  str += '';
  if (!padChar) {
    padChar = ' ';
  } else if (padChar.length > 1) {
    padChar = padChar.charAt(0);
  }
  type = (type === undefined) ? 'left' : 'right';

  if (type === 'right') {
    while (str.length < count) {
      str = str + padChar;
    }
  } else {
    // default to left
    while (str.length < count) {
      str = padChar + str;
    }
  }

  return str;
}
```
- example usage
```shell
...

    var shortDayTxt = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
    var monthTxt = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', '
December'];

    var f = {
/* Day */
// Day of month w/leading 0; 01..31
d: function () { return humanize.pad(f.j(), 2, '0'); },

// Shorthand day name; Mon..Sun
D: function () { return f.l().slice(0, 3); },

// Day of month; 1..31
j: function () { return jsdate.getDate(); },
...
```

#### <a name="apidoc.element.humanize.relativeTime"></a>[function <span class="apidocSignatureSpan">humanize.</span>relativeTime (timestamp)](#apidoc.element.humanize.relativeTime)
- description and source-code
```javascript
relativeTime = function (timestamp) {
  timestamp = (timestamp === undefined) ? humanize.time() : timestamp;

  var currTime = humanize.time();
  var timeDiff = currTime - timestamp;

  // within 2 seconds
  if (timeDiff < 2 && timeDiff > -2) {
    return (timeDiff >= 0 ? 'just ' : '') + 'now';
  }

  // within a minute
  if (timeDiff < 60 && timeDiff > -60) {
    return (timeDiff >= 0 ? Math.floor(timeDiff) + ' seconds ago' : 'in ' + Math.floor(-timeDiff) + ' seconds');
  }

  // within 2 minutes
  if (timeDiff < 120 && timeDiff > -120) {
    return (timeDiff >= 0 ? 'about a minute ago' : 'in about a minute');
  }

  // within an hour
  if (timeDiff < 3600 && timeDiff > -3600) {
    return (timeDiff >= 0 ? Math.floor(timeDiff / 60) + ' minutes ago' : 'in ' + Math.floor(-timeDiff / 60) + ' minutes');
  }

  // within 2 hours
  if (timeDiff < 7200 && timeDiff > -7200) {
    return (timeDiff >= 0 ? 'about an hour ago' : 'in about an hour');
  }

  // within 24 hours
  if (timeDiff < 86400 && timeDiff > -86400) {
    return (timeDiff >= 0 ? Math.floor(timeDiff / 3600) + ' hours ago' : 'in ' + Math.floor(-timeDiff / 3600) + ' hours');
  }

  // within 2 days
  var days2 = 2 * 86400;
  if (timeDiff < days2 && timeDiff > -days2) {
    return (timeDiff >= 0 ? '1 day ago' : 'in 1 day');
  }

  // within 29 days
  var days29 = 29 * 86400;
  if (timeDiff < days29 && timeDiff > -days29) {
    return (timeDiff >= 0 ? Math.floor(timeDiff / 86400) + ' days ago' : 'in ' + Math.floor(-timeDiff / 86400) + ' days');
  }

  // within 60 days
  var days60 = 60 * 86400;
  if (timeDiff < days60 && timeDiff > -days60) {
    return (timeDiff >= 0 ? 'about a month ago' : 'in about a month');
  }

  var currTimeYears = parseInt(humanize.date('Y', currTime), 10);
  var timestampYears = parseInt(humanize.date('Y', timestamp), 10);
  var currTimeMonths = currTimeYears * 12 + parseInt(humanize.date('n', currTime), 10);
  var timestampMonths = timestampYears * 12 + parseInt(humanize.date('n', timestamp), 10);

  // within a year
  var monthDiff = currTimeMonths - timestampMonths;
  if (monthDiff < 12 && monthDiff > -12) {
    return (monthDiff >= 0 ? monthDiff + ' months ago' : 'in ' + (-monthDiff) + ' months');
  }

  var yearDiff = currTimeYears - timestampYears;
  if (yearDiff < 2 && yearDiff > -2) {
    return (yearDiff >= 0 ? 'a year ago' : 'in a year');
  }

  return (yearDiff >= 0 ? yearDiff + ' years ago' : 'in ' + (-yearDiff) + ' years');
}
```
- example usage
```shell
...

####humanize.numberFormat(number [, decimals = 2, decPoint = '.', thousandsSep = ','])####
Format a number to have decimal significant decimal places, using decPoint as the decimal separator, and thousandsSep as thousands
 separater

####humanize.naturalDay(timestamp [, format = 'Y-m-d'])####
Returns 'today', 'tomorrow' or 'yesterday', as appropriate, otherwise format the date using the passed format with humanize.date
()

####humanize.relativeTime(timestamp)####
Returns a relative time to the current time, seconds as the most granular up to years to the least granular.

####humanize.ordinal(integer)####
Converts a number into its [ordinal representation](http://en.wikipedia.org/wiki/Ordinal_number_\(linguistics\)).

####humanize.filesize(filesize [, kilo = 1024, decimals = 2, decPoint = '.', thousandsSep = ',']) ####
Converts a byte count to a human readable value using kilo as the basis, and numberFormat formatting
...
```

#### <a name="apidoc.element.humanize.time"></a>[function <span class="apidocSignatureSpan">humanize.</span>time ()](#apidoc.element.humanize.time)
- description and source-code
```javascript
time = function () {
  return new Date().getTime() / 1000;
}
```
- example usage
```shell
...
'''

## Functions available: ##

####humanize.noConflict()####
Give control of the "humanize" variable back to its previous owner. Returns a reference to the humanize object.

####humanize.time()####
Retrieves the current time in seconds

####humanize.date(format [, timestamp / JS Date Object = new Date()])####
This is a port of [php.js date](http://phpjs.org/functions/date:380) and behaves exactly like [PHP's date](http://php.net/manual
/en/function.date.php)

####humanize.numberFormat(number [, decimals = 2, decPoint = '.', thousandsSep = ','])####
Format a number to have decimal significant decimal places, using decPoint as the decimal separator, and thousandsSep as thousands
 separater
...
```

#### <a name="apidoc.element.humanize.truncatechars"></a>[function <span class="apidocSignatureSpan">humanize.</span>truncatechars (string, length)](#apidoc.element.humanize.truncatechars)
- description and source-code
```javascript
truncatechars = function (string, length) {
  if (string.length <= length) { return string; }
  return string.substr(0, length) + '…';
}
```
- example usage
```shell
...

####humanize.linebreaks(string)####
Converts a string's newlines into properly formatted html ie. one new line -> br, two new lines -> p, entire thing wrapped in p

####humanize.nl2br(string)####
Converts a string's newlines into br's

####humanize.truncatechars(string, length)####
Truncates a string to length-1 and appends '…'. If string is shorter than length, then no-op

####humanize.truncatewords(string, numWords)####
Truncates a string to only include the first numWords words and appends '…'. If string has fewer words than newWords, then no-op
...
```

#### <a name="apidoc.element.humanize.truncatewords"></a>[function <span class="apidocSignatureSpan">humanize.</span>truncatewords (string, numWords)](#apidoc.element.humanize.truncatewords)
- description and source-code
```javascript
truncatewords = function (string, numWords) {
  var words = string.split(' ');
  if (words.length < numWords) { return string; }
  return words.slice(0, numWords).join(' ') + '…';
}
```
- example usage
```shell
...

####humanize.nl2br(string)####
Converts a string's newlines into br's

####humanize.truncatechars(string, length)####
Truncates a string to length-1 and appends '…'. If string is shorter than length, then no-op

####humanize.truncatewords(string, numWords)####
Truncates a string to only include the first numWords words and appends '…'. If string has fewer words than newWords, then no-op
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
