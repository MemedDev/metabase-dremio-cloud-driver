# metabase-dremio-cloud-driver

Dremio Cloud driver for Metabase BI

Tested on:

-   Dremio Cloud
-   Metabase 0.43.0+


## Which features works

Dremio Driver can works in most metabase functionalities:

-   get correct data type for columns
-   support filter by numbers & strings & datetime
-   get table lists
-   x-ray on dremio tables


## How to use

1.  Download the dremio.metabase-driver.jar from releases
2.  Put it under metabase's plugins folder (plugins folder is at the same parent folder with metabase.jar)
3.  Restart metabase


## Building the driver

For Metabase 0.43.0+, there were many changes, for exmample, the build tool changed from lein to Clojure CLI Tools. So, the build steps for metabase-dremio-cloud-driver 1.1.x also changed.

### Prereq: Build Metabase source locally

Please refer to [Building Metabase](https://www.metabase.com/docs/latest/developers-guide/build.html) document.

### Build metabase-dremio-driver

clone the source code, and put it under the same parent folder as metabase's source code.

then, run

```shell
clojure -X:build :project-dir "\"$(pwd)\""
```

The generated "dremio.metabase-driver.jar" can be found in target folder


## Thanks

Based on <https://github.com/Baoqi/metabase-dremio-driver>.