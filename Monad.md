// SPDX-License-Identifier: MIT

// Make sure the compiler version is below 0.8.24 since Cancun compiler is not supported just yet
pragma solidity >=0.8.0 <=0.8.24;

contract Gmonad { 
    string public greeting;

    constructor(string memory _greeting) {
        greeting = _greeting;
    }

    function setGreeting(string calldata _greeting) external {
        greeting = _greeting;
    }
}
