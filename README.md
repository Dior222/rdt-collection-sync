# rdt-collection-sync
syncronyze solr collection create when in start rdt module in multi-process
we use solr in out project and we have a module called rdt, which is to put messages consumed from kafka to SolrCloud.
We have a timer task to create the collection for the next day at mid-night. When start the module in multi-process, each
will create the same collection. So I made this project to simulate this situation in order to sync the creation.
