let nfts = [];
// 2. mintNFT function creates an NFT object and stores it
function mintNFT(name,about, imageURL) {
  // Create an NFT object with the provided metadata
 const nft = {
name: name,
 about: about,
 imageURL: imageURL,
  };
  // Add the NFT object to the nfts array
 nfts.push(nft);
}
// 3. listNFTs function iterates through the nfts array and prints metadata
function listNFTs() {
 console.log("Your NFTs:");
// Loop through each NFT in the nfts array
for (const nft of nfts) {
console.log("Name:", nft.name);
console.log("About:", nft.about);
console.log("Image URL:", nft.imageURL);
console.log("---");
  }
}
// 4. getTotalSupply function returns the length of the nfts array
function getTotalSupply() {
 return nfts.length;
}
// Call the functions to test them (example usage)
mintNFT("Java Script", "A unique langauge", "https://.../javasc.png");
mintNFT("metacraft", "learn different skills  ", "https://.../metacf.jpg");
console.log("Total NFTs:", getTotalSupply());
listNFTs();
