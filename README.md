# BLOCKTRACTOR is a fully-decentralised smart-contract service marketplace built on the Ethereum Blockchain.

## 1. Contracts

### Blocktractor.sol

Blocktractor is a Marketplace smart contract that interacts with Service and Profile Smart Contracts.

Functions

- createService(title,description,price)
  - Service Provider can create a service
    returns index number of Service created
- deleteService(serviceNumber)
  - Service Provider can delete a service
- listService(serviceNumber)
  - Service Provider can list their service
- delistService(serviceNumber)
  - Service Provider can delist their service
- viewMyServices()
  - Getter Function for services provided by service provider
- requestService()
  - Service Requester can request a service
- approveService()
  - Service Provider can approve requested service
- rejectService()
  - Service Provider can reject requested service
- completeService()
  - Service Provider can complete rendered service
- statusService()
  - Getter Function for status of Service
- registerProfle()
  - Registering a profile on Blocktractor
- removeProfile()
  - Removing a profile on Blocktractor

### Service.sol

Service smart contract interacts only with the Blocktractor smart contractor.

### Profile.sol

Profile smart contract interacts only with the Blocktractor smart contractor.
Each profile can be both a service provider and a service requester.

Functions

- createProfile(name,username,password)

  - Creation of Profile

- getName()
  - Returns name of Profile

## 2. Migrations

## 3. Test

To compile and test Blocktractor smart contracts, run the following codes.

```bash
npm install
truffle compile
truffle migrate
truffle test
```
