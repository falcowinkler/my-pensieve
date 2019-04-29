
---

KSQL streams take n kafka streams and create a new stream based on their SQL query. KSQL tables also create an underlying stream, but that stream is a changelog of an aggregation-query. If you select from a table within KSQL, that means you are selecting from a table that has just the latest value for each key of that query.