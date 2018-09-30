# Cisco ASA Notes

- Cisco ASAs will generate a LOT of data. So take special care of the shard settings for these indices. 
- In general, 50GB shard sizes is about the preferred norm. So if number of shards is '6' this should allow for 300GB indices. However if your index sizes start to get larger than this, then it may be best to consider moving from daily to hourly indices.
- As always, keep an eye on the index sizes then make decisions from there. 