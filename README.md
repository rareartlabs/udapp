### development

```
git clone git@github.com:kumavis/udapp.git
cd udapp
git checkout -b wip
npm install
npm start
# do hackz, commit code
git push origin wip
```

### running the dapp

The app runs the example dapp token.json by default. To run a different Dapp you built with Truffle

- run `truffle compile` and `truffle deploy` to deploy the dapp to the network of your choice
- find the JSON output for the contract you want at `build/contracts/<your-contract>.json`
- duplicate that file into the `/tokens` directory
- update the `truffleJSON` variable to that file name
- make sure Metamask is pointed to the network on which you deployed

`npm run start` should now give you an interface to your dapp
