# “生物（Entity）” 配置

## 概述

此配置定义了游戏中的生物（怪物/动物）列表，包括它们的属性、描述与图像。  
每个生物包含生命值、攻击性、分布区域以及击杀方式的信息。

### 生物对象的属性

在 `listOfEntity` 数组中的每个生物具有以下属性：

| 属性 | 类型 | 描述 |
|----------|-----|----------|
| `categoryID` | String | 分类 ID |
| `entityClassname` | String | 游戏中生物类的技术名称 |
| `entityTitle` | String | 生物的显示名称（可用于覆盖默认名称） |
| `entityDesc` | String | 生物的详细描述 |
| `entityLocation` | String | 生物的栖息地或出现区域 |
| `killInfo` | String | 有关如何击杀生物的策略与提示 |
| `entityHealth` | Number | 生物的生命值数量（-1 = 从游戏中自动读取） |
| `entityPowerType` | Number | 攻击性类型：0 - 中立、1 - 攻击性、2 - 温和 |
| `imageSmallEntity` | String | 生物的小图标路径（用于列表显示） |
| `imageEntity` | String | 生物的大图路径，若填写则替代模型预览 |

## 配置示例

```json
[
    {
      "entityClassname": "Animal_UrsusArctos",
      "entityTitle": "棕熊",
      "entityDesc": "大型掠食者，生活在森林地区。在保护领地或幼崽时表现出强烈攻击性。嗅觉和听觉极佳。",
      "entityLocation": "针叶林、混合林、山区",
      "killInfo": "适合使用大口径枪械对付。避免近身战斗。对头部射击更为有效。",
      "entityHealth": 800,
      "entityPowerType":1,
      "imageSmallEntity": "relife_BookSystem/images/entities/bear_small.edds",
      "imageEntity": "relife_BookSystem/images/entities/bear_large.edds"
    },
    {
      "entityClassname": "Animal_CapraHircus",
      "entityTitle": "野山羊",
      "entityDesc": "中型草食动物。胆小易逃跑，是良好的肉类和皮革来源。",
      "entityLocation": "山坡、丘陵地区",
      "killInfo": "任何武器都能轻松击杀。由于靠近时会逃跑，建议远距离射击。",
      "entityHealth": 150,
      "entityPowerType": 2,
      "imageSmallEntity": "relife_BookSystem/images/entities/goat_small.edds",
      "imageEntity": "relife_BookSystem/images/entities/goat_large.edds"
    },
    {
      "entityClassname": "Infected_Runner",
      "entityTitle": "感染者·奔跑者",
      "entityDesc": "感染早期的人类，仍然具备高速移动能力，但失去理智。",
      "entityLocation": "城市区域、废弃定居点",
      "killInfo": "对头部射击最为有效。会成群攻击。由于速度快，近战极其危险。",
      "entityHealth": 120,
      "entityPowerType": 1,
      "imageSmallEntity": "relife_BookSystem/images/entities/runner_small.edds",
      "imageEntity": "relife_BookSystem/images/entities/runner_large.edds"
    }
  ]
