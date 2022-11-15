# NFT_USING_MORALIS

Git Link: https://github.com/roopatumu/NFT_USING_MORALIS.git


How to build your own nfts using the tools provided by morales Morales provides a very nice integration with ipfs, the industry standard for decentralized storage, allowing us to build nfts on-the-fly using only graphical user interfaces and minimal amounts of code. To get started, we'll go to this page to sign up for our dap. 

We can communicate with it. This is because minting is a transaction, and we need an active ethereum address to submit transactions to the blockchain. Now, we want to create a nft name, but we'll do that after we choose the file because this will be something intriguing and the one that we're going to mint is the powerful.

We're going to mint this one as a nft, so we're going to choose the name we're going to call it powerful ivan fingers amazing stamina likes. I believe that was his name, the person who invented it. The name and description of our nft are web3, who frequents the gym, enjoys hiking, and drinks an excessive amount of coffee. Let's go on to the next minute.
  
Let's do it now. We're going to upload a mint. This may take some time because there are a lot of things happening in the background, and this is one of them. We need to sign the transaction because we're about to deal with a contract.

We need to send the transaction to the contract, and we have the transaction through which we repaired the nft. It might take some time for us to see it in our open sea, but the transaction was confirmed in my open c collection. We have strong ivan fingers, and we have all the describing information about it, so obviously we have the image and we have a great stamina like guev 3, who regularly works out at the gym, enjoys going on hikes, and drinks too much coffee.


We are currently in the testnet and this is it, guys. It's a pretty great app and you can mint your own nfts with it, but how does this app work? That was intended in this contract and it was done through the rinkevi blockchain, so this is it. What we have here is a pretty basic Flask application. Typically, a random Raspberry Pi executes our application, which then activates all of the files under this app directory, including the index.html file over here.
   
The nft minter requires the name of the nft, the date, a description, and the most crucial field of all, which is our file element. When we upload this file element, we will be able to of loaded and minted with this button that will trigger our logic. Once our logic runs, we display the result of the transaction that trigger are n.
    
Let's investigate the logic to see what it all means. To analyze the reasoning, keep in mind that a nft is similar to a deed of property. If you visit the property registration in your city, you will see that it has electronic records, and those electronic records have metadata about the property.

They did include the owner's information, however metadata serves as the description and serves to identify the item. When you mint a nft, the key issue that you deal with is integrating the token with the metadata. This includes knowing the address of the house, the cadastral information about the house, which means knowing the asset value for tax purposes, and the blueprints and measurements of the property.

There are two ways to deal with it: either you can deal with it in a centralized fashion, which is pretty okay but then you will have a single point of failure, or you can do it more in line with what the blockchain industry is all about: you can do it in a decentralized fashion, but if you do it that way, you will need access to ipfs. The token says who is the owner because it has the information about that in the blockchain, but the metadata identifies the object.
    
 With that in mind, dealing with ipfs directly may require some heavy effort on your part in order to have this functionality prepared in your dab. If you utilize Morales, however, this will be really simple. I'll give you an example. Here, we have the function that activates when we pick our file.
 
 We only want the first file that is captured by this interaction with this file that we are capturing from that element of our html, so we're just going to point here to element 0. When we click upload, what happens is that it collects the get element by id of our file component that we have in our html. This component captures files in an array.
 
 We are creating a new moralist file object. Once we have this object, it is very simple to save it either to the decentralized ipfs network or the slightly centralized morale server; morale supports both methods. In this case, we will save the object in a decentralized manner by sending the command image file save to ipfs.
 
 When we save our image to ipfs, we will receive two things from morales. First, we will receive the hash of the file in ipfs, which is the method that ipfs uses to identify that no single file is duplicated in their network. Second, we will receive the name of the moralist object that we created here. We are saving this moralist object that we created here to ipfs. Here in the middle, we are simply deactivating these elements 
 
So this is what we are going to acquire from Morales here. Now that we have that image url, we will generate a metadata object that contains everything that we are going to save regarding our nft. The url basically has to be provided by someone who has an ipfs gateway in this case Morales offers you both.

When we have all the metadata ready, we will simply do the same thing that we did before and store that in ipfs but this time we will do it by storing the json object, so that's what we are doing. We are getting our element by id here, which is our name for the name of our nft, our description, which is the description of our nft, and the image, which will be represented by the image jury that we are getting from morality in the

That I'm setting up here with the json javascript object that you have created here will accomplish the task of serializing this for you in order to store it in ipfs, something that morales is also providing for you out of the box. After we have that numericalist file ready and we simply save it to ipfs, we get our ipfs url or jury, and then with that we can call our mean token function, which means token is done by interacting with it

Here's what we have: Returning to our logic for our minting token function, we are simply sending a transaction to the contract that we are describing over here, and that transaction must contain the encoded function call. As a result, we are only receiving the API for the function that we are calling with the parameter and that will be encoded by this functionality that we are creating here.

We add the function to the transaction as a transaction parameter, send it to the blockchain, and wait for the transaction hash to be returned. At that point, we know the transaction has been processed and can print the user's transaction id, indicating that the nft has been created successfully. We connected with a metal mask, gave our nft a name, and described the qualities we intended to attribute to this nft. After selecting your file, minting it, and receiving this transaction, if you go to open C, here is our nft.
