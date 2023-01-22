# Data storage in MilkWire 
MilkWire is primarily a content publishing system. Artists can publish new Albums by appending their catalog through interacting with the smart contract. 
The smart contract acts as an index of artists and content creators. Those content creators are able to publish new content with a link to the CID of the 
media. Users can subscribe to artists and automatically get the latest releases by those artists. Any user is able to create curator accounts. 
Curator accounts can create playlists or slectively share already published content on the network. 



## Artist Identity 
Artist identity in MilkWire is based around an artis't address. In ethereum addresses can either be externally owned accounts (EOA) or Contract accounts. 
When an artist creates an account on MilkWire they are registering a new artist address on the MilkWire index. 

The milkwire index is a smart contract that is able to keep a sequential list of all published work by an artist. 

## How is content stored on MilkWire?

The actual media is stored on IPFS.

IPFS (The InterPlanetary File System) https://ipfs.tech/ is the backbone of the data storage for the MilkWire protocol. 
IPFS allows content to be addressesd by a universal content identifier (CID). This CID is used to retrieve the data from the p2p network
through either a local node or a remote gateway.

