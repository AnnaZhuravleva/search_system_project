================================================================================
search_system
================================================================================

Description
--------------------------------------------------------------------------------

Project of a search system based on Elastic search

- This search system can find 20 most relevant documents from the 
  database posts.csv, located in the project folder, based on the 
  request
- Database consists of posts.csv file (database of documents)and 
  Index located in the Cloud Elasticsearch database
  (https://www.elastic.co/cloud/, 
  'https://9a669b1781184222b80810649034afc6.eastus2.azure.elastic-cloud.com:9243')
- Web-app page is based on Flask and is located on http://127.0.0.1:5000/ localhost
- Logs of errors are stored in logs.log

Installation
--------------------------------------------------------------------------------
python3 setup.py install --user

```
>>> import search_system
>>> search_system.start()
```
