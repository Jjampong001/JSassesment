let collectionNFT = []; 

function mintNFT (_name, _color, _breed, _weight) {
    const Dog ={
        "name":_name,
        "color":_color,
        "breed":_breed,
        "weight":_weight,
    }
    collectionNFT.push(Dog);
console.log("minted: " + _name);

}    
function listNFTs () {
    for(let i = 0; i < collectionNFT.length; i++){
        console.log("\nId: \t\t" + (i+1));
        console.log("name: \t\t"+ collectionNFT[i].name);
        console.log("color: \t\t"+ collectionNFT[i].color);
        console.log("breed: "+ collectionNFT[i].breed);
        console.log("weight: \t\t"+ collectionNFT[i].weight);
    }    
}
function getTotalSupply() {
    console.log("TOTAL NFTs:" + collectionNFT. length);
}
mintNFT("Whitey","White","Aspin","15kg");
mintNFT("Blacky","Black","Aspin","25kg");
mintNFT("Browny","Brown","Aspin","18kg");
mintNFT("Bruno","Dark Brown","Aspin","5kg");
listNFTs();
getTotalSupply();
