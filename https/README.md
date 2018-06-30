# 爬虫情况说明

## 页面对照表

| 文件名    | 网页         | 地址                                                    |
| --------- | ------------ | :------------------------------------------------------ |
| plan.http | 全国高校查询 | https://gkcx.eol.cn/soudaxue/queryProvinceScoreNum.html |

## 全国高校查询

### 参数说明

| 请求参数            | 含义                         | 用法                                                                 |
| ------------------- | ---------------------------- | -------------------------------------------------------------------- |
| `messtype`          | 返回值类型                   | 填 `JSON`                                                            |
| `lunum`             |                              |                                                                      |
| `callback`          | JSONP 函数名                 |                                                                      |
| `provinceforschool` | 学校所在省份                 |                                                                      |
| `schooltype`        | 学历层次                     |                                                                      |
| `page`              | 当前页                       | 从 1 开始，根据返回值中的 `totalRecord` 字段获取和 `size` 计算最大值 |
| `size`              | 每页数量                     | 10                                                                   |
| `keyWord`           | 查询关键词                   |                                                                      |
| `schoolproperty`    | 院校分类                     |                                                                      |
| `schoolflag`        |                              |                                                                      |
| `province`          | 查撇省份                     |                                                                      |
| `fstype`            | 理科或文科                   |                                                                      |
| `zhaoshengpici`     | 招生批次                     |                                                                      |
| `fsyear`            |                              |                                                                      |
| `_`                 | 查询发起时的 Unix 时间偏移量 | 利用 momnet 库或 JS 原生 `Date` 类的 `getTime` 方法获取              |