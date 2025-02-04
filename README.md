# Installation
```shell
git clone
```

- Créer un .env :

PRIVATE_KEY=

POLYGONSCAN_API_KEY=

```shell
npm install
```

# Token publiés et déployés: 
MyToken : https://mumbai.polygonscan.com/address/0x908C79d78544ffF5ba4AD828A5E518030b006141#code
MyCrowdsale : https://mumbai.polygonscan.com/address/0x968dc34f72E546082eaBaE102e7B6E49911A2119#code


# Tester les tokens :
```shell
npx hardhat test
```

# Déployer les tokens :
```shell
npx hardhat run scripts/deploy.js --network mumbai
```

# Adresses :
MyToken address : 0x57EBA3AFbfCFE7877F7057158855B30BDC3cc8E9

MyCrowdsale address : 0x37234e8f29A509c9EaB8Db305CB8778D8274610e

# Vérifier le code source :
```shell
npx hardhat verify --network mumbai 0x57EBA3AFbfCFE7877F7057158855B30BDC3cc8E9
npx hardhat verify --constructor-args arguments/arguments.js --network mumbai 0x968dc34f72E546082eaBaE102e7B6E49911A2119
```

# Deployer et vérifier un token en même temps :
```shell
npx hardhat deploy-and-verify --network mumbai --contractname MyToken
npx hardhat deploy-and-verify --network mumbai --contractname MyCrowdsale
```
