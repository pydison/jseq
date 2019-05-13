# jseq
序列解析系统

示例接口

http://t.weather.sojson.com/api/weather/city/101050607

```
  from yulonglib.jseq import Jseq
  J=Jseq("http://t.weather.sojson.com/api/weather/city/{}")
  result=J.j_ld(("101050701","101050607"),("data","forecast"),"date","week")
```


即可得到

```
[
{'date': u'24', 'week': u'\u661f\u671f\u4e94'}
{'date': u'25', 'week': u'\u661f\u671f\u516d'}
{'date': u'26', 'week': u'\u661f\u671f\u65e5'}
{'date': u'27', 'week': u'\u661f\u671f\u4e00'}
{'date': u'13', 'week': u'\u661f\u671f\u4e00'}
{'date': u'14', 'week': u'\u661f\u671f\u4e8c'}
{'date': u'15', 'week': u'\u661f\u671f\u4e09'}
{'date': u'16', 'week': u'\u661f\u671f\u56db'}
{'date': u'17', 'week': u'\u661f\u671f\u4e94'}
{'date': u'18', 'week': u'\u661f\u671f\u516d'}
{'date': u'19', 'week': u'\u661f\u671f\u65e5'}
{'date': u'20', 'week': u'\u661f\u671f\u4e00'}
{'date': u'21', 'week': u'\u661f\u671f\u4e8c'}
{'date': u'22', 'week': u'\u661f\u671f\u4e09'}
{'date': u'23', 'week': u'\u661f\u671f\u56db'}
{'date': u'24', 'week': u'\u661f\u671f\u4e94'}
{'date': u'25', 'week': u'\u661f\u671f\u516d'}
{'date': u'26', 'week': u'\u661f\u671f\u65e5'}
{'date': u'27', 'week': u'\u661f\u671f\u4e00'}
]

```
