# xdncov
西电晨午晚检自动填报小脚本 little shell

```
curl -k https://xxcapp.xidian.edu.cn/uc/wap/login/check -d "username=*Your 学号*&password=*Your Password*"
curl -k https://xxcapp.xidian.edu.cn/xisuncov/wap/open-report/save -d "sfzx=1&tw=1&area=%E9%99%95%E8%A5%BF%E7%9C%81%20%E8%A5%BF%E5%AE%89%E5%B8%82%20%E9%9B%81%E5%A1%94%E5%8C%BA&city=%E8%A5%BF%E5%AE%89%E5%B8%82&province=%E9%99%95%E8%A5%BF%E7%9C%81&address=%E9%99%95%E8%A5%BF%E7%9C%81%E8%A5%BF%E5%AE%89%E5%B8%82%E9%9B%81%E5%A1%94%E5%8C%BA%E7%94%B5%E5%AD%90%E5%9F%8E%E8%A1%97%E9%81%93%E7%A0%94%E7%A9%B6%E7%94%9F96%E5%8F%B7%E5%AE%BF%E8%88%8D%E6%A5%BC%E8%A5%BF%E5%AE%89%E7%94%B5%E5%AD%90%E7%A7%91%E6%8A%80%E5%A4%A7%E5%AD%A6%E5%8C%97%E6%A0%A1%E5%8C%BA&geo_api_info=%7B%22type%22%3A%22complete%22%2C%22info%22%3A%22SUCCESS%22%2C%22status%22%3A1%2C%22%24Da%22%3A%22jsonp_240868_%22%2C%22position%22%3A%7B%22Q%22%3A34.23255%2C%22R%22%3A108.91512999999998%2C%22lng%22%3A108.91513%2C%22lat%22%3A34.23255%7D%2C%22message%22%3A%22Get%20ipLocation%20success.Get%20address%20success.%22%2C%22location_type%22%3A%22ip%22%2C%22accuracy%22%3Anull%2C%22isConverted%22%3Atrue%2C%22addressComponent%22%3A%7B%22citycode%22%3A%22029%22%2C%22adcode%22%3A%22610113%22%2C%22businessAreas%22%3A%5B%5D%2C%22neighborhoodType%22%3A%22%22%2C%22neighborhood%22%3A%22%22%2C%22building%22%3A%22%22%2C%22buildingType%22%3A%22%22%2C%22street%22%3A%22%E7%99%BD%E6%B2%99%E8%B7%AF%22%2C%22streetNumber%22%3A%228%E5%8F%B7%22%2C%22country%22%3A%22%E4%B8%AD%E5%9B%BD%22%2C%22province%22%3A%22%E9%99%95%E8%A5%BF%E7%9C%81%22%2C%22city%22%3A%22%E8%A5%BF%E5%AE%89%E5%B8%82%22%2C%22district%22%3A%22%E9%9B%81%E5%A1%94%E5%8C%BA%22%2C%22township%22%3A%22%E7%94%B5%E5%AD%90%E5%9F%8E%E8%A1%97%E9%81%93%22%7D%2C%22formattedAddress%22%3A%22%E9%99%95%E8%A5%BF%E7%9C%81%E8%A5%BF%E5%AE%89%E5%B8%82%E9%9B%81%E5%A1%94%E5%8C%BA%E7%94%B5%E5%AD%90%E5%9F%8E%E8%A1%97%E9%81%93%E7%A0%94%E7%A9%B6%E7%94%9F96%E5%8F%B7%E5%AE%BF%E8%88%8D%E6%A5%BC%E8%A5%BF%E5%AE%89%E7%94%B5%E5%AD%90%E7%A7%91%E6%8A%80%E5%A4%A7%E5%AD%A6%E5%8C%97%E6%A0%A1%E5%8C%BA%22%2C%22roads%22%3A%5B%5D%2C%22crosses%22%3A%5B%5D%2C%22pois%22%3A%5B%5D%7D&sfcyglq=0&sfyzz=0&qtqk=&ymtys=0"
```
填这个就肯定没错，电脑浏览器默认的就这个，有兴趣的可以自己decode然后改参数

脚本使用方法：下载脚本，修改你的学号和密码保存，放到一个24小时不关机还能联网的机子上，可以是路由器，可以是服务器，甚至是手机（后台杀死警告）。
```
nohup sh ./ncov.sh &
```
完事
