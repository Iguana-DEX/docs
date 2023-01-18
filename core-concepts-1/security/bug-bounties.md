# Bug Bounties

{% hint style="warning" %}
The bug bounties on this page apply only to the Balancer **smart contracts** which secure protocol funds on the Ethereum mainnet. Bug reports pertaining to Balancer's web interfaces, both in terms of UI/UX or servers/infrastructure, are not eligible. Only the first reporter of a given contract vulnerability will be rewarded, and findings already discovered as part of a formal audit are ineligible.  
  
Vulnerabilities involving non-standard ERC20 tokens are also ineligible, as it would be trivial to insert an exploit into a token for the sake of applying to this bug bounty. A standard, Balancer-compatible ERC20 token is one that conforms to all [EIP-20 interfaces](https://eips.ethereum.org/EIPS/eip-20) _and_ exhibits expected behavior in implementation; i.e., transfers move exactly N tokens from sender to recipient, and balances do not change by any means other than transfers. Notably, tokens with transfer fees, rebasing supplies, or streaming mechanics are not compatible with Balancer, but that list is not exhaustive.
{% endhint %}

## Overview

Balancer has completed smart contract audits with Trail of Bits, OpenZeppelin, and Certora. We also will run a continuous bug bounty program for the V2 release of the Balancer core contracts.

## Scope

The bug bounty covers any of the core smart contracts deployed on Ethereum mainnet. The code can be found at: [https://github.com/balancer-labs/balancer-core-v2](https://github.com/balancer-labs/balancer-core-v2)

Submissions should be based off commit hash: [https://github.com/balancer-labs/balancer-core-v2/tree/v1.0.0](https://github.com/balancer-labs/balancer-core-v2/tree/v1.0.0)

Mainnet Vault can be found at: [https://etherscan.io/address/0xBA12222222228d8Ba445958a75a0704d566BF2C8](https://etherscan.io/address/0xBA12222222228d8Ba445958a75a0704d566BF2C8)

## Rewards

The bounty program will pay out rewards according to the severity of a vulnerability. See eligibility section below for more details. The final reward amount is at the sole discretion of Balancer Labs and will be paid in the specified sum of either USD or ETH, whichever amount is **more valuable**. In other words, the reward value increases with the price of ETH but can never fall below the given dollar amount.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Reward</th>
      <th style="text-align:left">Severity</th>
      <th style="text-align:left">Examples</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>1,000 ETH<br />or<br />$2,000,000</b>
      </td>
      <td style="text-align:left">Critical</td>
      <td style="text-align:left">
        <ul>
          <li>Draining significant funds from the Vault</li>
          <li>Permanently locking significant funds in the Vault</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>250 ETH<br />or<br />$500,000</b>
      </td>
      <td style="text-align:left">High</td>
      <td style="text-align:left">
        <ul>
          <li>Severe rounding errors where an attacker can steal funds in excess of
            any gas costs or swap fees</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>25 ETH<br />or<br />$50,000</b>
      </td>
      <td style="text-align:left">Medium</td>
      <td style="text-align:left">
        <ul>
          <li>Minor rounding errors that allow an attacker to slowly manipulate balances
            to their advantage</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>5 ETH<br />or<br />$10,000</b>
      </td>
      <td style="text-align:left">Low</td>
      <td style="text-align:left">
        <ul>
          <li>Informational and code quality based disclosures</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Reporting / Disclosures

Please report any findings to [security@balancer.finance](mailto:security@balancer.finance), with full details about any vulnerability and steps/code to reproduce. Allow us time to review and remediate any findings before public disclosure.

