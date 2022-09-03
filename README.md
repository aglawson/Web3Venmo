# P2

P2 is a web3 version of a peer to peer payment platform (think venmo, zelle, etc).
P2 is more user friendly than just using the base layer of ETH to move value, because it relies on usernames rather than unreadable wallet addresses. 

## In the works
1. Add ERC20 tokens **done**
2. Add ability to add users as 'friends' who can request payments (similar to venmo) **done**
3. Remove USD conversions (to make #1 more smooth) **done**
4. Test profusely *In Progress*
5. Simple frontend to visualize functionality

## Latest Test Results
```
    Deployment
      ✔ initializes ETH token at deployment (42ms)
    Account Functionality
      ✔ can create new accounts (59ms)
      ✔ users can add friends (47ms)
      ✔ can deposit funds
      ✔ can request funds from friends (46ms)
      ✔ can fulfill requests (62ms)
      ✔ user can reject request (60ms)
      ✔ can send funds (83ms)
      ✔ user can withdraw funds (84ms)
      ✔ user can remove friends
    ERC20 Functionality
      ✔ owner can add ERC20 token
      ✔ user can deposit ERC20 token (96ms)
      ✔ user can withdraw ERC20 (64ms)
    Security
      ✔ only owner can add tokens (46ms)
      ✔ only friends can request money
      ✔ does not allow duplicate usernames
      ✔ does not allow same wallet to make multiple accounts
      ✔ does not allow funds to be sent to non existent user (38ms)
      ✔ does not allow users to fulfill requests not sent to them (76ms)
      ✔ does not allow a rejected request to be fulfilled (52ms)


  20 passing (2s)

```