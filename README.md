# MyBigDataknowledge
## Flink
### WaterMark 是什么
WaterMark是通过时间推进的，在事件时间语义的窗口计算中，由事件时间推进，当WaterMark被推进到窗口计算的阈值时触发窗口计算。方便Flink处理乱序的事件。比如在Flink中创建了一个10s的窗口，允许延迟的事件为3s，那么当事件时间推进到13s时，WaterMark才会被推进到10s，即触发第一次窗口计算。
