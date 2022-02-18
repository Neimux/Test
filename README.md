const MongoClient = require('mongodb').MongoClient;
const url = 'mongodb://et02104%40zgie.ztech:QSDqsdqsd1221!@mongodb-201.dbaas-mongodb.iaas.cagip.group.gca:27017,mongodb-202.dbaas-mongodb.iaas.cagip.group.gca:27017,mongodb-203.dbaas-mongodb.iaas.cagip.group.gca:27017,mongodb-204.dbaas-mongodb.iaas.cagip.group.gca:27017'
const dbName = 'scripta-cagip-ctdbbackend-dev'

MongoClient.connect(url, function(err, client) {
    console.log("Connecté à MongoDB");
    const db = client.db(dbName);
    client.close();
  });
