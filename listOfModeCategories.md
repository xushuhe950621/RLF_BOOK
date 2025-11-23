配置子分类。每个大分类都可以拥有自己的子分类，而“全部”分类始终存在。

| 字段            | 类型      | 描述                                                                 |
| --------------- | --------- | -------------------------------------------------------------------- |
| `categoryID`    | `string`  | 子分类的唯一标识符，必须唯一！                 |
| `categoryTitle` | `string`  | 子分类名称的本地化键。通常格式为 `#STR_...`，也可以直接写名称 |
| `categoryIcon`  | `string`  | 子分类图标路径。支持 `.edds` 格式。                  |


## 各主分类的子分类示例
```json
  "Places": [
        {
            "categoryID": "TestCat",
            "categoryTitle": "毒区材料",
            "categoryIcon": "relife_Core/images/icons/abstract-001.edds"
        }
    ],
    "Drugs": [
        {
            "categoryID": "TestCat",
            "categoryTitle": "示例分类",
            "categoryIcon": "relife_Core/images/icons/abstract-001.edds"
        },
        {
            "categoryID": "TestCat2",
            "categoryTitle": "示例分类 2",
            "categoryIcon": "relife_Core/images/icons/abstract-001.edds"
        }
    ],
