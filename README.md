# PerfMonCollectorAPI
Python/Flask service deployed in AWS to receive zipped PerfMon log files, store in an S3 bucket, and provide tools for retrieval

## Tasks
* Standup python/flask service
* Basic auth on requests
* Route for submission
  * Respond in < 1 sec
  * Verify it's a log file
  * Store in s3 bucket
  * Respond 'good' or 'bad'
* Route for retrieving files
  * Navigate s3 bucket
  * Pull from s3 bucket and send FLO (file like object) when file is specified
