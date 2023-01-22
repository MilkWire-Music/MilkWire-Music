## How publishing content on MilkWire works 

Content is published on MilkWire using the following process:
![publishProcess drawio](https://user-images.githubusercontent.com/22245297/213942824-212745bb-33b8-4b2c-a33d-e5cbb340670a.png)


1. Artist Creates Album
2. Artist adds album to MilkWire to publish 
    1. CAR file is generated. (Same process as https://car.ipfs.io/)
    2. CAR file is uploaded to an ipfs node and replicated via pinning service (nft.storage) 
3. Artist publishes new album. This is an interaction with the smart contract. This adds the CID for the uploaded CAR file to the new entry in the artist's collection. 
    1. Users are able to pull the latest music by polling the smart contract for the user's address on the smart contract. 
4. Listener Follows an Artist Address
5. Listener Queries Artist Albums 
6. Listener Gets album IPFS CID 
7. Listener Streams Music From IPFS



##Quick primer 

### What is IPFS

IPFS is the "InterPlanetary File System". It is a universal content addressing scheme. This means having a file hash not only describes the file but also the location of that file on the network. A way to think about this is it is like a universal bittorrent swarm where all files can be identified by a hash identifier. 

The advantage of IPFS is the content addressing scheme. This allows data to be identified and located by a hash. That can be abstracted away to either local, lan or file copies avaiable on a remote ipfs node. 

### What is a CAR file? 
Car stands for "Content Archive Format". It is part of the [ipfs standard](https://ipld.io/specs/transport/car/). Car files can be thought of as "TAR files that are designed for storing collections of content addressed data" - Form [this article by nft.storage](https://nft.storage/docs/concepts/car-files/). 
