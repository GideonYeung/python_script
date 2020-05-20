# python_script

## 1. WbGrawler.py 爬取微博图片。
## 2. city.py 爬取国家统计局数据。
## 3. 爬取国家统计局需要的sql：
DROP TABLE IF EXISTS `tab_citys`;
CREATE TABLE `tab_citys` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `parent_id` int(11) DEFAULT NULL,
  `city_name_zh` varchar(20) NOT NULL,
  `city_name_en` varchar(20) DEFAULT NULL,
  `city_level` int(11) NOT NULL,
  `city_code` char(12) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=742037 DEFAULT CHARSET=utf8;
