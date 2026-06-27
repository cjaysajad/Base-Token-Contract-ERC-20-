# Base Token Contract (ERC-20)
```bash
npm install @openzeppelin/contracts
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0
import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
contract BaseToken is ERC20 {
    constructor() ERC20("BaseToken", "BT") {
        _mint(msg.sender, 1000000 * 10 ** decimals());
    }
}
