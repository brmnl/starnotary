# Goerli Deployment Log

```
truffle(develop)> compile

Compiling your contracts...
===========================
> Compiling ./app/node_modules/@openzeppelin/contracts/token/ERC721/ERC721.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/token/ERC721/IERC721.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/token/ERC721/IERC721Receiver.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/token/ERC721/extensions/IERC721Metadata.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/Address.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/Context.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/Strings.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/introspection/ERC165.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/introspection/IERC165.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/math/Math.sol
> Compiling ./app/node_modules/@openzeppelin/contracts/utils/math/SignedMath.sol
> Compiling ./contracts/Migrations.sol
> Compiling ./contracts/StartNotary.sol
> Artifacts written to /Users/manuel/git/starnotary/build/contracts
> Compiled successfully using:
   - solc: 0.8.12+commit.f00d7308.Emscripten.clang
truffle(develop)> test
Using network 'develop'.


Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.


  ✔ can Create a Star (80ms)
  ✔ lets user1 put up their star for sale (98ms)
  ✔ lets user1 get the funds after the sale (205ms)
  ✔ lets user2 buy a star, if it is put up for sale (184ms)
  ✔ lets user2 buy a star and decreases its balance in ether (176ms)
  ✔ can add the star name and star symbol properly (86ms)
  ✔ lets 2 users exchange stars (175ms)
  ✔ lets a user transfer a star (121ms)
  ✔ lookUptokenIdToStarInfo test (67ms)

  9 passing (1s)

truffle(develop)> migrate --reset --network goerli

Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.


Migrations dry-run (simulation)
===============================
> Network name:    'goerli-fork'
> Network id:      5
> Block gas limit: 30000000 (0x1c9c380)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > block number:        9625200
   > block timestamp:     1693676668
   > account:             0x80CB4FebdA6d1003549b6B6c2d298aa5C9f6e832
   > balance:             0.045878584572675355
   > gas used:            250200 (0x3d158)
   > gas price:           1 gwei
   > value sent:          0 ETH
   > total cost:          0.0002502 ETH

   -------------------------------------
   > Total cost:           0.0002502 ETH


2_deploy_contracts.js
=====================

   Deploying 'StarNotary'
   ----------------------
   > block number:        9625202
   > block timestamp:     1693676671
   > account:             0x80CB4FebdA6d1003549b6B6c2d298aa5C9f6e832
   > balance:             0.042949698572675355
   > gas used:            2882973 (0x2bfd9d)
   > gas price:           1 gwei
   > value sent:          0 ETH
   > total cost:          0.002882973 ETH

   -------------------------------------
   > Total cost:         0.002882973 ETH

Summary
=======
> Total deployments:   2
> Final cost:          0.003133173 ETH




Starting migrations...
======================
> Network name:    'goerli'
> Network id:      5
> Block gas limit: 30000000 (0x1c9c380)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xa476ad79c5eb1e9843effb987d4385a3a774a489ee2a3471b133e75432691995
   > Blocks: 1            Seconds: 12
   > contract address:    0xc8d77F0FdE610d9e7FF46C5ECca4AE157F8a6549
   > block number:        9625206
   > block timestamp:     1693676688
   > account:             0x80CB4FebdA6d1003549b6B6c2d298aa5C9f6e832
   > balance:             0.045878584572675355
   > gas used:            250200 (0x3d158)
   > gas price:           1 gwei
   > value sent:          0 ETH
   > total cost:          0.0002502 ETH

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0002502 ETH


2_deploy_contracts.js
=====================

   Deploying 'StarNotary'
   ----------------------
   > transaction hash:    0xd96983b7fd07ac2e6a9d073ef816f86b44a4f6e5b3438c9bf87ac5646d63d3fa
   > Blocks: 0            Seconds: 4
   > contract address:    0xa2A1824D259b0E8afDA1f64a33B30dE127a07662
   > block number:        9625208
   > block timestamp:     1693676712
   > account:             0x80CB4FebdA6d1003549b6B6c2d298aa5C9f6e832
   > balance:             0.042949698572675355
   > gas used:            2882973 (0x2bfd9d)
   > gas price:           1 gwei
   > value sent:          0 ETH
   > total cost:          0.002882973 ETH

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:         0.002882973 ETH

Summary
=======
> Total deployments:   4
> Final cost:          0.006266346 ETH


truffle(develop)>
```