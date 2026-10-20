<!--
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
 with the License.  You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 -->

# Python API reference

The [Python API reference](pydocs/index.html) documents Sedona's Python modules, classes, and functions, including their parameters and return types.

For functions used with PySpark DataFrames, see the [SQL function reference](pydocs/sedona.spark.sql.html). For example, [ST_Length](pydocs/sedona.spark.sql.html#sedona.spark.sql.st_functions.ST_Length) calculates the length of a linestring geometry:

```python
from sedona.spark.sql.st_functions import ST_Length

df.select(ST_Length("geometry").alias("length"))
```

This example assumes a DataFrame named `df` with a geometry column named `geometry` and a Spark session configured with Sedona. See the [Python installation guide](../setup/install-python.md) for setup instructions and the [DataFrame API guide](sql/DataFrameAPI.md) for argument conventions and more examples.
