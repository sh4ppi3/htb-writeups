# Recon

![[Pasted image 20260805010412.png]]
# Foothold

Please note that the MongoDB server running on Mongod is only compatible with Mongo Shell version <= 2.3.2

` curl -O https://downloads.mongodb.com/compass/mongosh-2.3.2-linux-x64.tgz

![[Pasted image 20260805010803.png]]

To see all databases inside mongodb

`show dbs;
![[Pasted image 20260805011114.png]]

Lets see whats inside sensitive_information, to do it, lets select it first.
`use sensitive_information

![[Pasted image 20260805011329.png]]

An list it content

`show collections;

![[Pasted image 20260805011352.png]]
# Flag
Found the flag!

To get it, we need to use the `db.collection.find()` command. Substitute `collection` with the target collection name:

`db.flag.find();

![[Pasted image 20260805011412.png]]
