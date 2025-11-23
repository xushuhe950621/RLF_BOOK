| 参数                         | 类型            | 描述                               |
| -------------------------- | ------------- | -------------------------------- |
| `isShowCraft`              | Integer       | 是否在界面中显示该配方                      |
| `isAutoShowIngredients`    | Integer       | 是否自动显示配方的材料                      |
| `categoryID`               | String        | 合成所属分类的 ID，如果留空则显示在“所有合成”中       |
| `craftItemClassname`       | String        | 合成后生成的物品类名                       |
| `isAutoFindResults`        | Integer       | 是否自动从所有继承自 RecipeBase 的配方中查找合成结果 |
| `CraftHandleName`          | Array[String] | 如果关闭自动查找结果，这里填写手动指定的配方类名         |
| `NeedPerk`                 | Integer       | 所需技能（ID）                         |
| `needItemInInventory`      | Array         | 在玩家物品栏中必须存在的物品列表                 |
| `needItemInInventoryCount` | Array         | 对应物品所需数量                         |
| `craftHandleDisplayName`   | String        | 合成配方在界面中的显示名称                    |
| `IngredientsOneIcon`       | String        | 第一个材料的图标                         |
| `IngredientsTwoIcon`       | String        | 第二个材料的图标                         |
| `ignoredCraftToDisplay`    | Array[String] | 在显示中需要忽略的配方列表                    |
| `ingredientsOneList`       | Array[String] | 第一个材料的可用物品列表                     |
| `ingredientsTwoList`       | Array[String] | 第二个材料的可用物品列表                     |

使用示例
```json
{
  "isShowCraft": 1,
  "isAutoShowIngredients": 0,
  "craftItemClassname": "RLF_Ignited_Cigare",
  "isAutoFindResults": 1,
  "CraftHandleName": ["CraftClass"],
  "NeedPerk": -1,
  "needItemInInventory": [],
  "needItemInInventoryCount": [],
  "craftHandleDisplayName": "",
  "IngredientsOneIcon": "",
  "IngredientsTwoIcon": "",
  "ignoredCraftToDisplay": ["craft1", "craft2"],
  "ingredientsOneList": ["Rag"],
  "ingredientsTwoList": ["NailBox"]
}
