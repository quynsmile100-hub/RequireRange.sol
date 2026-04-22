# RequireRange.sol
RequireRange.sol
pragma solidity ^0.8.20;
contract RequireRange {
    uint public num;

    function set(uint x) public {
        require(x >= 1 && x <= 50, "Out of range");
        num = x;
    }
}
