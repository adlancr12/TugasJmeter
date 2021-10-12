# Tugas Meet 9th JMeter

Adlan Chosyiyar Rochman



## Ditambah baris ke 2 dan 3

```python
import groovy.json.JsonSlurper
log.error(prev.getResponseCode().toString())
log.error(prev.getResponseDataAsString())
def jsonData = new JsonSlurper().parseText(prev.getResponseDataAsString())
log.error(jsonData.user.authtoken)
def authToken = jsonData.user.authtoken
vars.put('token',authToken)
```
