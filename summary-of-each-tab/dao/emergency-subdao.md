# Emergency subDAO

The [Emergency DAO](https://dao.curve.fi/emergencymembers) is an idea pioneered by Curve that empowers a small group to “kill” pools and gauges **in the** **event of malicious activity and/or potential loss of funds.** The Balancer emergency subDAO was established after the [following vote](https://vote.balancer.fi/#/proposal/0x63fab7ab9ef5b9579dabb82058b8ea309e39c766d435438b55fff8db7c1f69fd).&#x20;

The Emergency subDAO is a 4-of-7 multisig with the following members:

* Solarcurve (0x512fce9B07Ce64590849115EE6B32fd40eC0f5F3)
* Mike B (0xF01Cc7154e255D20489E091a5aEA10Bc136696a8)
* Zekraken (0xafFC70b81D54F229A5F50ec07e2c76D2AAAD07Ae)
* Zen Dragon (0x7c2eA10D3e5922ba3bBBafa39Dc0677353D2AF17)
* Markus (0x6bB4720473d4D7133f944785e5EE1A650C07f34e)
* Fernando (0xbbF0Ae5195444264364CA7eb7E3BB1971B4c3eCb)
* Nico (0x815d654E930E840D0E0Ee1B18FFc8Fb4ddA4c6B3)

Gnosis safe addresses:
- Ethereum: [0xA29F61256e948F3FB707b4b3B138C5cCb9EF9888](https://gnosis-safe.io/app/eth:0xA29F61256e948F3FB707b4b3B138C5cCb9EF9888/home) 
- Polygon: [0x3c58668054c299bE836a0bBB028Bee3aD4724846](https://gnosis-safe.io/app/matic:0x3c58668054c299bE836a0bBB028Bee3aD4724846/home)
- Arbitrum: [0xf404C5a0c02397f0908A3524fc5eb84e68Bbe60D](https://gnosis-safe.io/app/arb1:0xf404C5a0c02397f0908A3524fc5eb84e68Bbe60D/home)
- Optimism: [0xd4c87b33afcE39F1E3F4aF1ce8fFFF7241d9128B](https://gnosis-safe.io/app/oeth:0xd4c87b33afcE39F1E3F4aF1ce8fFFF7241d9128B/home)



An additional power of the Emergency subDAO will be to add a token to the deny list on the newly created “[ProtocolFeesWithdrawer](https://forum.balancer.fi/t/introduce-protocolfeeswithdrawer/3188)” contract. In order for a token to be added back to the allow list a veBAL governance vote would be required. A token would only be added to the deny list in the event of an issue along the lines of the recent [Synthetix bug disclosure](https://forum.balancer.fi/t/medium-severity-bug-found/3161).

\
[The BIP139 ](https://snapshot.org/#/balancer.eth/proposal/0x6e0d7cbcd35f9b3949bf7f4607d71ac66a97561b0f304a1939c400f710ea0cbd)updates the following permissions of the Emergency subDAO:\
\-`enableRecoveryMode()` for Pools to provide a simple way to exit pools proportionally at the cost of disabling protocol fees (swaps, joins, etc. still work)

\-`denylistToken()` to prevent withdrawing certain tokens from the protocol fee withdrawer

\-`disable()` to shutdown pool factories ( this is to prevent further pools from being created, existing pools remain unaffected)

