# catj
Displays XML files in a flat format. Doesn't do namespaces or attributes.

Input:

```
<items>
	<item id="0001" type="donut">
		<name>Cake</name>
		<ppu>0.55</ppu>
		<batters>
			<batter id="1001">Regular</batter>
			<batter id="1002">Chocolate</batter>
			<batter id="1003">Blueberry</batter>
		</batters>
		<topping id="5001">None</topping>
		<topping id="5002">Glazed</topping>
		<topping id="5005">Sugar</topping>
		<topping id="5006">Sprinkles</topping>
		<topping id="5003">Chocolate</topping>
		<topping id="5004">Maple</topping>
	</item>
</items>
```

Output:

```
/items/item/name = "Cake"
/items/item/ppu = 0.55
/items/item/batters/batter[0] = "Regular"
/items/item/batters/batter[1] = "Chocolate"
/items/item/batters/batter[2] = "Blueberry"
/items/item/topping[0] = "None"
/items/item/topping[1] = "Glazed"
/items/item/topping[2] = "Sugar"
/items/item/topping[3] = "Sprinkles"
/items/item/topping[4] = "Chocolate"
/items/item/topping[5] = "Maple"
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
