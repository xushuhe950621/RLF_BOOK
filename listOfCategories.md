分类配置  
字段 | 类型 | 描述  
---|---|---  
showCategory | int | 是否显示该分类（1 — 显示，0 — 隐藏）。  
categoryID | string | 分类的唯一标识符，用于代码中，请勿修改！  
categoryTitle | string | 分类名称的本地化键。通常形式为 #STR_.... 或直接写名称  
categoryIcon | string | 分类图标的路径。支持 .edds 格式。  

在配置中添加分类只会让它出现在界面中，但点击时不会执行任何动作。  
你只能修改分类的名称、是否显示以及图标。
