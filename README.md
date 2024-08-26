# Polkadot Developer Bounties

Community Driven Development and Maintenance for the Polkadot Ecosystem

## Goals

Maintaining an ecosystem as large as the Polkadot Developer community is not easy!

Unlike more traditional developer ecosystems, the Polkadot community is entirely decentralized.
There are over 100 development teams all contributing to the Polkadot developer ecosystem.
This means that maintaining high quality developer documentation and resources is particularly difficult.

The goal of this repository is to coordinate and incentivize community driven development and maintenance of the Polkadot ecosystem.

Here, you will find ways to contribute to the Polkadot developer ecosystem, either by noting issues

## How

The Polkadot Developer Bounties is powered by the [Substrate Tip Bot](https://github.com/paritytech/substrate-tip-bot).

The Substrate Tip Bot is a GitHub application which can make submit Tip proposals to the Polkadot treasury.
The tip bot is triggered by curators / owners of this repository, who will review evidence submitted to this repository.

### Submissions

When you make a contribution that improved the Polkadot developer ecosystem, you can open a pull request to update the [`submissions.json`](submissions.json) file included in this repository.

In that file, you should add a new entry with the following information:

```json
{
	"author": "<github username>",
	"description": "<short description of problem solved / work done",
	"evidence": "<github pull request url>"
}
```

Then in the body of your pull request you must be sure to include the text:

```text
polkadot address: <SS58 Address>
```

Curators of this repo will review your work and either accept or reject your pull request, to keep track of the work done by the community.

The author of the github pull request must match the author of the evidence so that there is no chance that someone is claiming credit for someone else's work.

You can see an example of a simple submission here: https://github.com/substrate-developer-hub/bounties/pull/1

### Rewards

As mentioned above, this project uses the [Substrate Tip Bot](https://github.com/paritytech/substrate-tip-bot), which can open a tip for authors of a pull request.

If the pull request is accepted by this repo, you should also find that one of the curators trigger the tip bot via a comment like:

```text
/tip {small | medium | large | <custom value>}
```

You should review the `substrate-tip-bot` project to get the latest details on the size of these tips.

This does NOT automatically pay the contributor, but simply submits a proposal to Polkadot which is reviewed by OpenGov.

Note that it is possible that even after your contribution is accepted here, it may be possible that OpenGov rejects the tip. However, we assume that the quality and size of tips approved by the curators will lead to a high acceptance rate by the Polkadot governance.

You can see on-chain activity of the tip bot account here: https://polkadot.subscan.io/account/14Sbk1RvKa9x7k8CThWoEYKA21LDduRbcivnzkDdm2WnDutM

## Rules

This project openly acknowledges that creating a system for rewarding people to submit and fix issues is ripe for abuse and grifting.

As such, it is important to establish rules defining the expected conduct around this initiative.

1. No asking for, expectation of, or discussion of payments.

	The primary goal of this repository is to maintain the Polkadot developer ecosystem. The rewards system exists, and acts as a catalyst for proactive contributions, but should not really be the point of discussion or a general expectation from anyone. Avoid comments like:

	- "I will work on X if I get paid $Y."
	- "I should receive $X, because it took me Y hours to complete this issue."

2. Respect the opinions of the curator.

	The curators have full control over evaluating contributions and rewards. Curators have the best interests of the community in mind, and thus are incentivized to evaluate and reward people to encourage future contributions.

3. No double dipping.

	Submitters should not be paid multiple times for doing the same work. This means that if you already received a tip or bounty reward for some fix, you should not submit it again here. Similarly, if you are an owner of an open source project and are being funded already, you should not submit another request here. This is really for community members to earn small rewards for actively

4. No spamming.

	Submitters should use common sense to determine when it is appropriate to submit a contribution. Trivial and mindless contributions will not be accepted or tolerated.

	- Adding a single punctuation is spam.
	- Deleting a double newline is spam.
	- Mindlessly formatting text through a tool is spam.
	- etc...

	That is not to say that we do not want these kinds of contributions in general, but practically speaking, this is not the quality or size of work which deserves payments or tips. Use your best judgement here, and listen to feedback from the curators if they reject your submission.
