# 物品描述配置 (Items)

## 概述

此配置定义了游戏中的物品列表，包括它们的描述和可发现位置。  
每个物品包含技术类名、显示名称、详细说明以及可找到的位置。

## 配置结构

### 物品对象的属性

在 `listOfItemInfo` 数组中的每个物品包含以下属性：

| 属性 | 类型 | 描述 |
|----------|-----|----------|
| `itemClassname` | String | 游戏中物品类的技术名称 |
| `itemTitle` | String | 物品的显示名称 |
| `itemInfo` | String | 物品的详细描述、属性与用途 |
| `itemInfoLocation` | String | 玩家可找到该物品的位置说明 |

## 配置示例

```json
[
    {
      "itemClassname": "Apple",
      "itemTitle": "苹果",
      "itemInfo": "新鲜水果，富含维生素。可恢复少量健康值并减轻饥饿。放置数天后会腐坏。",
      "itemInfoLocation": "苹果园、废弃农场、森林中的野生苹果树"
    },
    {
      "itemClassname": "Morphine",
      "itemTitle": "吗啡",
      "itemInfo": "强效止痛剂。可立即恢复健康，但会导致短暂的视线模糊。频繁使用可能导致成瘾。",
      "itemInfoLocation": "医院、医务室、救护车、急救包"
    },
    {
      "itemClassname": "AK74",
      "itemTitle": "AK-74",
      "itemInfo": "5.45mm口径的自动步枪。在中距离具有良好精度和可靠性。需要定期清洁以保持性能。",
      "itemInfoLocation": "军事基地、检查站、士兵尸体、武器仓库"
    },
    {
      "itemClassname": "Bandage",
      "itemTitle": "绷带",
      "itemInfo": "用于包扎的医疗绷带。可止血并缓慢恢复健康。一次性物品。",
      "itemInfoLocation": "医疗机构、家庭急救箱、救护车、居民房屋"
    },
    {
      "itemClassname": "Gasoline",
      "itemTitle": "汽油",
      "itemInfo": "用于车辆与发电机的燃料。极易燃，应小心存放与使用。",
      "itemInfoLocation": "加油站、车库、车辆中的油桶、燃料储备仓库"
    },
    {
      "itemClassname": "WoodenPlank",
      "itemTitle": "木板",
      "itemInfo": "由处理过的木材制成的建材。用于修复掩体、制作路障以及制造简单工具。",
      "itemInfoLocation": "建筑仓库、木材厂、破损建筑、棚屋和车库"
    }
  ]
