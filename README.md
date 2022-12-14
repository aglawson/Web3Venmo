## NOTE: Feel free to improve frontend, I know it is horrendous.

# Web3Venmo
This is a web3 version of a peer to peer payment platform (think venmo, zelle, etc).
It is more user friendly than just using the base layer to move value, because it relies on usernames rather than unreadable wallet addresses. 

# Frontend
Avalanche Network Only
https://aglawson.github.io/P2/
contract address: 0xB3b42e9CffC5526Dd11Aa5DB433D576C1941a14F
Current value in contract: 0.01 AVAX, 100 VPND

## In the works
1. Add ERC20 tokens **done**
2. Add ability to add users as 'friends' who can request payments (similar to venmo) **done**
3. Remove USD conversions (to make #1 more smooth) **done**
4. Test profusely **done**
5. Simple frontend to visualize functionality **done**

## Latest Test Results
```
    Deployment
      ✔ initializes BASE token at deployment
    Account Functionality
      ✔ can create new accounts
      ✔ users can add friends (74ms)
      ✔ can deposit funds
      ✔ can request funds from friends (41ms)
      ✔ can fulfill requests (47ms)
      ✔ user can reject request (49ms)
      ✔ can send funds (59ms)
      ✔ user can withdraw funds (46ms)
      ✔ user can remove friends
    ERC20 Functionality
      ✔ owner can add ERC20 token
      ✔ user can deposit ERC20 token (74ms)
      ✔ user can withdraw ERC20 (62ms)
    Security
      ✔ only owner can add tokens (39ms)
      ✔ only friends can request money
      ✔ does not allow duplicate usernames
      ✔ does not allow same wallet to make multiple accounts
      ✔ does not allow funds to be sent to non existent user (38ms)
      ✔ does not allow users to fulfill requests not sent to them (88ms)
      ✔ does not allow a rejected request to be fulfilled (46ms)
      ✔ does not allow a user to reject a request not sent to them (88ms)


  21 passing (2s)

```
