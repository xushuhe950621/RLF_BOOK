用于合成的分类配置

| 字段            | 类型      | 描述                                                                 |
| --------------- | --------- | -------------------------------------------------------------------- |
| `categoryID`    | `string`  | 分类的唯一标识符，需要在合成配置中引用！                              |
| `categoryTitle` | `string`  | 分类名称的本地化键。通常形式为 `#STR_...`，也可以直接写中文名称         |
| `categoryIcon`  | `string`  | 分类图标的路径。支持 `.edds` 格式。                                   |

```json
 "listOfCraftCategories": [
        {
            "categoryID": "Cannabis",
            "categoryTitle": "大麻",
            "categoryIcon": "relife_Core/images/icons/abstract-002.edds"
        },
        {
            "categoryID": "Other",
            "categoryTitle": "其他",
            "categoryIcon": "relife_Core/images/icons/abstract-001.edds"
        }
    ],
