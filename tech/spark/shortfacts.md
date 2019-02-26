
---

When including dependencies such as `org.apache.spark:spark-avro_2.12:2.4.0` one needs to include the Service specification in META-INF folder, meaning you have to add the class `org.apache.spark.sql.avro.AvroFileFormat` to `src/main/resources/META-INF/services/org.apache.spark.sql.sources.DataSourceRegister`