# catj
Displays XML files in a flat format. Doesn't do namespaces or attributes.

Input:

```
<note>
  <to>Tove</to>
  <from>Jani</from>
  <heading>Reminder</heading>
  <body>Don't forget me this weekend!</body>
</note>
```

Output:

```
/note/to = Tove
/note/from = Jani
/note/heading = Reminder
/note/body = Don't forget me this weekend!
```

## Why?

- It makes it easier to understand the structure of XML files.
- The output is valid absolute xpath which can be used directly in code.

## Install

```
npm install -g catx
```

## Usage

```
catx [file]
```

If no file is specified, catx reads from the standard input.

## Version History
+ **1.0**
	+ Initial release.
  + Inspired by Soheil Rashidi's catj: http://soheilrashidi.com
  + Also @dynamicwebpaige's tweet: https://twitter.com/DynamicWebPaige/status/1142220407719616513 

## Author
**Sam Moorhouse**

+ http://globalcode.org.uk/

## Copyright and License
Copyright 2019 Sam Moorhouse

Licensed under the The MIT License (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

http://www.opensource.org/licenses/mit-license.php

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
