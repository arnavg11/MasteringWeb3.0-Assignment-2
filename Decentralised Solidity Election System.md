# Decentralised Solidity Election System
## Candidate registration
Registration for candidates can be done by the candidate's node itself using registerCandidate(). The candidate's desired ID should not be taken as it is the primary key to vote or access any candidate details.
## Voter registration
Voter's have to be registered by the election's moderator(set to the address of the person who initialised the contract) using registerVoter().
## Casting votes
Voters can cast votes by their registered systems using castVote(). Once a vote is cast, the voter is deemed ineligible to further vote.
## Candidate details
Details about a candidate's name and current votecounts can be accessed by anyone by providing the desired candidate's ID using getName() and seeVotes() respectively.
## Election results
The result of the elections can be viewed using getWinner(). It returns the ID of the candidate witht he most number of votes.