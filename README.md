# starcitizen-data
# 星际公民商品数据库
## 使用方式
1. 通过cdn获取本库的索引及内容文件 前缀:https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/
  例: https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/index.json
2. 自己实现任何方式搜索index.json(必须)以及ext_index.json(可选)中的索引,根据得到的相对路径后,拼上前缀得到商品的信息
  例: 
  ```
   //搜索得到下面的索引
    {"id":"082c2ffb-1c54-45e5-90bf-f411d9a06425","name":"'Arrow' I","name_cn":"箭头 I","path":"Data/Libs/Foundry/Records/Entities/SCItem/Ships/Weapons/Missiles/MISL_S01_IR_VNCL_Arrow.json","show_type_key":"Missile","size":1,"grade":1},{"id":"1754a3d4-4aa9-469d-8fb7-d8611bd3e9a1","name":"'Bullet' II","name_cn":"子弹 II","path":"Data/Libs/Foundry/Records/Entities/SCItem/Ships/Weapons/Missiles/MISL_S02_IR_VNCL_Bullet.json","show_type_key":"Missile","size":2,"grade":1}
    //根据path拿到信息
    https://cdn.jsdelivr.net/gh/herokillerJ/starcitizen-data@latest/Data/Libs/Foundry/Records/Entities/SCItem/Ships/Weapons/Missiles/MISL_S02_IR_VNCL_Bullet.json
    //解析内容
  ```
