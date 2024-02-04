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
  "author": "FooBar",
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
|names|字型的次要名稱， Schema 請參考 [Names](#names)|
|author|字型作者|
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

## 如何貢獻

### 增加字型

請根據 schema 修改 `FreeFontList.json` 檔案後，再發個 pull request 給我。

### 回報問題與改善建議

發個 issue 說明你遇到的問題或是改善的建議。 

## 以下專案使用到本專案的字型列表

如果你的專案有使用到這個列表，也可以在下面的專案列表增加上去，然後發個 `README.md` 的 pull request 給我。

### 專案列表