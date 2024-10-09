# Questions 

## Solidity
Write a function that will delete items (one at a time) from a dynamic array without leaving gaps in the array.

You should assume that the items to be deleted are chosen at random, and try to do this in a gas efficient manner.

For example imagine your array has 12 items and you need to delete the items at indexes 8, 2 and 7.

The final array will then have items {0,1,3,4,5,6,9,10,11}

## Extra Question :
When creating the function selector "uint" will be replaced by "uint256" , see the example here from the Docs

 `0xa5643bf2`: the Method ID. 
  
  This is derived from the signature 
  
  `sam(bytes,bool,uint256[])`. 
  
  Note that `uint` is replaced with its canonical representation `uint256`.
Could this be used maliciously in an exploit, if so, how would that be done ?


# Answers

## Extra Question:
Here is an example on how we could "exploit" this by misleading users:

Open in remix: 
https://gist.github.com/Nynko/4d26cc93e3efcd71be105d331cc5a8ca

It may not be the expected answer but seems to be an exploit. 
