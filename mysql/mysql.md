## 常用命令
### 查询
- SELECT left(`id`, 10) as pid FROM `data_stat_news_hours` group by `pid` order by `pid` desc limit 10,20 \G;
