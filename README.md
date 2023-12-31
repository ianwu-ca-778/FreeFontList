# FreeFontList
The list of free fonts collected online.

## Schema

```json
{
  "version": "1.0.0",
  "fonts": [{
    ...
  }]
}
```

|屬性|說明|
|--|--|
|version|Schema 的版本|
|fonts|Font 列表|

### Font

```json
{
  "name": "FooBarFont",
  "names": {
    ...
  },
  "version": "1.0.0",
  "url": "https://www.foo.bar",
  "downloadUrl": "https://www.foo.bar/fooFont.zip",
  "donateUrl": "https://www.foo.bar/donate",
  "license": {
    ...
  }
}
```

|屬性|說明|
|--|--|
|name|字型的主要名稱|
|version|字型的版本|
|url|字型的網站|
|downloadUrl|字型的下載網址|
|donateUrl|字型贊助的網址|
|license|字型的授權|

#### Names

```json
{
  "en-US": "FooBarFont",
  "zh-TW": "福爸體",
  ...
}
```

字型的其他名稱，屬性請參考 [ISO Language Code](http://www.lingoes.net/en/translator/langcode.htm)

#### License

```json
{
  "type": "MIT",
  "url": "https://www.foo.bar/license"
}

```

|屬性|說明|
|--|--|
|type|授權類型|
|url|授權說明網址|

## Example

```json
{
  "version": "1.0.0",
  "fonts": [{
    "name": "FooFont",
    "names": {
      "zh-TW": "福爸體"
    },
    "version": "1.0.0",
    "url": "https://www.foo.bar",
    "downloadUrl": "https://www.foo.bar/fooFont.zip",
    "donateUrl": "https://www.foo.bar/donate",
    "license": {
      "type": "MIT",
      "url": "https://www.foo.bar/license"
    }
  }]
}
```