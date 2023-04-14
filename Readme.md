MyToken Smart Contract 


This is a smart contract written in Solidity that creates a custom token called "Solana".

Requirements


The contract has public variables that store the details about the coin (Token Name, Token Abbrv., Total Supply).
The contract has a mapping of addresses to balances (address => uint).
The contract has a mint function that takes two parameters: an address and a value. The function then increases the total supply by that number and increases the balance of the “sender” address by that amount.
The contract has a burn function, which works the opposite of the mint function, as it will destroy tokens. It will take an address and value just like the mint functions. It will then deduct the value from the total supply and from the balance of the “sender”.
The burn function should have conditionals to make sure the balance of "sender" is greater than or equal to the amount that is supposed to be burned.


Public Variables


      TokenName: A string variable that stores the name of the token.
      TokenAbbrv: A string variable that stores the abbreviation of the token.
      TotalSupply: An unsigned integer variable that stores the total supply of the token.


Mapping


      balances: A mapping variable that maps an address to a uint value that stores the balance of that address.


Functions


      mint(address _address, uint _value)


              This function takes two parameters: an address and a value. The function then increases the total supply by that number and increases the balance of the “sender” address by that amount.

      burn(address _address, uint _value)


          This function takes two parameters: an address and a value. It will deduct the value from the total supply and from the balance of the “sender”. It has       conditionals to make sure the balance of "sender" is greater than or equal to the amount that is supposed to be burned.
