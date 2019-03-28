# sources
Json 格式化

```kotlin
 fun prettify(json_text: String): String {
        val parser = JsonParser()
        val json = parser.parse(json_text)
        val gson = GsonBuilder().setPrettyPrinting().create()
        return gson.toJson(json)
    }
```
Json 模板
```json
[
  [
    [
      "Hello there",
      "你好",
      null,
      null,
      1
    ]
  ],
  null,
  "zh-CN"
]
```
