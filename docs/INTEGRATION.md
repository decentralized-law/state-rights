# Website Integration Guide

This guide explains how to add the Declaration of State Rights and Duties to your website.

## Basic Implementation

1. **Download the file**
   - Download the `StateRightsFrontEnd.html` file from this repository's `frontend` directory

2. **Add to your website**
   - Copy the HTML code from the file
   - Paste it into any page on your website where you want to display the Declaration
   - **Important:** Many standard content management systems, such as WordPress, require a specific HTML embedding approach (see Website Builder Implementation below)

3. **Key customization points**
   - Contract address: The file is pre-configured with the official Ethereum contract address `0x1855cc1cd697baf8a014c5bae7f18505f855aca6`
   - RPC URL: Modify the `rpcUrl` variable to use your preferred Ethereum node provider if needed
   - Styling: Adjust the `titleStyle` and `textStyle` variables to match your website's design

### Website Builder Implementation

When using website builders such as WordPress, Wix, Squarespace, or Shopify, you might need to use their specific HTML embedding features to add this code to your site. Look for options like "Custom HTML," "HTML Embed," "Code Block," or similar functionality in your website builder's interface. Make sure you're pasting the code in HTML mode rather than visual/text mode for proper functionality.

## Configuration Options

### Contract Address

```javascript
// The official deployed contract address
const contractAddress = "0x1855cc1cd697baf8a014c5bae7f18505f855aca6";
```

### Ethereum Network URL

```javascript
// Ethereum Mainnet (production)
const rpcUrl = "https://ethereum.publicnode.com";
```

You can use any Ethereum mainnet RPC provider of your choice, including your own node if you have one.

## Alternative Integration Methods

### IPFS Integration

If you prefer to load the Declaration from IPFS instead of directly from the Ethereum blockchain, you can use the following IPFS CID:

```
bafkreihse425qqhba26kcfpjkgqr73dsu3zxopniivjwlqzcfiii25xqr4
```

You can access this through any IPFS gateway, for example:
```
https://gateway.pinata.cloud/ipfs/bafkreihse425qqhba26kcfpjkgqr73dsu3zxopniivjwlqzcfiii25xqr4
```

## That's it!

The HTML file is self-contained with all necessary code to fetch and display the Declaration of State Rights and Duties. No additional files or dependencies need to be installed on your server.
