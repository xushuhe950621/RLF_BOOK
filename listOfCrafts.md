合成项目配置  
字段 | 类型 | 描述  
---|---|---  
craftID | string | 合成项目的唯一标识符。  
categoryID | string | 所属的合成分类标识符。  
craftTitle | string | 合成项目的本地化名称键。  
craftIcon | string | 合成项目图标路径。支持 .edds 格式。  
ingredients | array | 所需材料数组。每项包含 itemID（物品标识符）、count（数量）。  
results | array | 合成结果数组。每项包含 itemID（物品标识符）、count（数量）。  
craftTime | int | 合成所需时间（秒）。  
craftSkill | string | 技能需求标识符。  
craftRank | int | 合成等级需求（例如 1 = 初级, 2 = 中级, 3 = 高级）。  

示例配置：  
"listOfCrafts": [
{
"craftID": "exampleCraft1",
"categoryID": "Other",
"craftTitle": "示例合成 1",
"craftIcon": "relife_Core/images/icons/example.edds",
"ingredients": [
{ "itemID": "item1", "count": 2 },
{ "itemID": "item2", "count": 1 }
],
"results": [
{ "itemID": "item3", "count": 1 }
],
"craftTime": 30,
"craftSkill": "basicCrafting",
"craftRank": 1
}
]
