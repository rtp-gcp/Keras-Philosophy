
# Notes



## Hi-lites on orig repo

Some of this came from a hackathon repo I did previously.

| code                 | Notes                                                                                             |
| -------------------- | ------------------------------------------------------------------------------------------------- |
| src/ML-try-007.ipynb | Was the final submission code                                                                     |
|                      | Sets up the notebook to use tensorboard.                                                          |
|                      | I doubt tensorboard works in watsonx - remove it                                                  |
|                      | Uses ./csv/usgs_gsvb_v2.csv for data                                                              |
|                      | The input has 9K rows and 8 columns                                                               |
|                      | Should break this up into a single file to generate the clean data including a yaml data contract |
|                      | adds new columns, normalizes the data                                                             |
|                      | -- cut off for cleaning data --                                                                   |
|                      |  The rest of the code has:                                                                        |
|                      |     * Defining model                                                                              |
|                      |     * training model                                                                              |
|                      |     * testing model                                                                               |
| csv/usgs_gsvb_v2     | Initial set of *raw* data                                                                         |
|                      | Originally this data came from two sources USGS and Greenstream sensor data                       |
|                      | This dataset has been massaged and combined previously to make the current file.                  |



