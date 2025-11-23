# “医疗”部分配置 listOfDrugs

## 概述

此配置定义了可消耗物品（药物）的列表及其效果与属性。  
每个药物包含作用持续时间以及对玩家产生的各种效果。

## 配置结构

### 药物对象的属性

在 `listOfDrugs` 数组中的每个药物都包含以下属性：

| 属性 | 类型 | 描述 |
|----------|-----|----------|
| `className` | String | 药物的唯一标识符 / 名称 |
| `timeEffect` | Number | 药物效果持续时间（秒，可为小数） |
| `listOfPlusEffect` | Array | 药物带来的正面效果列表 |
| `listOfMinusEffect` | Array | 药物带来的负面效果 / 副作用列表 |
| `listOfMoreInfo` | Array | 关于药物的其他附加信息 |

### 效果对象结构

在效果数组（`listOfPlusEffect`、`listOfMinusEffect`、`listOfMoreInfo`）中的每个对象包含：

| 属性 | 类型 | 描述 |
|----------|-----|----------|
| `textList` | String | 效果或附加信息的文本描述 |

## 配置示例

```json
[
    {
      "className": "Adrenaline",
      "timeEffect": 100.0,
      "listOfPlusEffect": [
        {
          "textList": "移动速度提升 50%"
        },
        {
          "textList": "射击精度提高 25%"
        }
      ],
      "listOfMinusEffect": [
        {
          "textList": "生命值降低 10 点"
        },
        {
          "textList": "效果结束后会出现手部颤抖"
        }
      ],
      "listOfMoreInfo": [
        {
          "textList": "在紧急情况下使用的刺激剂"
        },
        {
          "textList": "在医疗场所中较为罕见"
        }
      ]
    }
  ]
