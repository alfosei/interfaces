# **Clet Name Service Payment Contract** 
## **Description**: 
**This contract serves as a payment gateway for acquiring clet names**

> **⚠ NOTICE!** : *All function inputs must be lowercase to prevent undesirable results*

**Functions**:

- [*pay*](#1-function-pay)
- [*addYears*](#2-function-addyears)
- [*getAmountToPay*](#3-function-getamounttopay)
- [*getEthPrice*](#4-function-getethprice)
- [*setListingPrice*](#5-function-setlistingprice)
- [*buyListedName*](#6-function-buylistedname)
- [*transferName*](#7-function-transfername)
- [*nameExists*](#8-function-nameexists) 
- [*isExpired*](#9-function-isexpired)

## 1. **function *pay***
___
This function takes three parameters, **'name'** of type ***string***, **'years'** of type ***integer*** and **'partner'** of type ***address***. It unlocks any available name on the **SKALE** Chain.
```shell
function pay(string memory _name, uint256 _years,
address _partner) external payable;
```
## 2. **function *addYears***
___
This function takes two parameters, **'name'** of type ***string*** abd **'years'** of type ***integer***. It adds specified number of years to an existing name.
```shell
function addYears(string memory _name, uint256 _years) external payable;
```

## 3. **function *getAmountToPay***
___
This function takes two parameters, **'name'** of type ***string*** and **'years'** of type ***integer***. It returns the price of a name based on number of years.
```shell
function getAmountToPay(string memory _name, uint256 _years) external view;
```

## 4. **function *getEthPrice***
___
This function returns the current ETH value in USD.
```shell
function getEthPrice() external view returns (uint256);
```

## 5. **function *setListingPrice***
___
This function takes two parameters, **'name'** of type ***string*** and **'amount'** of type ***integer***. It allows a user to set the cost price of an owned name.
```shell
function setListingPrice(string memory _name, uint256 _amount) external;
```

## 6. **function *buyListedName***
___
This function takes one parameter, **'name'** of type ***string***. It acquires a non-expired listed name.
```shell
function buyListedName(string memory _name) external payable;
```

## 7. **function *transferName***
___
This function takes two parameters, **'name'** of type ***string*** and **'newOwner'** of type ***address***. It transfers an owned name to a new owner. The function is also called before transfer on **SKALE** Chain
```shell
function transferName(string memory _name, address _newOwner) external;
```

## 8. **function *nameExists***
___
This function takes one parameter, **'name'** of type ***string*** and returns a boolean value. It checks if a name is owned.
```shell
function nameExists(string memory _name) external view returns (bool);
```

## 9. **function *isExpired***
___
This function takes one parameter, **'name'** of type ***string***. It checks if a name is expired. It also returns a boolean value.
```shell
function isExpired(string memory _name) external view returns (bool);
```

# **Join Our Community**

- [Clet - One Name For All Blockchains](https://www.clet.domains/)
- [Discord](https://discord.gg/TDedn26Hnc)
- [Twitter](https://twitter.com/cletNS)
