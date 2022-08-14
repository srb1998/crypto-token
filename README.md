# crypto-token
//Made Contract on Remix-IDE for creating Cryptocurrency Token under 10 lines of code

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.5;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";

contract Ghostcoin is ERC20 {
    
    constructor(string memory _name,string memory _symbol)

    ERC20(_name,_symbol)
    
    {
        _mint(msg.sender,100 * (10**18));
    }

}
