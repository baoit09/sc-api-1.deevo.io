# supply-chain-service
Food supply chain RESTful API Service (NodeJS) is designed and implemented with Domain-Driven Design (DDD).
Designed to connect to Hyperledger's first network (docker-compose-e2e-cli.yaml).

# Remember on Channel.js file, change:
let use_admin_signer = true;
if (request.txId) {
  use_admin_signer = request.txId.isAdmin();
}

# To start app:
1. clone this repo from github
2. cd to supply-chain-service
3. run: npm install
4. run: utils/get-remote-config.sh with appropriate parameters
5. run: node utils/enrollAdmin.js
6. run: npm start

  If it shows up: [API Server is running at http://localhost:3001/] means that api server is started up successfuly.
