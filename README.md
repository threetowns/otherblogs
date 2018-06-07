# NPGIS

* `mapConfig.json`

  ```json
  {
      "mapOpts":
      {
          "minZoom": 10,   // 最小级别，根据实际切片的级数来确定
          "maxZoom": 18,   // 最大级别，根据实际切片的级数来确定
          "defaultZoom":18,
          "centerPoint": [121.46954675546338,30.919911396365844],  //中心点坐标
          "restrictedExtent": [   // 抓图工具设置的抓图范围
              13478926.539104,3595651.244330,
              13576307.31314,3669642.2877104
          ],
          "projection": "EPSG:900913"   //投影方式：900913
      },
      "vectorLayer": [
          {
              "layerName": "shanghaiBaseMap1",
              "layerType": "NPMapLib.Layers.GaoDeLayer",
              "layerOpt":
              {
                  "url": ["http://172.19.59.8:25003/v3/tile?x=${x}&y=${y}&z=${z}"],
                  "centerPoint": [121.46954675546338,30.919911396365844],
                  "isBaseLayer": true                
              }
          },
          {
              "layerName": "shanghaiBaseMap2",
              "layerType": "NPMapLib.Layers.GaoDeLayer",
              "layerOpt":
              {
                  "url": ["http://172.19.59.8:25033/v3/tile?x=${x}&y=${y}&z=${z}"],
                  "isBaseLayer": false,
                  "centerPoint": [121.46954675546338,30.919911396365844]
              }
          }
      ],
      "sattilateLayer": []
  }
  ```

  



***



## 联系方式

* email：`threetowns@163.com`
* qq: `1223930438`
