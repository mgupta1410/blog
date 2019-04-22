## Apache Solr Quick Install

April 22, 2019

The instructions on the Apache Solr website are not very clear, and the download links are broken. This tutorial might be helpful. 

_(Tested for Solr 8.0.0)_

- Get the desired version from [Apache Solr Archives](https://archive.apache.org/dist/lucene/solr/) and extract.
```
wget https://archive.apache.org/dist/lucene/solr/8.0.0/solr-8.0.0.tgz
tar -zxvf solr-8.0.0.tgz
```

_Note that solr-x.x.x-src.tgz contains the source files, and needs to be compiled, for pre-compiled binaries make sure to download solr-x.x.x.tgz._

- Provide appropriate permissions 
```
chmod -R 755 solr-8.0.0
```

- Start the server 
```
cd solr-8.0.0 
./bin/solr start -e cloud
```

Expected Output
```
Welcome to the SolrCloud example!

This interactive session will help you launch a SolrCloud cluster on your local workstation.
To begin, how many Solr nodes would you like to run in your local cluster? (specify 1-4 nodes)
```

- You are good to go! Follow further instructions from the [Solr website](https://lucene.apache.org/solr/guide/7_0/solr-tutorial.html#exercise-1)
- Enjoy searching! 
