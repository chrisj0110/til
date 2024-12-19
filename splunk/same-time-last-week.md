# Searching same time period last week

To overlay the same data from a week ago, for example for a timechart over the last 48 hours:

```
index=my_index earliest=-2d | timechart count as 48hours
| appendcols [search index="my_index" earliest=-9d latest =-7d | timechart count as LastWeek]
```

If you're looking at a full week, for example, then you can use `timewrap` from https://apps.splunk.com/app/1645/, like:

```
index=my_index | timechart count | timewrap w
```
