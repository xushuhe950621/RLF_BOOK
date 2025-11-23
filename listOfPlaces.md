# 兴趣点（Places）配置

## 概述

此配置定义了游戏中的地点列表，包括其属性、图片和访问条件。  
每个地点都包含名称、描述、搜索半径以及相关图片信息。

## 配置结构

### 地点对象的属性

在 `listOfPlaces` 数组中的每个地点包含以下属性：

| 属性 | 类型 | 描述 |
|----------|-----|----------|
| `idPagePlace` | Number | 地点页面的唯一标识符 |
| `needPaperToShow` | Number | 查看该地点所需的纸张数量（0 = 默认可见） |
| `placeTitle` | String | 地点名称 |
| `placeDesc` | String | 地点描述 |
| `radiusSearch` | Number | 该地点的搜索半径（单位：米） |
| `mapImg` | String | 地点地图图片路径 |
| `placeImg` | Array | 地点图片路径数组 |

## 配置示例

```json
 [
    {
      "idPagePlace": 0,
      "needPaperToShow": 0,
      "placeTitle": "废弃医院",
      "placeDesc": "灾难后被遗弃的旧医院。这里可能找到医疗用品和医疗设备。",
      "radiusSearch": 100,
      "mapImg": "relife_BookSystem/images/map.edds",
      "placeImg": [
        "relife_BookSystem/images/hospital_exterior.edds",
        "relife_BookSystem/images/hospital_lobby.edds",
        "relife_BookSystem/images/hospital_ward.edds",
        "relife_BookSystem/images/hospital_basement.edds"
      ]
    },
    {
      "idPagePlace": 1,
      "needPaperToShow": 1,
      "placeTitle": "军事基地",
      "placeDesc": "被遗弃的军事基地，遗留有部分装备和物资。",
      "radiusSearch": 150,
      "mapImg": "relife_BookSystem/images/base_map.edds",
      "placeImg": [
        "relife_BookSystem/images/base_gate.edds",
        "relife_BookSystem/images/base_barracks.edds",
        "relife_BookSystem/images/base_armory.edds"
      ]
    }
  ]
使用说明
idPagePlace：必须为每个地点唯一，避免冲突

needPaperToShow：用于控制地点解锁进度；若启用，需要找到对应地点的纸张才能查看

placeTitle：用于界面的清晰简短地点名称

placeDesc：提供地点背景、用途与细节描述

radiusSearch：影响搜索物品或交互触发的区域范围

mapImg：地点地图的图片路径

placeImg：地点的图片数组，可包含多张图片

文件格式
格式：使用 .edds 格式以兼容游戏引擎

图片数量：placeImg 可包含任意数量的图片

推荐分辨率：

地图：512×512 像素

地点图：1024×1024 像素

添加新地点
若要添加新地点：

在 listOfPlaces 中加入新的对象

设置唯一的 idPagePlace（递增或任意唯一值）

设置 needPaperToShow 以控制解锁方式

在 placeTitle 中填写地点名称

在 placeDesc 中撰写地点的详细说明

设置合适的搜索半径 radiusSearch

在 mapImg 填写地图图片路径

在 placeImg 中添加地点图片路径数组

地点系统特点
进度系统
needPaperToShow: 0 → 默认直接可访问

needPaperToShow: 1 → 需找到该地点的纸张并加入书中后才能访问

图片管理
placeImg 中第一张图片通常作为默认主图

其余图片用于展示更多细节或角度

地图图片（mapImg）独立显示，与地点图分开
