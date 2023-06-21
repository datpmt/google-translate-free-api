# Google Translate Free API
Although not the most complete API product, it is free and has all the necessary APIs to be able to create translation extensions for your application.\
Let read the [document](https://api.datpmt.com) and use it.\
Warning!!!\
This is a free application and must not be used for commercial purposes. DATPMT disclaims all litigation related to unauthorized use.
## * Translate string
Method: `GET`, URL: `api/v1/dictionary/translate`\
Params: `[string, from_lang, to_lang]`
```
string # <= 5000 characters

from_lang # default en

to_lang # default vi
```
<p align="center"><img src="https://api.datpmt.com/assets/t-b0f5d50f3387eaabbae57e3273aaa1df8cb2b19bb135807f319fb45806f915e6.png"></p>

Example: GET `https://api.datpmt.com/api/v1/dictionary/translate?string=summer`
```
=> "mùa hè"
```
## * Alternate translations
Method: `GET`, URL: `api/v1/dictionary/alternate_translations`\
Params: `[keyword, from_lang, to_lang]`
```
keyword # string

from_lang # default en

to_lang # default vi
```
<p align="center"><img src="https://api.datpmt.com/assets/at-3f96c877a177eb42ac490b5e20e5a57c986f84052eed469e7c645e9308f3f2d4.png"></p>

Example: GET `https://api.datpmt.com/api/v1/dictionary/alternate_translations?keyword=summer`
```
=> "mùa hè, mùa hạ, hè"
```

## * Examples
Method: `GET`, URL: `api/v1/dictionary/examples`\
Params: `[keyword, from_lang]`
```
keyword # string

from_lang # default en
```
<p align="center"><img src="https://api.datpmt.com/assets/ex-b6240bf93527a779f96b4f01d8c7a960907eed52f0ef30b1bac26c02fb644865.png"></p>

Example: GET `https://api.datpmt.com/api/v1/dictionary/examples?keyword=summer`
```json
[
  "summer vacation.",
  "The plant flowers in late summer.",
  "The golden summer of her life.",
  "A long hot summer."
]
```

## * Definitions
Method: `GET`, URL: `api/v1/dictionary/definitions`\
Params: `[keyword, from_lang]`\
Response: # `[ preposition: [desc example sysnonyms] ]`
```
keyword # string

from_lang # default en
```
<p align="center"><img src="https://api.datpmt.com/assets/md-4a68a6ce65cbe586e24e54c457c8c420aeffd94e82007835d17fa20bdf78d5e2.png"></p>

Example: `GET` `https://api.datpmt.com/api/v1/dictionary/definitions?keyword=summer`
```json
[
  {
    "noun": [
      [
        "The warmest season of the year, in the northern hemisphere from june to august and in the southern hemisphere from december to february.",
        "summer vacation.",
        null
      ],
      [
        "A horizontal bearing beam, especially one supporting joists or rafters.",
        null,
        null
      ]
    ]
  },
  {
    "verb": [
      [
        "Spend the summer in a particular place.",
        null,
        null
      ]
    ]
  }
]
```

## * Transliteration
Method: `GET`, URL: `api/v1/dictionary/transliteration`\
Params: `[keyword, from_lang]`
```
keyword # string

from_lang # default en
```
<p align="center"><img src="https://api.datpmt.com/assets/t-b0f5d50f3387eaabbae57e3273aaa1df8cb2b19bb135807f319fb45806f915e6.png"></p>

Example: `GET` `https://api.datpmt.com/api/v1/dictionary/transliteration?keyword=summer`
```
=> "ˈsəmər"
```

## * See more
Method: `GET`, URL: `api/v1/dictionary/see_more`\
Params: `[keyword, from_lang]`\
Response: # `[kids -> kid, tables -> table]`
```
keyword # string

from_lang # default en
```
<p align="center"><img src="https://api.datpmt.com/assets/rw-a604055ff84edfecf2d6f31006f8ddebd3fb05e85a73730d6385614b2b44191d.png"></p>

Example: `GET` `https://api.datpmt.com/api/v1/dictionary/see_more?keyword=kids`
```
=> "kid"
```