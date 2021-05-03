03-29-2021
- Updated broken links to STAC API spec pages and HLS V1.5 User Guide   

03-25-2021
- Added `conda install jupyter notebook --yes` as an instruction to the README and tutorial (issue with `holoviews`/`geoviews` plots not rendering)   
- Added a check during automation (section 6) that will skip a file that has already been processed and is available in the current directory  
- Updated the way that the crs is passed to `hvplot()`    
- Added `from subprocess import Popen, DEVNULL, STDOUT` to address issue when `_netrc` is not found  
- Added optional ` #gdal.SetConfigOption("GDAL_HTTP_UNSAFESSL", "YES")` call for users that need it  
- Updated time series with more observations from March 2021  

03-22-2021
- Removed GDAL config option to turn SSL off (not needed)   
- Added `.sortby()` function to the `xarray` data array to assure L30 and S30 observations are ordered chronologically   
- Changed the time period of interest to 09-01-2020 to 03-31-2021    
- Updated the section on generating a `.netrc` or `_netrc` file based on user platform

03-15-2021
- Updated `collections` to product `shortnames` (in place of `concept_id`) to align with latest release of CMR-STAC.   
- Updated logic for search responses with no data found (now returns valid response with `numberReturned` = 0).   
- Changed all queries to CMR-STAC LPCLOUD Search endpoint from **GET** requests to **POST** requests.    
- Combined `collections` call to LP CLOUD Search endpoint into a single POST request with a list of both HLS products.  
- Updated README with link to CHANGELOG.md  

02-12-2021
- Replaced `bounding_box` with `bbox` and `concept_id` with `collections` to fix breaking change in CMR-STAC search parameter spec and added CHANGELOG.md to repo  

01-26-2021  
- Added Support for HLSL30 V1.5  
- Updated the HLS Script

12-15-2020
- Pull request #5: Added functionality to handle files that are unable to be downloaded
- Fixed COG overviews issue and added filtering for empty observations
- Added functionality to handle files that are unable to be downloaded

11-20-2020
- Pull request #4: Corrected flipped description of bounding box coordinates
- Corrected flipped description of bounding box coordinates

11-19-2020
- Pull request #3: Updated tutorial and readme to reflect cmr-stac updates and peer review suggestions
- Updated tutorial and readme to reflect cmr-stac updates and peer review suggestions

11-17-2020
- Merge pull request #2 in LPDUR/hls-tutorial from develop to master
- Updated code to reflect new STAC endpoint and peer review revisions

10-28-2020
- Merge pull request #1 in LPDUR/hls-tutorial from develop to master
- Updated tutorial and README from AF review
- Updated tutorial and README from AF review

10-27-2020
- updated tutorial and readme from MJ review

10-08-2020
- Added additional guidance on setting up netrc file
- Updated tutorial, README, and added html output and requirements file

09-29-2020
- Initial Commit
