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