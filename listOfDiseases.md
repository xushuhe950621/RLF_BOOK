# 疾病描述参数 "listOfDiseases"

## 数据结构

该对象是一个包含疾病信息的数组，每个疾病具有以下结构：

### 疾病的主要参数

| 参数 | 类型 | 描述 |
|----------|-----|----------|
| `diseasesTitle` | String | 疾病名称 |
| `iconPath` | String | 疾病图标路径 |
| `timeEffect` | Float | 作用持续时间或影响时间 |
| `diseasesSymptom` | Array[Object] | 疾病症状的数组 |
| `diseasesCause` | Array[Object] | 疾病成因的数组 |
| `diseasesHeal` | Array[Object] | 疾病治疗方式的数组 |

### 症状和成因的结构

| 参数 | 类型 | 描述 |
|----------|-----|----------|
| `textList` | String | 症状或成因的文本描述 |

## 使用示例

```json
{
  "diseasesTitle": "痔疮",
  "iconPath": "relife_BookSystem/images/diseases.edds",
  "timeEffect": 100.0,
  "diseasesSymptom": [
    {
      "textList": "疾病症状的描述"
    }
  ],
  "diseasesHeal": [
    {
      "textList": "疾病治疗方法的描述"
    }
  ],
  "diseasesCause": [
    {
      "textList": "疾病成因的描述"
    },
    {
      "textList": "疾病成因的描述 2"
    }
  ]
}
