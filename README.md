# RandLabs Solidity Challenge

## Sport Gambling  
  
### Summary  
  
A gambling app is a service where the people can bet to their favorite team for a game expecting a huge reward in case they win it. In the other case that their team lose the game, the users will lose their betted amount. The gambling process is very easy, there are two pools, one for every team. The users to bet to their favorite team, they need to put the money into the respective team pool. Once one of the them win the match the total amount in the pool of the loser team will be distributed proportionally to the users that betted to the winner team.

#### Considerations: 
- 1% of the total amount in both pools is for fees. That means if there are total of USD50.000 in both pools, USD500 corresponds for fees and USD49.500 for the rewards.
- The user can cancel their bet and withdraw all the amount or modify the amount deposited in the contract.
- New entries, updates or cancel bets must be accepted until 1 hour before the match.
- Everyone can create a match but only the owner/creator of the contract can withdraw the fees.
- Only the creator of the event can set the match result.
- If a match is canceled, you must return the amount betted from the users or allow the users to withdraw their betted amount.
- The user can only withdraw their rewards after the creator set the result of the match.

### Example

Lets say that there are 2 users, User A and User B, and two teams, Team X and Team Y. Use user A wants to bet 100 USD to the Team X and the user B wants to bet to the Team Y. The total price pool is 100.000 USD, where USD1.000 is on fees, USD29.700 is the total amount betted for Team X and USD69.300 is the total amount betted for team. If the Team X wins the game, the User A will receive the USD99 (after fees) from his bet plus USD231 from the Team Y reward pool. The User A won a total of USD310. 

### Requirements

- You can use any library like truffle to develop this challenge.
- Write tests. Make sure that all your code is tested properly.
- Create a script in Javascript to interact with the contract, prefereable implement it using _ethers.js_.

### Nice to have

- A GUI to interact with the Smart Contract prefereable in React.
