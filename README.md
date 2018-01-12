# blockchain-asset-management
Asset Management on the Factom Public Blockchain

# Factom commands
curl -X POST --data-binary '{"jsonrpc": "2.0", "id": 0, "method": "heights"}' -H 'content-type:text/plain;' http://courtesy-node.factom.com:80/v2

curl -X POST --data-binary '{"jsonrpc": "2.0", "id": 0, "method":"pending-entries", "params": {}}' -H 'content-type:text/plain;' http://courtesy-node.factom.com:80/v2

curl -X POST --data-binary '{"jsonrpc": "2.0", "id": 0, "method":"entry","params":{"hash":"bafeb4aa48717d968a3e3e89091c245070f9c7e6a9301d4e71aea56b39c842a7"}}' -H 'content-type:text/plain;' http://courtesy-node.factom.com:80/v2

curl -X POST --data-binary '{ "jsonrpc": "2.0", "id": 0, "method": "compose-entry", "params": { "entry": {"chainid":"48e0c94d00bf14d89ab10044075a370e1f55bcb28b2ff16206d865e192827645",  "extids":["cd90", "90cd"], "content":"abcdef"}, "ecpub":"EC2DKSYyRcNWf7RS963VFYgMExo1824HVeCfQ9PGPmNzwrcmgm2r"}}' -H 'content-type:text/plain;' http://courtesy-node.factom.com:80/v2



// create EC address
./factom-cli newecaddress entrycredits1
EC34a6u7R8LE4YVq2anvoswBBZmDEWBUCBsfHFK9vfiQJcz352CP

// to start composing a new tx
$ ./factom-cli newtx <tx_name>

