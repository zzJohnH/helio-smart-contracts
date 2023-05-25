# 本地测试步骤

* 在 `http://nodereal.io`申请账号，拿到BSC RPC API key
* 本地单独运行区块链，命令: `npx hardhat node --fork ${BSC RPC API key}`
* 部署合约，运行`npx hardhat test test/e2e/e2e.test.js --network localhost`
* 部署成功后，可以把部署代码注释掉，写自己的测试用例，PS：只要步骤2不关掉，一次部署可以永远使用