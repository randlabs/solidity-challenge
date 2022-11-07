# RandLabs Solidity Challenge

## Sport Gambling  
  
### Summary  
  
A gambling app is a service where individuals can bet on their favorite teams to win games for a potential reward. However, if their team loses the game, the users will lose their betted amount. The gambling process is very easy - there are two pools, one for every team. For users to bet on their favorite team, they need to put the money into the respective team pool. Once one of the teams win the match, the total amount in the pool of the losing team will be distributed proportionally to the users that bet on the winning team.

#### Considerations: 
- 1% of the total amount in both pools is for fees. That means if there is a total of USD50.000 in both pools, USD500 corresponds for fees and USD49.500 for the rewards.
- The user can cancel their bet and withdraw the entire amount or modify the amount they deposited in the contract.
- New entries, updates or cancelled bets must be accepted up to 1 hour before the match.
- Anyone can create a match but only the owner/creator of the contract can withdraw the fees.
- Only the creator of the event can set the match result.
- If a match is canceled, you must return the amount betted from the users or allow the users to withdraw their betted amount.
- The user can only withdraw their rewards after the creator has set the result of the match.
- The smart contract must use an ERC20 token previously created with the same characteristics as the USDC token.

### Example

Let's say that there are 2 users, User A and User B, and two teams, Team X and Team Y. Use user A wants to bet 100 USD to the Team X and the user B wants to bet to the Team Y. The total prize pool is 100.000 USD, where USD1.000 is on fees, USD29.700 is the total amount betted for Team X and USD69.300 is the total amount betted for team. If the Team X wins the game, the User A will receive the USD99 (after fees) from his bet plus USD231 from the Team Y reward pool. The User A won a total of USD310. 

### Requirements

- Design and code a contract for Sport Gambling app, take all the assumptions you need to move forward. You can use any library like truffle to develop this challenge.
- Write tests. Make sure that all your code is tested properly.
- Create a script in Javascript to interact with the contract, prefereable implement it using _ethers.js_.

### Nice to have

- A GUI to interact with the Smart Contract prefereable in React.
