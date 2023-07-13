# MedVault: Blockchain EHR Project

## Project Description

Welcome to MedVault, a paradigm shift in managing Electronic Health Records (EHRs). This pioneering project leverages blockchain technology to deliver an enhanced level of security, transparency, and interoperability for EHRs.

MedVault utilizes Ganache from the Truffle Suite, Metamask, Django, and Angular. Ganache, our Ethereum blockchain emulator, provides the ideal environment to develop and test our smart contracts, enabling a secure exchange and storage of health records. Metamask is integrated into MedVault to allow users to interact with our decentralized application (dApp) seamlessly, offering secure transactions within the Ethereum network.

The backend operations are run by Django, a powerful, secure Python-based web framework. Django facilitates user management and provides interfaces for standard CRUD operations on the EHRs.

Angular, a robust JavaScript framework, powers our frontend, providing an intuitive user interface. With its modular architecture, Angular offers smooth integration with Django and Metamask, creating a responsive and engaging user experience.

## Setup and Installation

For instructions on how to set up and install MedVault, please follow the steps provided in the here:
Packa## Packages Needed:

- Node JS : [Download here](https://nodejs.org/en/download/)
- Python: [Download here](https://www.python.org/downloads/)
- IPFS : [Download here](https://dist.ipfs.io/#go-ipfs)
- Angular: Install using npm
    ```
    npm install -g @angular/cli
    ```
- Truffle: Install using npm
    ```
    npm install -g truffle
    ```
    If the above fails, run:
    ```
    npm install -g truffle@5.4.29
    ```
    Note: Ubuntu permissions may vary depending on the method of npm install.

Download and install git if not already installed.

- Git: [Download here](https://git-scm.com/downloads)

Open Terminal in Server Directory 

**Commands may differ for Linux and MacOS**

Open GANACHE and import the project.

Start Terminal in the Client Directory
NB: Setup Metamask before opening the project.

Open: http://localhost:4200/ on Client Side

## Clearing the Server and Client

This is in the case of a fresh redo of the steps of the project.
CLient:
```
npm i --force
truffle migrate
npm start
```

Server directory:
```
python -m pip install virtualenv
python -m virtualenv venv
       Windows: venv/scripts/activate
      macOs / Linux : source venv/bin/activate
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
## IPFS Configuration
Configure the below after running the IPFS file
```
ipfs init
ipfs daemon
``` 
This is in the IOFS Settings
```
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
```
## Repeat Build
For starting project 2nd time:
Run Ganache
Ensure Metamask is Using the right network
Client:
```
 npm start
 ```

Server:
```
 venv/Scripts/activate
python manage.py runserver
```

IPFS: 

```
ipfs daemo
```
## Contributing 

We appreciate and encourage contributions! Please send an email for more inquiry to sharon.kangethe@strathmore.edu or neema.karanu@strathmore.edu.

## License

MedVault is licensed under no license for the time being.
