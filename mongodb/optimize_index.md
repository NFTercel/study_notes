mongodb索引优化
======================

1, geoWithin距离筛选时，使用2dsphere索引比2d索引快很多。

实际项目中，单表1亿数据时，如果用2d索引，则一次查询要500ms左右；而改为2dsphere索引后，只要30ms左右。

