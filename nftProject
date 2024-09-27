import java.util.ArrayList;
import java.util.List;

class NFT {
    String name;
    String artist;
    int year;


    public NFT(String name, String artist, int year) {
        this.name = name;
        this.artist = artist;
        this.year = year;
    }


    public void displayNFT() {
        System.out.println("Name: " + name);
        System.out.println("Artist: " + artist);
        System.out.println("Year: " + year);
        System.out.println("-----------------");
    }
}

public class Main {
    static List<NFT> nftCollection = new ArrayList<>();


    public static void mintNFT(String name, String artist, int year) {
        NFT nft = new NFT(name, artist, year);
        nftCollection.add(nft);
    }


    public static void listNFTs() {
        for (int i = 0; i < nftCollection.size(); i++) {
            System.out.println("NFT #" + (i + 1) + ":");
            nftCollection.get(i).displayNFT();
        }
    }


    public static int getTotalSupply() {
        return nftCollection.size();
    }

    public static void main(String[] args) {

        mintNFT("AirJordan x Dior", "Nike and Christian Dior", 2020);
        mintNFT("Nike Jumpman Jack", "Travis Scott", 2024);
        mintNFT("Medelin Sunset", "Nike x J Balvin", 2023);

        listNFTs();
        System.out.println("Total NFTs minted: " + getTotalSupply());
    }
}
