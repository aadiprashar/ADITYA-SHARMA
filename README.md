# NFT Minting Project

This project demonstrates a basic implementation of minting NFTs (Non-Fungible Tokens) using JavaScript. The NFTs represent various districts in Uttarakhand, India, with metadata including the district name, photo, exploring places, local food, and feedback.

## Requirements

1. Create a variable that can hold a number of NFTs.
2. Create an object inside the `mintNFT` function that will hold the metadata for your NFTs. The metadata values will be passed to the function as parameters. When the NFT is ready, store it in the variable created in step 1.
3. The `listNFTs` function will print all of your NFTs' metadata to the console.
4. The `getTotalSupply` function should return the number of NFTs you have created.

## Project Structure

- **index.html**: The main HTML file.
- **index.js**: The JavaScript file containing the functions to mint and list NFTs, and to get the total supply of NFTs.

## Functions

### mintNFT

This function takes in values as parameters, creates an NFT object using the parameters passed to it for its metadata, and stores it in the `nft` array.

```javascript
function mintNFT(zila_name, photo, exploring_places, zila_food, feedback) {
    const NFT = {
        "zila_name": zila_name,
        "photo": photo,
        "exploring_places": exploring_places,
        "zila_food": zila_food,
        "feedback": feedback
    };
    nft.push(NFT);
    console.log("Minting", zila_name);
}
```
```
listNFTs
This function loops through the nft array and prints each NFT's metadata to the console.
function listNFTs() {
    for (let i = 0; i < nft.length; i++) {
        console.log("**********************************")
        console.log("*   THE LAND OF GOD- UTTRAKHAND   *");
        console.log("**********************************");
        console.log("ZILA NAME:\t" + nft[i].zila_name);
        console.log("PHOTO:\t" + nft[i].photo);
        console.log("EXPLORING PLACES:\t" + nft[i].exploring_places);
        console.log("ZILA FOOD:\t" + nft[i].zila_food);
        console.log("FEEDBACK:\t" + nft[i].feedback);
        console.log("*********************************");
    }
}
```
```

getTotalSupply
This function returns the total number of NFTs created.
function getTotalSupply() {
    return nft.length;
}
```
```
Usage
To use the project, include the index.js file in your HTML file and call the functions as demonstrated below:
// Minting some NFTs
mintNFT("DEHRADUN", "dehradun.png", "Mindrolling monestry, shiv Temple, Robber's cave", "Chana Madra, Dham, Siddu", "Dehradun, the capital city, nestled in the lap of the Himalayas, known for its colonial architecture as well as its beauty , scenic beauty, and delicious cuisine and having Lovely people.");
mintNFT("HARIDWAR", "haridwar.png", "ganges, Ganga Tat, Famous temple of Haridwar", "street food, vegetables-chaat, Bhel", "haridwar, known as the Valley of Gods and in hindu culture its also called the please where everyone gets peace after death, famous for its picturesque landscapes, adventure sports-rafting etc, and mouthwatering local delicacies.");
mintNFT("Rudraprayag", "rudraprayag.png", "Kedarnath Dham, Rivers, Beautiful and Ancient temples", "Aaloo ke gutke, Kafuli, Chha Gosht", "Rudraprayag, the cultural capital, located on the feet of Bholenath Lord shiva near kedarnath dham, renowned for its temples, lakes, and delectable cultural cuisine.");
mintNFT("chamoli", "chamoli.png", "chopta trek, Tungnath temple, Hemkund sahib", "Thukpa, Siddu, Dham", "Chamoli, the land of gods and goddesses, blessed with pristine beauty, apple orchards, and a rich cultural heritage, offering a delightful culinary experience.");
mintNFT("Pauri Garhwal", "gharwal.png", "Neelkanth mahadev, Binsar mahadev temple, jwalpa devi temple", "Bakery food , sattu, Tudkiya Bhat", "Gharwal, the valley of milk and honey, renowned for its ancient temples, lush greenery, and lip-smacking traditional cuisine.");
```
```

// Listing all NFTs to see their details
listNFTs();
console.log("Total NFTs created: " + getTotalSupply());
```

License
This project is licensed under the MIT License - see the LICENSE file for details.


// Printing the total number of NFTs created
console.log("Total NFTs created: " + getTotalSupply());

License
This project is licensed under the MIT License - see the LICENSE file for details.
