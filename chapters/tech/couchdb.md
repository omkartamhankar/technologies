## CouchDB :smiley: :exclamation: fa18-423-03



|          |             |
| -------- | ----------- |
| title    | CouchDB     | 
| status   | 10          |
| section  | NoSQL       |
| keywords | NoSQL       |


### Old

The Apache Software Foundation makes CouchDB [@www-couchdb.apache] available as an option
for those seeking an open-source, NoSQL, document-oriented
database. CouchDB, or cluster of unreliable commodity hardware
database, stores data as a JSON-formatted document
[@www-exploringcdb-couchdb].  Documents can consist of a variety
of field types, e.g., text, booleans or lists, as well as metadata
used by the software. CouchDB does not limit the number of fields per
document, and it does not require any two documents to consist of
matching or even similar fields
[@www-techoverview-couchdb]. That is, the document has
structure, but the structure can vary by document.  CouchDB
coordinates cluster activities using the master-master mode by
default, which means it does not have any one in charge of the
cluster.  However, a cluster can be set up to write all data to single
node, which is then replicated across the cluster.  Either way, the
system can only offer eventual consistency. CouchDB serves as the
basis of Couchbase, Inc's Couchbase Server
[@www-cdb-vs-cbs-couchdb].


### New

Berkeley DB [@www-couchdb.apache] is an open source data management library. Because it is open
source, anyone can use it for free. It has a few features that make it highly
versatile for developers. First, the database library is scalable. Berkeley DB's
initial library is

> "under 300 kilobytes of text space on common architecture, but it can manage
> databases up to 256 terabytes in size" [fa18-423-03-berkeleydb-intro].

Second, it exhibits an application programming interface that allows the user to
enter a simple call function to operate the database libraries and management
services. Berkeley DB supports C, C++, Java, Tcl, PHP, Python, and Perl.
Furthermore, developers can embed Berkeley DB directly into their program and
with the API, data store, concurrent, transactional, and replication
configuration options all run on the back end.

Berkeley was originally released in 1996. It was developed by Margo Seltzer and
Keith Bostin of Sleepycat Software and sold to Oracle Corporation in 2006. Since
the database management library software's inceptions it has went through many
advances and iterations. When first released, Berkeley DB was designed only to
handle large data, greater than the size of the hash buckets being used, and to
provide

> "constant time mapping being has values and page addresses"
> [fa18-423-03-berkeleydb-design].

One of the most complex developments was introducing a recovery manager in
Berkeley DB 2.0.6. Berkeley DB also offers Btree, Queue, Recno, and Hash access
methods. As mentioned previously, there is a library interface because the
developers realized that the service required front end functionality for both
the applications and the internal code. Furthermore, the developers introduced
managers for each of the configuration options that required all their own
architectures.

