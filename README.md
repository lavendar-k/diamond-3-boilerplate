# Diamond-3-Hardhat Implementation

This is an implementation for [EIP-2535 Diamond Standard](https://github.com/ethereum/EIPs/issues/2535). To learn about other implementations go here: https://github.com/lavendar-k/diamond-3-boilerplate

The standard loupe functions have been gas-optimized in this implementation and can be called in on-chain transactions. However keep in mind that a diamond can have any number of functions and facets so it is still possible to get out-of-gas errors when calling loupe functions. Except for the `facetAddress` loupe function which has a fixed gas cost.

**Note:** The loupe functions in DiamondLoupeFacet.sol MUST be added to a diamond and are required by the EIP-2535 Diamonds standard.

## Installation

1. Clone this repo:
```console
git clone git@github.com:lavendar-k/diamond-3-boilerplate.git
```

2. Install NPM packages:
```console
cd diamond-3-boilerplate
npm install
```

## Deployment

```console
npx hardhat run scripts/deploy.js
```

