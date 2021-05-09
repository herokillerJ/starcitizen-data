# starcitizen-data
# <方舟知识协会>星际公民商品数据库
## 使用方式
1. 通过github原地址或cdn获取本库的索引及内容文件 cdn前缀:https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/
  例: https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/index.json
2. 自己实现任何方式搜索index.json(必须)以及ext_index.json(可选)中的索引,根据得到的相对路径后,拼上前缀得到商品的信息
  例: 
  ```
   //搜索得到下面的索引
    {"id":"082c2ffb-1c54-45e5-90bf-f411d9a06425","name":"'Arrow' I","name_cn":"箭头 I","path":"Data/Libs/Foundry/Records/Entities/SCItem/Ships/Weapons/Missiles/MISL_S01_IR_VNCL_Arrow.json","show_type_key":"Missile","size":1,"grade":1}
    //根据path拿到信息
    https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/Data/Libs/Foundry/Records/Entities/SCItem/Ships/Weapons/Missiles/MISL_S01_IR_VNCL_Arrow.json
    //解析内容
  ```
## 注意事项
1. cdn的刷新时间请参考jsdelivr官方文档，当推送新release后应该是一天时间，用@latest应该足够满足绝大部分场景
2. index.json中包含游戏版本号，通过json内的version字段判断是否应该更新你的本地缓存索引，当然也可以选择每隔一段时间就重建索引，毕竟一共也就几千条数据
