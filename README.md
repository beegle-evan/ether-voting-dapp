# ether-voting-dapp

# install ganache ( http://truffleframework.com/ganache/ )


#chapter1
npm install ganache-cli web3@0.20.3 solc
node_modules/.bin/ganache-cli

실행 결과

Available Accounts
==================
(0) 0x217015063116B92008ea3D2190260F92e10d49c4 (100 ETH)
(1) 0xAC834be9D0d6972ADd4436170Dab9f86ad469e7C (100 ETH)
(2) 0x6800b3402452071fa0D9abE7224dceE220089179 (100 ETH)
(3) 0x31D685dAd7fACc1b2AC56c1031E625463b3De680 (100 ETH)
(4) 0xcfD6Dd3999faa0A1779416FFfb973FDd6E36b1df (100 ETH)
(5) 0x04087B087273461429507Bd54C31Fa3BF21A61f8 (100 ETH)
(6) 0x4693cEA265881EFF9C55B5D5aD82f3f5D3d91F07 (100 ETH)
(7) 0xEdb84671DaDBB4A92Dd0c5c272126e1d687f47Dc (100 ETH)
(8) 0x62d5B7859081f5C3e58fAa77b8a8b34e57a5D5Ee (100 ETH)
(9) 0xF8cB53906c04410BdfCbE4d82513Ee5fC701e284 (100 ETH)

Private Keys
==================
(0) 0xec496fa09a72898e89ec92ea2be1094f47997e50ef71232c90e4a4fe17ee741f
(1) 0xbb87d39fde646972f872b9bdfe02be22bb5d7b52a7dc4358dbadca34b676c376
(2) 0xfe67a6896f0e805e2a580aea13c7f25bacd6c4e5a9aae79e574e899e406725ed
(3) 0x2ecc8fadd1102eab1e90f8e31541fd216b738e7879e51f9ecdfdd598fd7ffce6
(4) 0xac280b9446f78ab1f69540483bb1498207364c37924f4b24f7c5be269f2c14e2
(5) 0x416d7bac2fb9459260a85fc9f5e33aaa08fd2bed0f6df3f6b5bf32f5fda051ab
(6) 0x1b5b736da0f4a37634ceb716318a89034e7bf812eb04bf3fcb0b37e62bd1a440
(7) 0xe2fe46c41a6c3fd0bebc12af6887312a94bdb0b134e534e18ae25d8c1997d2fd
(8) 0x66fca102e09764d94006f2b0ec089d7b80d380ea4410f18eed4883d65a4992d9
(9) 0x97b4bbd4e4ada158e77f5256f40f352ff715aa0048169e79bf024ab791f8f025

HD Wallet
==================
Mnemonic:      advice injury demise menu luggage auction whisper summer actual endorse stage crash
Base HD Path:  m/44'/60'/0'/0/{account_index}

Gas Price
==================
20000000000

Gas Limit
==================
6721975

Call Gas Limit
==================
9007199254740991

Listening on 127.0.0.1:8545


# 다른 tab에서 node 실행 후, 
Web3 = require('web3')
web3 = new Web3(new Web3.providers.HttpProvider("http://localhost:8545"))

> web3.eth.accounts
[ '0x217015063116b92008ea3d2190260f92e10d49c4',
  '0xac834be9d0d6972add4436170dab9f86ad469e7c',
  '0x6800b3402452071fa0d9abe7224dcee220089179',
  '0x31d685dad7facc1b2ac56c1031e625463b3de680',
  '0xcfd6dd3999faa0a1779416fffb973fdd6e36b1df',
  '0x04087b087273461429507bd54c31fa3bf21a61f8',
  '0x4693cea265881eff9c55b5d5ad82f3f5d3d91f07',
  '0xedb84671dadbb4a92dd0c5c272126e1d687f47dc',
  '0x62d5b7859081f5c3e58faa77b8a8b34e57a5d5ee',
  '0xf8cb53906c04410bdfcbe4d82513ee5fc701e284' ]
> web3.eth.getBalance('0x217015063116b92008ea3d2190260f92e10d49c4')
BigNumber { s: 1, e: 20, c: [ 1000000 ] }
>
> web3.eth.getBalance('0x217015063116b92008ea3d2190260f92e10d49c4').toNumber()
100000000000000000000
> web3.fromWei('100000000000000000000', 'ether')
'100'


remix.ethereum.org
