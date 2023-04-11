# Comparing `tmp/osmsg-0.1.8.tar.gz` & `tmp/osmsg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmsg-0.1.8.tar", last modified: Tue Feb 28 10:09:15 2023, max compression
+gzip compressed data, was "osmsg-0.1.9.tar", last modified: Wed Mar  1 06:22:21 2023, max compression
```

## Comparing `osmsg-0.1.8.tar` & `osmsg-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-02-28 10:09:15.924600 osmsg-0.1.8/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       33 2023-01-31 12:02:37.000000 osmsg-0.1.8/MANIFEST.in
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    10362 2023-02-28 10:09:15.914600 osmsg-0.1.8/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    10090 2023-02-27 14:33:40.000000 osmsg-0.1.8/README.md
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-02-28 10:09:15.854600 osmsg-0.1.8/data/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)  5499774 2023-01-30 06:25:38.000000 osmsg-0.1.8/data/countries_un.geojson
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-02-28 10:09:15.904600 osmsg-0.1.8/osmsg/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)        0 2023-01-25 07:15:16.000000 osmsg-0.1.8/osmsg/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    38272 2023-02-28 09:50:06.000000 osmsg-0.1.8/osmsg/app.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     6231 2023-02-28 09:00:58.000000 osmsg-0.1.8/osmsg/changefiles.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4997 2023-02-27 14:31:38.000000 osmsg-0.1.8/osmsg/changesets.py
--rwxr-xr-x   0 kshitij   (1000) kshitij   (1000)    17071 2023-02-28 09:00:58.000000 osmsg-0.1.8/osmsg/utils.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-02-28 10:09:15.914600 osmsg-0.1.8/osmsg.egg-info/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    10362 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      319 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/SOURCES.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)        1 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/dependency_links.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       41 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/entry_points.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       99 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/requires.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)        6 2023-02-28 10:09:15.000000 osmsg-0.1.8/osmsg.egg-info/top_level.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2023-02-28 10:09:15.924600 osmsg-0.1.8/setup.cfg
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      831 2023-02-28 10:08:58.000000 osmsg-0.1.8/setup.py
+drwxr-xr-x   0 kshitij    (501) staff       (20)        0 2023-03-01 06:22:21.228127 osmsg-0.1.9/
+-rw-r--r--   0 kshitij    (501) staff       (20)       33 2023-02-01 05:43:00.000000 osmsg-0.1.9/MANIFEST.in
+-rw-r--r--   0 kshitij    (501) staff       (20)    12302 2023-03-01 06:22:21.227841 osmsg-0.1.9/PKG-INFO
+-rw-r--r--   0 kshitij    (501) staff       (20)    12030 2023-03-01 06:22:03.000000 osmsg-0.1.9/README.md
+drwxr-xr-x   0 kshitij    (501) staff       (20)        0 2023-03-01 06:22:21.215551 osmsg-0.1.9/data/
+-rw-r--r--   0 kshitij    (501) staff       (20)  5499774 2023-02-01 05:18:18.000000 osmsg-0.1.9/data/countries_un.geojson
+drwxr-xr-x   0 kshitij    (501) staff       (20)        0 2023-03-01 06:22:21.226172 osmsg-0.1.9/osmsg/
+-rw-r--r--   0 kshitij    (501) staff       (20)        0 2023-01-16 10:16:28.000000 osmsg-0.1.9/osmsg/__init__.py
+-rw-r--r--   0 kshitij    (501) staff       (20)    40436 2023-03-01 06:22:03.000000 osmsg-0.1.9/osmsg/app.py
+-rw-r--r--   0 kshitij    (501) staff       (20)     6476 2023-03-01 06:22:03.000000 osmsg-0.1.9/osmsg/changefiles.py
+-rw-r--r--   0 kshitij    (501) staff       (20)     4997 2023-02-25 06:45:22.000000 osmsg-0.1.9/osmsg/changesets.py
+-rwxr-xr-x   0 kshitij    (501) staff       (20)    17216 2023-03-01 06:22:03.000000 osmsg-0.1.9/osmsg/utils.py
+drwxr-xr-x   0 kshitij    (501) staff       (20)        0 2023-03-01 06:22:21.227591 osmsg-0.1.9/osmsg.egg-info/
+-rw-r--r--   0 kshitij    (501) staff       (20)    12302 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/PKG-INFO
+-rw-r--r--   0 kshitij    (501) staff       (20)      319 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 kshitij    (501) staff       (20)        1 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 kshitij    (501) staff       (20)       41 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/entry_points.txt
+-rw-r--r--   0 kshitij    (501) staff       (20)       99 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/requires.txt
+-rw-r--r--   0 kshitij    (501) staff       (20)        6 2023-03-01 06:22:21.000000 osmsg-0.1.9/osmsg.egg-info/top_level.txt
+-rw-r--r--   0 kshitij    (501) staff       (20)       38 2023-03-01 06:22:21.228183 osmsg-0.1.9/setup.cfg
+-rw-r--r--   0 kshitij    (501) staff       (20)      831 2023-03-01 06:22:09.000000 osmsg-0.1.9/setup.py
```

### Comparing `osmsg-0.1.8/PKG-INFO` & `osmsg-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmsg
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenStreetMap Stats Generator : Commandline
 Home-page: https://github.com/kshitijrajsharma/OSMSG
 Author: Kshitij Raj Sharma
 Author-email: skshitizraj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -29,62 +29,83 @@
 ```
 pip install osmsg
 ```
 
 ### Usage:
 
 ```
-osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME] [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME]
-             [--country COUNTRY] [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]] [--force] [--rows ROWS] [--workers WORKERS] [--url URL] [--last_week]
-             [--last_day] [--last_month] [--last_year] [--last_hour] [--charts] [--summary] [--exact_lookup] [--changeset] [--all_tags] [--exclude_date_in_name]
-             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]] [--read_from_metadata READ_FROM_METADATA]
+osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME]
+             [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME] [--country COUNTRY]
+             [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]]
+             [--length LENGTH [LENGTH ...]] [--force] [--rows ROWS] [--workers WORKERS]
+             [--url URL [URL ...]] [--last_week] [--last_day] [--last_month] [--last_year]
+             [--last_hour] [--days DAYS] [--charts] [--summary] [--exact_lookup] [--changeset]
+             [--all_tags] [--temp] [--exclude_date_in_name]
+             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]]
+             [--read_from_metadata READ_FROM_METADATA]
 ```
 
 ### Options:
 
 ```
   -h, --help            show this help message and exit
   --start_date START_DATE
                         Start date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --end_date END_DATE   End date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --username USERNAME   Your OSM Username : Only required for Geofabrik Internal Changefiles
   --password PASSWORD   Your OSM Password : Only required for Geofabrik Internal Changefiles
   --timezone {Nepal,UTC}
                         Your Timezone : Currently Supported Nepal, Default : UTC
   --name NAME           Output stat file name
-  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until day stats since changeset replication is available for minute,
-                        avoid using for geofabrik url since geofabrik already gives country level changefiles
+  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until
+                        day stats since changeset replication is available for minute, avoid using
+                        for geofabrik url since geofabrik already gives country level changefiles
   --tags TAGS [TAGS ...]
                         Additional stats to collect : List of tags key
   --hashtags HASHTAGS [HASHTAGS ...]
-                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats for now , Only lookups if hashtag is contained on the string ,
-                        not a exact string lookup on beta
+                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats
+                        for now , Only lookups if hashtag is contained on the string , not a exact
+                        string lookup on beta
+  --length LENGTH [LENGTH ...]
+                        Calculate length of osm features , Only Supported for way created features ,
+                        Pass list of tags key to calculate eg : --length highway waterway , Unit is
+                        in Meters
   --force               Force for the Hashtag Replication fetch if it is greater than a day interval
   --rows ROWS           No. of top rows to extract , to extract top 100 , pass 100
-  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware to use this max no of workers may cause overuse of resources
-  --url URL             Your public OSM Change Replication URL
+  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware
+                        to use this max no of workers may cause overuse of resources
+  --url URL [URL ...]   Your public list of OSM Change Replication URL , 'minute,hour,day' option by
+                        default will translate to planet replciation url. You can supply multiple
+                        urls for geofabrik country updates , Url should not have trailing / at the
+                        end
   --last_week           Extract stats for last week
   --last_day            Extract Stats for last day
   --last_month          Extract Stats for last Month
   --last_year           Extract stats for last year
   --last_hour           Extract stats for Last hour
+  --days DAYS           N nof of last days to extract , for eg if 3 is supplied script will generate
+                        stats for last 3 days
   --charts              Exports Summary Charts along with stats
   --summary             Produces Summary.md file with summary of Run
-  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this hashtag search will search for the existence of text on hashtags and
-                        comments
-  --changeset           Include hashtag and country informations on the stats. It forces script to process changeset replciation , Careful to use this since changeset
+  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this
+                        hashtag search will search for the existence of text on hashtags and comments
+  --changeset           Include hashtag and country informations on the stats. It forces script to
+                        process changeset replciation , Careful to use this since changeset
                         replication is minutely
   --all_tags            Extract statistics of all of the unique tags and its count
+  --temp                Deletes downloaded osm files from machine after processing is done , if you
+                        want to run osmsg on same files again keep this option turn off
   --exclude_date_in_name
-                        By default from and to date will be added to filename , You can skip this behaviour with this option
+                        By default from and to date will be added to filename , You can skip this
+                        behaviour with this option
   --format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]
                         Stats output format
   --read_from_metadata READ_FROM_METADATA
-                        Location of metadata to pick start date from previous run's end_date , Generally used if you want to run bot on regular interval using
-                        cron/service
+                        Location of metadata to pick start date from previous run's end_date ,
+                        Generally used if you want to run bot on regular interval using cron/service
 ```
 
 It is a Simple python script processes osm files live and produces stats on the fly
 
 1. It can Generate Stats on Country Level for countries . Countries are available in [here](./data/countries_un.csv)
 2. It can also take any other server replication changefile to extract stats (Tested with Geofabrik and Planet Replication)
 3. Can Generate hashtag statistics
@@ -95,14 +116,16 @@
 ```
 {"name":"username","uid":uid,"changesets":1,"nodes.create":1071,"nodes.modify":2100,"nodes.delete":0,"ways.create":146,"ways.modify":69,"ways.delete":0,"relations.create":0,"relations.modify":1,"relations.delete":0,"building.create":138,"building.modify":11,"building.delete":0,"highway.create":5,"highway.modify":49,"highway.delete":0,"waterway.create":0,"waterway.modify":4,"waterway.delete":0,"amenity.create":0,"amenity.modify":3,"amenity.delete":0,"landuse.create":3,"landuse.modify":1,"landuse.delete":0,"natural.create":0,"natural.modify":3,"natural.delete":0,"total_map_changes":3387}
 ```
 
 ### Start Right Away :
 
 - Extract Stat of last hour and visualize stats/charts
+  
+  By default replication is minute url.
 
 ```
 osmsg --last_hour --charts --changeset
 ```
 
 ### More Example Commands
 
@@ -111,17 +134,18 @@
 ```
 osmsg --url "https://planet.openstreetmap.org/replication/minute" --format csv --tags building highway waterway amenity --name stats --all_tags --last_hour
 ```
 
 In order to extract for specific country just add --country with country name as in [data/countries_un.csv](./data/countries_un.csv) for eg : For Nepal : `--country Nepal`
 
 - To extract stats for last day whole world with all the tags and specified stat :
-
+  
+  You can either pass url "https://planet.openstreetmap.org/replication/day" itself or if you want to use planet default replciation url you can simply pass as : minute , day & hour , script will get url itself  
 ```
-osmsg  --url "https://planet.openstreetmap.org/replication/day" --format csv --last_day --name stats --all_tags
+osmsg  --url day --format csv --last_day --name stats --all_tags
 ```
 
 If you wish to have tags with specific count for key you can include them as `--tags "building" "highway" ` & add --country to extract specific country , if you use geofabrik country updates you don't need to use --country option
 
 - To extract specific country with Geofabrik URL (extracts stats for 15 days custom date range)
 
 ```
@@ -135,27 +159,31 @@
 
   Processing geofabrik country based osm change files are faster as they will have changes only for country and smaller in size
 
 ```
 osmsg --start_date "2022-01-01 00:00:00+00:00" --url "http://download.geofabrik.de/asia/nepal-updates" --username 'your osm username' --password 'user osm password' --tags 'building' 'highway' 'waterway' 'amenity'  --format csv
 ```
 
+- Example of extract last 8 days of data for Turkey and Syria for hashtag smforst using geofabrik
+```
+osmsg --url http://download.geofabrik.de/europe/turkey-updates https://download.geofabrik.de/asia/syria-updates --username "OSM USERNAME" --password "OSM PASSWORD" --hashtags smforst --length highway --force --days 8 --tags building highway --all_tags
+```
 Check more commands examples inside `stats/` `stats_metadata.json`
 
 Now start generating stats with above sample commands
 
 ### TIPS & Tricks of using OSMSG:
 
 OSMSG uses/supports sources , --url provided on argument will be used for osm changefiles and for changeset it is default of planet replication/minute ( used for hashtag and country )
 
 1. To process weekly / monthly or yearly stats , Using minute replication might take forever on small machines , You can use daily replication files `/replication/day` to process faster and avoid network download issues for small minute fiels
 
 2. If you are generating stats for rightnow / past 10min / past 1 hour using specific timeframe , stick with minutely (Sometimes to reflect changes you made on stats , Planet may take few minutes)
 
-3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible
+3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible , To generate more than that you can supply multiple countries geofabrik urls so that script can go through only country changefiles as stated on example above for turkey and syria , similarly you can pass your countries url and generate monthly yearly etc 
 
 4. For Country stats , if you use the --country option : It will use the planet minutely changeset replication to determine the location of the cahngeset bbox centroid , which means to process larger time frame it might take time , to avoid this Use Geofabrik internal changefiles based on country , OSMSG Supports processing of those hence you can directly supply geofabrik changefiles url for country and produce yearly/monthly stats eg :
 
 ```
 osmsg --url "http://download.geofabrik.de/asia/nepal-updates" --username '${{ secrets.OSM_USERNAME }}' --password '${{ secrets.OSM_PASSWORD }}' --format csv --last_month --tags 'building' 'highway' 'waterway' 'amenity' --name last_month_stats  --all_tags
 ```
```

### Comparing `osmsg-0.1.8/README.md` & `osmsg-0.1.9/osmsg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: osmsg
+Version: 0.1.9
+Summary: OpenStreetMap Stats Generator : Commandline
+Home-page: https://github.com/kshitijrajsharma/OSMSG
+Author: Kshitij Raj Sharma
+Author-email: skshitizraj@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+
 # OpenStreetMap Stats Generator
 
 On the Fly Commandline Stats Generator for OpenStreetMap User Contributions
 
 I tweet stats Every day/week/month for Global/Region and #hotosm hashtag at https://twitter.com/stats_osm and store them [here](/stats/)
 
 Monitored stats are available under `stats`, Currently Bot monitors OSM as whole , hotosm hashtag , Nepal Country : weekly,monthly and yearly stats are stored in github and twitter
@@ -19,62 +29,83 @@
 ```
 pip install osmsg
 ```
 
 ### Usage:
 
 ```
-osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME] [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME]
-             [--country COUNTRY] [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]] [--force] [--rows ROWS] [--workers WORKERS] [--url URL] [--last_week]
-             [--last_day] [--last_month] [--last_year] [--last_hour] [--charts] [--summary] [--exact_lookup] [--changeset] [--all_tags] [--exclude_date_in_name]
-             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]] [--read_from_metadata READ_FROM_METADATA]
+osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME]
+             [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME] [--country COUNTRY]
+             [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]]
+             [--length LENGTH [LENGTH ...]] [--force] [--rows ROWS] [--workers WORKERS]
+             [--url URL [URL ...]] [--last_week] [--last_day] [--last_month] [--last_year]
+             [--last_hour] [--days DAYS] [--charts] [--summary] [--exact_lookup] [--changeset]
+             [--all_tags] [--temp] [--exclude_date_in_name]
+             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]]
+             [--read_from_metadata READ_FROM_METADATA]
 ```
 
 ### Options:
 
 ```
   -h, --help            show this help message and exit
   --start_date START_DATE
                         Start date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --end_date END_DATE   End date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --username USERNAME   Your OSM Username : Only required for Geofabrik Internal Changefiles
   --password PASSWORD   Your OSM Password : Only required for Geofabrik Internal Changefiles
   --timezone {Nepal,UTC}
                         Your Timezone : Currently Supported Nepal, Default : UTC
   --name NAME           Output stat file name
-  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until day stats since changeset replication is available for minute,
-                        avoid using for geofabrik url since geofabrik already gives country level changefiles
+  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until
+                        day stats since changeset replication is available for minute, avoid using
+                        for geofabrik url since geofabrik already gives country level changefiles
   --tags TAGS [TAGS ...]
                         Additional stats to collect : List of tags key
   --hashtags HASHTAGS [HASHTAGS ...]
-                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats for now , Only lookups if hashtag is contained on the string ,
-                        not a exact string lookup on beta
+                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats
+                        for now , Only lookups if hashtag is contained on the string , not a exact
+                        string lookup on beta
+  --length LENGTH [LENGTH ...]
+                        Calculate length of osm features , Only Supported for way created features ,
+                        Pass list of tags key to calculate eg : --length highway waterway , Unit is
+                        in Meters
   --force               Force for the Hashtag Replication fetch if it is greater than a day interval
   --rows ROWS           No. of top rows to extract , to extract top 100 , pass 100
-  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware to use this max no of workers may cause overuse of resources
-  --url URL             Your public OSM Change Replication URL
+  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware
+                        to use this max no of workers may cause overuse of resources
+  --url URL [URL ...]   Your public list of OSM Change Replication URL , 'minute,hour,day' option by
+                        default will translate to planet replciation url. You can supply multiple
+                        urls for geofabrik country updates , Url should not have trailing / at the
+                        end
   --last_week           Extract stats for last week
   --last_day            Extract Stats for last day
   --last_month          Extract Stats for last Month
   --last_year           Extract stats for last year
   --last_hour           Extract stats for Last hour
+  --days DAYS           N nof of last days to extract , for eg if 3 is supplied script will generate
+                        stats for last 3 days
   --charts              Exports Summary Charts along with stats
   --summary             Produces Summary.md file with summary of Run
-  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this hashtag search will search for the existence of text on hashtags and
-                        comments
-  --changeset           Include hashtag and country informations on the stats. It forces script to process changeset replciation , Careful to use this since changeset
+  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this
+                        hashtag search will search for the existence of text on hashtags and comments
+  --changeset           Include hashtag and country informations on the stats. It forces script to
+                        process changeset replciation , Careful to use this since changeset
                         replication is minutely
   --all_tags            Extract statistics of all of the unique tags and its count
+  --temp                Deletes downloaded osm files from machine after processing is done , if you
+                        want to run osmsg on same files again keep this option turn off
   --exclude_date_in_name
-                        By default from and to date will be added to filename , You can skip this behaviour with this option
+                        By default from and to date will be added to filename , You can skip this
+                        behaviour with this option
   --format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]
                         Stats output format
   --read_from_metadata READ_FROM_METADATA
-                        Location of metadata to pick start date from previous run's end_date , Generally used if you want to run bot on regular interval using
-                        cron/service
+                        Location of metadata to pick start date from previous run's end_date ,
+                        Generally used if you want to run bot on regular interval using cron/service
 ```
 
 It is a Simple python script processes osm files live and produces stats on the fly
 
 1. It can Generate Stats on Country Level for countries . Countries are available in [here](./data/countries_un.csv)
 2. It can also take any other server replication changefile to extract stats (Tested with Geofabrik and Planet Replication)
 3. Can Generate hashtag statistics
@@ -85,14 +116,16 @@
 ```
 {"name":"username","uid":uid,"changesets":1,"nodes.create":1071,"nodes.modify":2100,"nodes.delete":0,"ways.create":146,"ways.modify":69,"ways.delete":0,"relations.create":0,"relations.modify":1,"relations.delete":0,"building.create":138,"building.modify":11,"building.delete":0,"highway.create":5,"highway.modify":49,"highway.delete":0,"waterway.create":0,"waterway.modify":4,"waterway.delete":0,"amenity.create":0,"amenity.modify":3,"amenity.delete":0,"landuse.create":3,"landuse.modify":1,"landuse.delete":0,"natural.create":0,"natural.modify":3,"natural.delete":0,"total_map_changes":3387}
 ```
 
 ### Start Right Away :
 
 - Extract Stat of last hour and visualize stats/charts
+  
+  By default replication is minute url.
 
 ```
 osmsg --last_hour --charts --changeset
 ```
 
 ### More Example Commands
 
@@ -101,17 +134,18 @@
 ```
 osmsg --url "https://planet.openstreetmap.org/replication/minute" --format csv --tags building highway waterway amenity --name stats --all_tags --last_hour
 ```
 
 In order to extract for specific country just add --country with country name as in [data/countries_un.csv](./data/countries_un.csv) for eg : For Nepal : `--country Nepal`
 
 - To extract stats for last day whole world with all the tags and specified stat :
-
+  
+  You can either pass url "https://planet.openstreetmap.org/replication/day" itself or if you want to use planet default replciation url you can simply pass as : minute , day & hour , script will get url itself  
 ```
-osmsg  --url "https://planet.openstreetmap.org/replication/day" --format csv --last_day --name stats --all_tags
+osmsg  --url day --format csv --last_day --name stats --all_tags
 ```
 
 If you wish to have tags with specific count for key you can include them as `--tags "building" "highway" ` & add --country to extract specific country , if you use geofabrik country updates you don't need to use --country option
 
 - To extract specific country with Geofabrik URL (extracts stats for 15 days custom date range)
 
 ```
@@ -125,27 +159,31 @@
 
   Processing geofabrik country based osm change files are faster as they will have changes only for country and smaller in size
 
 ```
 osmsg --start_date "2022-01-01 00:00:00+00:00" --url "http://download.geofabrik.de/asia/nepal-updates" --username 'your osm username' --password 'user osm password' --tags 'building' 'highway' 'waterway' 'amenity'  --format csv
 ```
 
+- Example of extract last 8 days of data for Turkey and Syria for hashtag smforst using geofabrik
+```
+osmsg --url http://download.geofabrik.de/europe/turkey-updates https://download.geofabrik.de/asia/syria-updates --username "OSM USERNAME" --password "OSM PASSWORD" --hashtags smforst --length highway --force --days 8 --tags building highway --all_tags
+```
 Check more commands examples inside `stats/` `stats_metadata.json`
 
 Now start generating stats with above sample commands
 
 ### TIPS & Tricks of using OSMSG:
 
 OSMSG uses/supports sources , --url provided on argument will be used for osm changefiles and for changeset it is default of planet replication/minute ( used for hashtag and country )
 
 1. To process weekly / monthly or yearly stats , Using minute replication might take forever on small machines , You can use daily replication files `/replication/day` to process faster and avoid network download issues for small minute fiels
 
 2. If you are generating stats for rightnow / past 10min / past 1 hour using specific timeframe , stick with minutely (Sometimes to reflect changes you made on stats , Planet may take few minutes)
 
-3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible
+3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible , To generate more than that you can supply multiple countries geofabrik urls so that script can go through only country changefiles as stated on example above for turkey and syria , similarly you can pass your countries url and generate monthly yearly etc 
 
 4. For Country stats , if you use the --country option : It will use the planet minutely changeset replication to determine the location of the cahngeset bbox centroid , which means to process larger time frame it might take time , to avoid this Use Geofabrik internal changefiles based on country , OSMSG Supports processing of those hence you can directly supply geofabrik changefiles url for country and produce yearly/monthly stats eg :
 
 ```
 osmsg --url "http://download.geofabrik.de/asia/nepal-updates" --username '${{ secrets.OSM_USERNAME }}' --password '${{ secrets.OSM_PASSWORD }}' --format csv --last_month --tags 'building' 'highway' 'waterway' 'amenity' --name last_month_stats  --all_tags
 ```
```

### Comparing `osmsg-0.1.8/data/countries_un.geojson` & `osmsg-0.1.9/data/countries_un.geojson`

 * *Files identical despite different names*

### Comparing `osmsg-0.1.8/osmsg/app.py` & `osmsg-0.1.9/osmsg/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime as dt
 import json
 import os
 import re
 import shutil
 import sys
 import time
+import urllib.parse
 from datetime import datetime
 
 import dataframe_image as dfi
 import geopandas as gpd
 import humanize
 import osmium
 import pandas as pd
@@ -27,14 +28,15 @@
 )
 
 from .changefiles import (
     get_download_urls_changefiles,
     get_prev_hour,
     get_prev_year_dates,
     in_local_timezone,
+    last_days_count,
     previous_day,
     previous_month,
     previous_week,
     seq_to_timestamp,
     strip_utc,
 )
 from .changesets import ChangesetToolKit
@@ -308,15 +310,15 @@
         handler.apply_file(file_path[:-3], locations=True)
     else:
         handler.apply_file(file_path[:-3])
 
 
 def process_changesets(url):
     # print(f"Processing {url}")
-    file_path = get_file_path_from_url(url, "changesets")
+    file_path = get_file_path_from_url(url, "changeset")
     handler = ChangesetHandler()
     handler.apply_file(file_path[:-3])
     # print(f"Finished {url}")
 
 
 def auth(username, password):
     print("Authenticating...")
@@ -410,16 +412,17 @@
         type=int,
         default=None,
         help="No. of Parallel workers to assign : Default is no of cpu available , Be aware to use this max no of workers may cause overuse of resources",
     )
 
     parser.add_argument(
         "--url",
-        default="https://planet.openstreetmap.org/replication/minute",
-        help="Your public OSM Change Replication URL ",
+        nargs="+",
+        default=["https://planet.openstreetmap.org/replication/minute"],
+        help="Your public list of OSM Change Replication URL , 'minute,hour,day' option by default will translate to planet replciation url. You can supply multiple urls for geofabrik country updates , Url should not have trailing / at the end",
     )
 
     parser.add_argument(
         "--last_week",
         action="store_true",
         help="Extract stats for last week",
         default=False,
@@ -445,14 +448,20 @@
     parser.add_argument(
         "--last_hour",
         action="store_true",
         help="Extract stats for Last hour",
         default=False,
     )
     parser.add_argument(
+        "--days",
+        type=int,
+        default=None,
+        help="N nof of last days to extract , for eg if 3 is supplied script will generate stats for last 3 days",
+    )
+    parser.add_argument(
         "--charts",
         action="store_true",
         help="Exports Summary Charts along with stats",
         default=False,
     )
     parser.add_argument(
         "--summary",
@@ -477,17 +486,17 @@
     parser.add_argument(
         "--all_tags",
         action="store_true",
         help="Extract statistics of all of the unique tags and its count",
         default=False,
     )
     parser.add_argument(
-        "--store",
+        "--temp",
         action="store_true",
-        help="Stores downloaded osm files to machine itself to run different stats generation again, Will be useful if you are doing multiple analysis so that script will not download the files that are already downloaded",
+        help="Deletes downloaded osm files from machine after processing is done , if you want to run osmsg on same files again keep this option turn off",
         default=False,
     )
 
     parser.add_argument(
         "--exclude_date_in_name",
         action="store_true",
         help="By default from and to date will be added to filename , You can skip this behaviour with this option",
@@ -507,31 +516,35 @@
     )
 
     args = parser.parse_args()
     return args
 
 
 def main():
+    print("OSMSG : Waking up ......")
     args = parse_args()
     if args.start_date:
         start_date = strip_utc(
             dt.datetime.strptime(args.start_date, "%Y-%m-%d %H:%M:%S%z"), args.timezone
         )
 
     if not args.start_date:
         if (
             args.last_week
             or args.last_day
             or args.last_month
             or args.last_year
             or args.last_hour
+            or args.days
         ):
             pass
         else:
-            print("ERR: Supply start_date")
+            print(
+                "ERR: Supply start_date or extraction parameters such as last_day , last_hour"
+            )
             sys.exit()
 
     if args.end_date:
         end_date = args.end_date
         if not isinstance(end_date, datetime):
             end_date = dt.datetime.strptime(args.end_date, "%Y-%m-%d %H:%M:%S%z")
 
@@ -562,25 +575,59 @@
     hashtags = args.hashtags
     country = args.country
     cookies = None
     changeset = args.changeset
     exact_lookup = args.exact_lookup
     length = args.length
 
-    if "geofabrik" in args.url.lower():
-        if args.username is None:
-            args.username = os.environ.get("OSM_USERNAME")
-        if args.password is None:
-            args.password = os.environ.get("OSM_PASSWORD")
+    if args.url:
+        args.url = list(set(args.url))  # remove duplicates
+        for url in args.url:
+            if urllib.parse.urlparse(url).scheme == "":
+                # The URL is not valid
+                if url == "minute":
+                    args.url = ["https://planet.openstreetmap.org/replication/minute"]
+                elif url == "hour":
+                    args.url = ["https://planet.openstreetmap.org/replication/hour"]
+                elif url == "day":
+                    args.url = ["https://planet.openstreetmap.org/replication/day"]
+                else:
+                    print(f"Invalid input for urls {url}")
+                    sys.exit()
+            if url.endswith("/"):
+                print(f"{url} should not end with trailing /")
+                sys.exit()
 
-        if not (args.username and args.password):
-            assert (
-                args.username and args.password
-            ), "OSM username and password are required for geofabrik url"
-        cookies = auth(args.username, args.password)
+        if any("geofabrik" in url.lower() for url in args.url):
+            if args.username is None:
+                args.username = os.environ.get("OSM_USERNAME")
+            if args.password is None:
+                args.password = os.environ.get("OSM_PASSWORD")
+
+            if not (args.username and args.password):
+                assert (
+                    args.username and args.password
+                ), "OSM username and password are required for geofabrik url"
+            cookies = auth(args.username, args.password)
+
+    count = sum(
+        [
+            args.last_hour,
+            args.last_year,
+            args.last_month,
+            args.last_day,
+            args.last_week,
+            bool(args.days),
+        ]
+    )
+    if count > 1:
+        print(
+            "Error: only one of --last_hour, --last_year, --last_month, --last_day, --last_week, or --days should be specified."
+        )
+        sys.exit()
 
     if args.last_hour:
         start_date, end_date = get_prev_hour(args.timezone)
 
     if args.last_year:
         start_date, end_date = get_prev_year_dates(args.timezone)
 
@@ -588,14 +635,20 @@
         start_date, end_date = previous_month(args.timezone)
 
     if args.last_day:
         start_date, end_date = previous_day(args.timezone)
     if args.last_week:
         start_date, end_date = previous_week(args.timezone)
 
+    if args.days:
+        if args.days > 0:
+            start_date, end_date = last_days_count(args.timezone, args.days)
+        else:
+            print(f"Error : {args.days} should be greater than 0")
+            sys.exit()
     if args.read_from_metadata:
         if os.path.exists(args.read_from_metadata):
             with open(args.read_from_metadata, "r") as openfile:
                 # Reading from json file
                 meta_json = json.load(openfile)
             if "end_date" in meta_json:
                 start_date = datetime.strptime(
@@ -628,29 +681,28 @@
             changeset_start_seq,
             changeset_end_seq,
         ) = Changeset.get_download_urls(start_date, end_date)
         print(
             f"Processing Changeset from {strip_utc(Changeset.sequence_to_timestamp(changeset_start_seq),args.timezone)} to {strip_utc(Changeset.sequence_to_timestamp(changeset_end_seq),args.timezone)}"
         )
 
-        temp_path = os.path.join(os.getcwd(), "temp/changesets")
-        print(os.path.exists(temp_path))
+        temp_path = os.path.join(os.getcwd(), "temp/changeset", "changesets")
         if not os.path.exists(temp_path):
             os.makedirs(temp_path)
 
         max_workers = os.cpu_count() if not args.workers else args.workers
         print(f"Using {max_workers} Threads")
         print(
             "Downloading Changeset files using https://planet.openstreetmap.org/replication/changesets/"
         )
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             # Use `map` to apply the `download osm files` function to each element in the `urls` list
             for _ in tqdm(
                 executor.map(
-                    lambda x: download_osm_files(x, mode="changesets", cookies=cookies),
+                    lambda x: download_osm_files(x, mode="changeset", cookies=cookies),
                     changeset_download_urls,
                 ),
                 total=len(changeset_download_urls),
                 unit_scale=True,
                 unit="changesets",
                 leave=True,
             ):
@@ -670,78 +722,78 @@
                 pass
             # executor.shutdown(wait=True)
 
         print("Changeset Processing Finished")
         end_seq_timestamp = Changeset.sequence_to_timestamp(changeset_end_seq)
         if end_date > end_seq_timestamp:
             end_date = strip_utc(end_seq_timestamp, args.timezone)
+    for url in args.url:
+        print(f"Changefiles : Generating Download Urls Using {url}")
+        (
+            download_urls,
+            server_ts,
+            start_seq,
+            end_seq,
+            start_seq_url,
+            end_seq_url,
+        ) = get_download_urls_changefiles(start_date, end_date, url, args.timezone)
+        if server_ts < end_date:
+            print(
+                f"Warning : End date data is not available at server, Changing to latest available date {server_ts}"
+            )
+            end_date = server_ts
+            if start_date >= server_ts:
+                print("Err: Data is not available after start date ")
+                sys.exit()
+        global end_date_utc
+        global start_date_utc
 
-    print(f"Changefiles : Generating Download Urls Using {args.url}")
-    (
-        download_urls,
-        server_ts,
-        start_seq,
-        end_seq,
-        start_seq_url,
-        end_seq_url,
-    ) = get_download_urls_changefiles(start_date, end_date, args.url, args.timezone)
-    if server_ts < end_date:
+        start_date_utc = start_date.astimezone(dt.timezone.utc)
+        end_date_utc = end_date.astimezone(dt.timezone.utc)
         print(
-            f"Warning : End date data is not available at server, Changing to latest available date {server_ts}"
+            f"Final UTC Date time to filter stats : {start_date_utc} to {end_date_utc}"
         )
-        end_date = server_ts
-        if start_date >= server_ts:
-            print("Err: Data is not available after start date ")
-            sys.exit()
-    global end_date_utc
-    global start_date_utc
+        # Use the ThreadPoolExecutor to download the images in parallel
+        max_workers = os.cpu_count() if not args.workers else args.workers
+        print(f"Using {max_workers} Threads")
 
-    start_date_utc = start_date.astimezone(dt.timezone.utc)
-    end_date_utc = end_date.astimezone(dt.timezone.utc)
-    print(f"Final UTC Date time to filter stats : {start_date_utc} to {end_date_utc}")
-    temp_path = os.path.join(os.getcwd(), "temp/changefiles")
-    if not os.path.exists(temp_path):
-        os.makedirs(temp_path)
-
-    # Use the ThreadPoolExecutor to download the images in parallel
-    max_workers = os.cpu_count() if not args.workers else args.workers
-    print(f"Using {max_workers} Threads")
-
-    print("Downloading Changefiles")
-    with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-        # Use `map` to apply the `download osm files` function to each element in the `urls` list
-        for _ in tqdm(
-            executor.map(
-                lambda x: download_osm_files(x, mode="changefiles", cookies=cookies),
-                download_urls,
-            ),
-            total=len(download_urls),
-            unit_scale=True,
-            unit="changefiles",
-            leave=True,
-        ):
-            pass
-    print("Processing Changefiles")
+        print("Downloading Changefiles")
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+            # Use `map` to apply the `download osm files` function to each element in the `urls` list
+            for _ in tqdm(
+                executor.map(
+                    lambda x: download_osm_files(
+                        x, mode="changefiles", cookies=cookies
+                    ),
+                    download_urls,
+                ),
+                total=len(download_urls),
+                unit_scale=True,
+                unit="changefiles",
+                leave=True,
+            ):
+                pass
+        print("Processing Changefiles")
 
-    with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-        # Use `map` to apply the `download_image` function to each element in the `urls` list
-        # executor.map(process_changefiles, download_urls)
-        for _ in tqdm(
-            executor.map(process_changefiles, download_urls),
-            total=len(download_urls),
-            unit_scale=True,
-            unit="changefiles",
-            leave=True,
-        ):
-            pass
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+            # Use `map` to apply the `download_image` function to each element in the `urls` list
+            # executor.map(process_changefiles, download_urls)
+            for _ in tqdm(
+                executor.map(process_changefiles, download_urls),
+                total=len(download_urls),
+                unit_scale=True,
+                unit="changefiles",
+                leave=True,
+            ):
+                pass
 
-        # executor.shutdown(wait=True)
-    print("Changefiles Processing Finished")
+            # executor.shutdown(wait=True)
+        print(f"Changefiles Processing Finished using {url}")
     os.chdir(os.getcwd())
-    if not args.store:
+    if args.temp:
         shutil.rmtree("temp")
     if len(users) >= 1:
         # print(users)
         if args.all_tags:
             for user in users:
                 users[user]["tags_create"] = json.dumps(
                     dict(
```

### Comparing `osmsg-0.1.8/osmsg/changefiles.py` & `osmsg-0.1.9/osmsg/changefiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,22 @@
     today = datetime.today()
     previous_day = today - timedelta(days=1)
     return strip_utc(previous_day.strftime("%Y-%m-%d"), timezone), strip_utc(
         today.strftime("%Y-%m-%d"), timezone
     )
 
 
+def last_days_count(timezone, days):
+    today = datetime.today()
+    previous_day = today - timedelta(days=days)
+    return strip_utc(previous_day.strftime("%Y-%m-%d"), timezone), strip_utc(
+        today.strftime("%Y-%m-%d"), timezone
+    )
+
+
 def previous_week(timezone):
     today = datetime.today()
     start_date = today - timedelta(days=today.weekday() + 7)
     end_date = start_date + timedelta(days=6)
     return strip_utc(start_date.strftime("%Y-%m-%d"), timezone), strip_utc(
         end_date.strftime("%Y-%m-%d"), timezone
     )
```

### Comparing `osmsg-0.1.8/osmsg/changesets.py` & `osmsg-0.1.9/osmsg/changesets.py`

 * *Files identical despite different names*

### Comparing `osmsg-0.1.8/osmsg/utils.py` & `osmsg-0.1.9/osmsg/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,16 +480,15 @@
                 tag_counts[tag] = 0
             tag_counts[tag] += count
     return tag_counts
 
 
 def get_file_path_from_url(url, mode):
     url_splitted_list = url.split("/")
-    temp_path = os.path.join(os.getcwd(), f"temp/{mode}")
-
+    temp_path = os.path.join(os.getcwd(), f"temp/{mode}", url_splitted_list[-4])
     file_path = os.path.join(
         temp_path,
         f"{url_splitted_list[-3]}_{url_splitted_list[-2]}_{url_splitted_list[-1]}",
     )
     return file_path
 
 
@@ -508,14 +507,16 @@
             else:
                 response = requests.get(url)
 
             if not response.status_code == 200:
                 sys.exit()
 
             file_data = response.content
+            # Create the directory if it does not exist
+            os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
-            with open(file_path, "wb") as f:
+            with open(file_path, "xb") as f:
                 f.write(file_data)
 
         with gzip.open(file_path, "rb") as f_in, open(file_path[:-3], "wb") as f_out:
             shutil.copyfileobj(f_in, f_out)
         os.remove(file_path)
```

### Comparing `osmsg-0.1.8/osmsg.egg-info/PKG-INFO` & `osmsg-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: osmsg
-Version: 0.1.8
-Summary: OpenStreetMap Stats Generator : Commandline
-Home-page: https://github.com/kshitijrajsharma/OSMSG
-Author: Kshitij Raj Sharma
-Author-email: skshitizraj@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
 # OpenStreetMap Stats Generator
 
 On the Fly Commandline Stats Generator for OpenStreetMap User Contributions
 
 I tweet stats Every day/week/month for Global/Region and #hotosm hashtag at https://twitter.com/stats_osm and store them [here](/stats/)
 
 Monitored stats are available under `stats`, Currently Bot monitors OSM as whole , hotosm hashtag , Nepal Country : weekly,monthly and yearly stats are stored in github and twitter
@@ -29,62 +19,83 @@
 ```
 pip install osmsg
 ```
 
 ### Usage:
 
 ```
-osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME] [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME]
-             [--country COUNTRY] [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]] [--force] [--rows ROWS] [--workers WORKERS] [--url URL] [--last_week]
-             [--last_day] [--last_month] [--last_year] [--last_hour] [--charts] [--summary] [--exact_lookup] [--changeset] [--all_tags] [--exclude_date_in_name]
-             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]] [--read_from_metadata READ_FROM_METADATA]
+osmsg [-h] [--start_date START_DATE] [--end_date END_DATE] [--username USERNAME]
+             [--password PASSWORD] [--timezone {Nepal,UTC}] [--name NAME] [--country COUNTRY]
+             [--tags TAGS [TAGS ...]] [--hashtags HASHTAGS [HASHTAGS ...]]
+             [--length LENGTH [LENGTH ...]] [--force] [--rows ROWS] [--workers WORKERS]
+             [--url URL [URL ...]] [--last_week] [--last_day] [--last_month] [--last_year]
+             [--last_hour] [--days DAYS] [--charts] [--summary] [--exact_lookup] [--changeset]
+             [--all_tags] [--temp] [--exclude_date_in_name]
+             [--format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]]
+             [--read_from_metadata READ_FROM_METADATA]
 ```
 
 ### Options:
 
 ```
   -h, --help            show this help message and exit
   --start_date START_DATE
                         Start date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --end_date END_DATE   End date in the format YYYY-MM-DD HH:M:Sz eg: 2023-01-28 17:43:09+05:45
   --username USERNAME   Your OSM Username : Only required for Geofabrik Internal Changefiles
   --password PASSWORD   Your OSM Password : Only required for Geofabrik Internal Changefiles
   --timezone {Nepal,UTC}
                         Your Timezone : Currently Supported Nepal, Default : UTC
   --name NAME           Output stat file name
-  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until day stats since changeset replication is available for minute,
-                        avoid using for geofabrik url since geofabrik already gives country level changefiles
+  --country COUNTRY     Country name to extract (get name from data/un_countries) : Only viable until
+                        day stats since changeset replication is available for minute, avoid using
+                        for geofabrik url since geofabrik already gives country level changefiles
   --tags TAGS [TAGS ...]
                         Additional stats to collect : List of tags key
   --hashtags HASHTAGS [HASHTAGS ...]
-                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats for now , Only lookups if hashtag is contained on the string ,
-                        not a exact string lookup on beta
+                        Hashtags Statistics to Collect : List of hashtags , Limited until daily stats
+                        for now , Only lookups if hashtag is contained on the string , not a exact
+                        string lookup on beta
+  --length LENGTH [LENGTH ...]
+                        Calculate length of osm features , Only Supported for way created features ,
+                        Pass list of tags key to calculate eg : --length highway waterway , Unit is
+                        in Meters
   --force               Force for the Hashtag Replication fetch if it is greater than a day interval
   --rows ROWS           No. of top rows to extract , to extract top 100 , pass 100
-  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware to use this max no of workers may cause overuse of resources
-  --url URL             Your public OSM Change Replication URL
+  --workers WORKERS     No. of Parallel workers to assign : Default is no of cpu available , Be aware
+                        to use this max no of workers may cause overuse of resources
+  --url URL [URL ...]   Your public list of OSM Change Replication URL , 'minute,hour,day' option by
+                        default will translate to planet replciation url. You can supply multiple
+                        urls for geofabrik country updates , Url should not have trailing / at the
+                        end
   --last_week           Extract stats for last week
   --last_day            Extract Stats for last day
   --last_month          Extract Stats for last Month
   --last_year           Extract stats for last year
   --last_hour           Extract stats for Last hour
+  --days DAYS           N nof of last days to extract , for eg if 3 is supplied script will generate
+                        stats for last 3 days
   --charts              Exports Summary Charts along with stats
   --summary             Produces Summary.md file with summary of Run
-  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this hashtag search will search for the existence of text on hashtags and
-                        comments
-  --changeset           Include hashtag and country informations on the stats. It forces script to process changeset replciation , Careful to use this since changeset
+  --exact_lookup        Exact lookup for hashtags to match exact hashtag supllied , without this
+                        hashtag search will search for the existence of text on hashtags and comments
+  --changeset           Include hashtag and country informations on the stats. It forces script to
+                        process changeset replciation , Careful to use this since changeset
                         replication is minutely
   --all_tags            Extract statistics of all of the unique tags and its count
+  --temp                Deletes downloaded osm files from machine after processing is done , if you
+                        want to run osmsg on same files again keep this option turn off
   --exclude_date_in_name
-                        By default from and to date will be added to filename , You can skip this behaviour with this option
+                        By default from and to date will be added to filename , You can skip this
+                        behaviour with this option
   --format {csv,json,excel,image,text} [{csv,json,excel,image,text} ...]
                         Stats output format
   --read_from_metadata READ_FROM_METADATA
-                        Location of metadata to pick start date from previous run's end_date , Generally used if you want to run bot on regular interval using
-                        cron/service
+                        Location of metadata to pick start date from previous run's end_date ,
+                        Generally used if you want to run bot on regular interval using cron/service
 ```
 
 It is a Simple python script processes osm files live and produces stats on the fly
 
 1. It can Generate Stats on Country Level for countries . Countries are available in [here](./data/countries_un.csv)
 2. It can also take any other server replication changefile to extract stats (Tested with Geofabrik and Planet Replication)
 3. Can Generate hashtag statistics
@@ -95,14 +106,16 @@
 ```
 {"name":"username","uid":uid,"changesets":1,"nodes.create":1071,"nodes.modify":2100,"nodes.delete":0,"ways.create":146,"ways.modify":69,"ways.delete":0,"relations.create":0,"relations.modify":1,"relations.delete":0,"building.create":138,"building.modify":11,"building.delete":0,"highway.create":5,"highway.modify":49,"highway.delete":0,"waterway.create":0,"waterway.modify":4,"waterway.delete":0,"amenity.create":0,"amenity.modify":3,"amenity.delete":0,"landuse.create":3,"landuse.modify":1,"landuse.delete":0,"natural.create":0,"natural.modify":3,"natural.delete":0,"total_map_changes":3387}
 ```
 
 ### Start Right Away :
 
 - Extract Stat of last hour and visualize stats/charts
+  
+  By default replication is minute url.
 
 ```
 osmsg --last_hour --charts --changeset
 ```
 
 ### More Example Commands
 
@@ -111,17 +124,18 @@
 ```
 osmsg --url "https://planet.openstreetmap.org/replication/minute" --format csv --tags building highway waterway amenity --name stats --all_tags --last_hour
 ```
 
 In order to extract for specific country just add --country with country name as in [data/countries_un.csv](./data/countries_un.csv) for eg : For Nepal : `--country Nepal`
 
 - To extract stats for last day whole world with all the tags and specified stat :
-
+  
+  You can either pass url "https://planet.openstreetmap.org/replication/day" itself or if you want to use planet default replciation url you can simply pass as : minute , day & hour , script will get url itself  
 ```
-osmsg  --url "https://planet.openstreetmap.org/replication/day" --format csv --last_day --name stats --all_tags
+osmsg  --url day --format csv --last_day --name stats --all_tags
 ```
 
 If you wish to have tags with specific count for key you can include them as `--tags "building" "highway" ` & add --country to extract specific country , if you use geofabrik country updates you don't need to use --country option
 
 - To extract specific country with Geofabrik URL (extracts stats for 15 days custom date range)
 
 ```
@@ -135,27 +149,31 @@
 
   Processing geofabrik country based osm change files are faster as they will have changes only for country and smaller in size
 
 ```
 osmsg --start_date "2022-01-01 00:00:00+00:00" --url "http://download.geofabrik.de/asia/nepal-updates" --username 'your osm username' --password 'user osm password' --tags 'building' 'highway' 'waterway' 'amenity'  --format csv
 ```
 
+- Example of extract last 8 days of data for Turkey and Syria for hashtag smforst using geofabrik
+```
+osmsg --url http://download.geofabrik.de/europe/turkey-updates https://download.geofabrik.de/asia/syria-updates --username "OSM USERNAME" --password "OSM PASSWORD" --hashtags smforst --length highway --force --days 8 --tags building highway --all_tags
+```
 Check more commands examples inside `stats/` `stats_metadata.json`
 
 Now start generating stats with above sample commands
 
 ### TIPS & Tricks of using OSMSG:
 
 OSMSG uses/supports sources , --url provided on argument will be used for osm changefiles and for changeset it is default of planet replication/minute ( used for hashtag and country )
 
 1. To process weekly / monthly or yearly stats , Using minute replication might take forever on small machines , You can use daily replication files `/replication/day` to process faster and avoid network download issues for small minute fiels
 
 2. If you are generating stats for rightnow / past 10min / past 1 hour using specific timeframe , stick with minutely (Sometimes to reflect changes you made on stats , Planet may take few minutes)
 
-3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible
+3. For hashtag stats , planet changeset minute replication is by default for now (Found only this reliable source , couldn't find daily/monthly replication files) , Generating daily/weekly is only feasible , To generate more than that you can supply multiple countries geofabrik urls so that script can go through only country changefiles as stated on example above for turkey and syria , similarly you can pass your countries url and generate monthly yearly etc 
 
 4. For Country stats , if you use the --country option : It will use the planet minutely changeset replication to determine the location of the cahngeset bbox centroid , which means to process larger time frame it might take time , to avoid this Use Geofabrik internal changefiles based on country , OSMSG Supports processing of those hence you can directly supply geofabrik changefiles url for country and produce yearly/monthly stats eg :
 
 ```
 osmsg --url "http://download.geofabrik.de/asia/nepal-updates" --username '${{ secrets.OSM_USERNAME }}' --password '${{ secrets.OSM_PASSWORD }}' --format csv --last_month --tags 'building' 'highway' 'waterway' 'amenity' --name last_month_stats  --all_tags
 ```
```

### Comparing `osmsg-0.1.8/setup.py` & `osmsg-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Read the content of the README file
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 
 setup(
     name="osmsg",
-    version="0.1.8",
+    version="0.1.9",
     description="OpenStreetMap Stats Generator : Commandline",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kshitijrajsharma/OSMSG",
     author="Kshitij Raj Sharma",
     author_email="skshitizraj@gmail.com",
     license="MIT",
```

