# Collectibles

{% hint style="info" %}
Developer Note: Collectibles are referred to as NFT Models in the API.
{% endhint %}

**Collectibles** are essentially templates for all of the NFTs that are being made. This template contains all of the metadata and everything for everyone of the NFTs. Let's say I want to create 100 of an NFT. I'll create one Collectible (i.e. the template) and each of the 100 NFTs will use the same data from this Collectible. They'll all have their own serial number to differentiate them.&#x20;

There are a few defined fields that you'll need to fill out to define your **Collectible.** When you've created this Collectible, it's immediately ready to mint or transfer via our APIs.&#x20;

![Create a Collectible. Go to Collection -> \[Set\] -> \[+ New Collectible\]](<../../.gitbook/assets/image (9).png>)

**Field Reference:**&#x20;

* Title (Required): The title for these NFTs
* Description (Required): The title for these NFTs
* Quantity (Optional): The number of NFTs to create from this Collectible. If blank, this will be an unlimited quantity.&#x20;
* Rarity (Required): The specified rarity for these NFTs.&#x20;
* Artists (Optional): The names of any artists, companies, or organizations that you'd like to be associated with this NFT.&#x20;
* Poster (Required): An image to use as the poster image for this NFT. This is required because some external products (i.e. wallets, marketplaces) can only show images.
* Primary Content (Required): An image, video or anything else that you'd like to mint.

Then, there are advanced fields (all optional).

* Blockchain Metadata: These are key, value pairs that you'd like to put on the final blockchain.&#x20;
* Off-Chain Metadata: This is additional metadata, not put on chain that may be used for filtering, sorting or any other information on your applications.&#x20;
