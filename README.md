# Ethereum Classic Carbon Voting Experiments

*Please note that this project should be in no way considered an
"official" Ethereum Classic project, and no one is going to make a
definitive decision (at least for now) based on the voting here.*

Carbon vote is an idea to give voters voting rights by how much coin
they own. It has the feature that it is conducted without requiring
any coins to leave the voters' wallets. This repository is an
experiments of using Carbon voting for some Ethereum Classic related
issues using the Github Issues interface.

## How Do I Vote?

Go to [Issues](https://github.com/sorpaas/etcarbon/issues) page and
you will find the currently voting issues. In the first comment of
every issue, you can find the voting addresses for "Yes", "No", and
"This proposal is not clear".

Send a zero value transaction to any of those addresses to vote. If
you later changed your opinion, resend another zero value transaction
to any of those addresses again.

## How Do I Make a New Proposal?

Create a new [issue](https://github.com/sorpaas/etcarbon/issues/new)
with your proposal. In your proposal, please explain in detail about
what this voting is about for "Yes" and "No". You also need to specify
a voting period.

Next you need to create the voting contracts. Right now this should be
done by hand. In the future this will be automated by a Github bot.

Create three voting contracts "Yes", "No", "This proposal is not
clear" using the contract code provided
at [contracts/vote.sol](contracts/vote.sol). Please let a developer
know if you have trouble deploying the contracts.

After the voting period end, the actual voting rates can be collected
from the blockchain. We will soon publish a tool to do this.

## FAQ

### Why do we use Github Issues rather than a webpage like Ethereum's CarbonVote.com?

Github Issues allow civilized discussions of a proposal that has been
tested by many open source projects. This is at least better than a
simple web page that people cannot comment or improve the proposal.

Github also has a good spam detection method that prevents a user to
register many multiple Github accounts to spam this repository.

### You mentioned that this is an experiment. What is the goal for this repository?

Besides the actual voting on the proposals we have currently, the goal
is to gradually improve the voting contracts and make it "fair" so it
can be used in the future to make big decisions for the community. For
example, a hard fork.
