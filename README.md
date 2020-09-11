# 基金净值获取三部曲

## 第一步：全量获取
	文件名形如：510880_lsjz.csv
## 第二步：过滤排序
	文件名形如：510880_lsjz_sort.csv
保留列表项如下：<br>
| 日期 | 单位净值 | 历史净值 | 日增长率 | 申购状态 | 赎回状态 |
|----- | ------- | -------- | ------- | ------- | --------|
|2012/8/9| 1 | 1 | % | 场内买入 | 场内卖出|
|2012/8/10 | 1.0001 | 1.0001 | 0.01% | 场内买入 | 场内卖出|
| 2012/8/17 | 1.0003 | 1.0003| 0.02% | 场内买入 | 场内卖出 |
| 2012/8/24 | 1.0008| 1.0008 | 0.05% | 场内买入 | 场内卖出 |
|...| ... | ... | ... | ... |... |
|2020/9/10|1.1075|1.1575|-0.58%|场内买入 | 场内卖出 |

## 第三步：增量获取
	在第二步文件基础上进行追加增量净值信息，文件名保持不变

# 净值估值表（初步计划）
| 基金代码 | 基金名称 | 昨日净值 | 估值区间|
| 510890 | 红利ETF | 1.1075 | 低 | 偏低 | 偏高 | 高 |
|        |         |        | -- | -- | -- | -- |
|        |         |        | 0.8035-0.9919|0.9919-1.1118|1.1118-1.1906|1.1906-1.4136|
| ----   |   ---   |   ---  | -----------------------------------------------------|
