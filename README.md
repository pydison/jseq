# jseq
序列解析系统

示例接口

http://t.weather.sojson.com/api/weather/city/101050607

```
  from yulonglib.jseq import Jseq
  J=Jseq("http://t.weather.sojson.com/api/weather/city/{}")
  result=J.j_ld(("101050701","101050607"),("data","forecast"),"date","week")
```
