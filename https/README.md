# 爬虫情况说明

- [页面对照表](#%E9%A1%B5%E9%9D%A2%E5%AF%B9%E7%85%A7%E8%A1%A8)
- [全国高校查询](#%E5%85%A8%E5%9B%BD%E9%AB%98%E6%A0%A1%E6%9F%A5%E8%AF%A2)
    - [参数说明](#%E5%8F%82%E6%95%B0%E8%AF%B4%E6%98%8E)

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