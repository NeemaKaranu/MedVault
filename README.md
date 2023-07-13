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

Server directory:
## IPFS Configuration
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


## Contributing 

We appreciate and encourage contributions! Please refer to our [Contributing Guide](CONTRIBUTING.md) for more information.

## License

MedVault is licensed under the terms of the MIT license. For complete details,
