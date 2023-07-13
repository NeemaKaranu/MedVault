Project Summary:
To address the concerns highlighted in this chapter we aim to implement the system with the use of Etheruem and Soidity as well as Ganache. 
Hyperledger Fabric, as a permissioned blockchain framework, ensures privacy, data control, and fine-grained access control required in healthcare settings. 
Since all the transactions are combined in a block and arranged in a chain as explained in the first diagram above. 
On top of the blockchain, Hyperledger fabric provides some additional features which perfectly fit the current scenario. 
By being permissioned and closed blockchain, no person can get added into the network unlike permissionless blockchains such as Bitcoin, Ethereum. 
This solves the confidentiality problem of patients’ data. 
 
2.4: Block Diagram 
 
 
The fabric has a concept of Certificate Authority for every organization or common CA called Fabric CA and MSP which provides identities and verifies when a transaction request is made. 
Moreover, all the components of the fabric network are scalable and pluggable. 
It enables the creation of a decentralized network where authorized participants can securely access and update patient records, ensuring data integrity and immutability. 
Patient will be able to fully view their history at the touch of a button and have control of the professionals that would access their records. 
The patient needs to create an account only the first time the patient visits any one of the hospitals in the network, during the first visit the patient provides details to the admin, admin invokes the AdminContract to create a patient. 
In the backend, firstly the admin certificate is used to connect to the network, and a transaction is created which adds the patient object to the ledger and adds the patient identity to the blockchain network.  
After the creation of the patient is successful, the server creates a temporary password for the patient using which the patient can log in to the network. 
The patient credentials are added to the ledger as the patient can go to any of the hospitals in the network. The doctor provides details to the admin, who then firstly connects to the network and then adds the doctor as an identity to the blockchain network. And the credentials of the doctor are stored in the hospitalspecific database. Now as patient and doctor are added as identities in the blockchain network, for the next interaction the patient/doctor can connect to the network using their certificates. 



Packages Needed:

Node JS : https://nodejs.org/en/download/ 
Python: https://www.python.org/downloads/
IPFS : https://dist.ipfs.tech/#go-ipfs 
angular: npm install -g @angular/cli
truffle: npm install -g truffle      \
if failed run :  npm install -g truffle@5.4.29
*Ubuntu permissions may vary depending on ,ethod of npm install

download and install git if not installed.
git: https://git-scm.com/downloads


open Terminal in Server Directory 

```
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py run server

*Commands may differ for Linux and MacOS**
open GANACHE and import project

 
````
Start Terminal in the Client Directory

npm install --force
truffle migrate
npm start

```

NB: Setup metamask before opening the project

open: http://localhost:4200/ on CLient Side

**** CLEARING THE SERVER  AND CLIENT ***

This is in the case of a fresh Redo of the steps of the project

Server dir:python manage.py flush
CLient :truffle migrate





```

IPFS Configuration

"Access-Control-Allow-Headers": [
      "X-Requested-With",
      "Access-Control-Expose-Headers",
      "Range"
   ],
   "Access-Control-Expose-Headers": [
      "Location",
      "Ipfs-Hash"
   ],
   "Access-Control-Allow-Methods": [
      "POST",
      "GET"
   ],
   "Access-Control-Allow-Origin": [
      "*"
   ],
   "X-Special-Header": [
      "Access-Control-Expose-Headers: Ipfs-Hash"
   ]