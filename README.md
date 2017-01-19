# data_science
data science projects

code to download, process, and analyze [Chicago's publicly available taxi data](http://digital.cityofchicago.org/index.php/chicago-taxi-data-released/).

Something of a companion to the [nyc-taxi-data](https://github.com/toddwschneider/nyc-taxi-data) repo. The repos share some similar code and structure, but do not explicitly depend on each other.

## Instructions

##### 1. Install [PostgreSQL](http://www.postgresql.org/download/) and [PostGIS](http://postgis.net/install)

Both are available via [Homebrew](http://brew.sh/) on Mac OS X

##### 2. Download and import Chicago taxi data

Note: the raw data is a single uncompressed ~40GB .csv file, it will take a little while to download!

```
./download_raw_data.sh
./initialize_database.sh
./import_trip_data.sh
```

##### 3. Analysis

`prepare_analysis.sql` and `analysis.R` scripts to do analysis in Postgres and [R](https://www.r-project.org/)

