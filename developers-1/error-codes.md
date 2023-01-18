---
description: >-
  Vault exceptions will revert with "BAL#" instead of text; see below for the
  interpretation of the number.
---

# Error Codes

All error codes for the Balancer V2 core contracts are defined in the [`BalancerErrors`](https://github.com/balancer-labs/balancer-core-v2/blob/master/contracts/lib/helpers/BalancerErrors.sol) contract.

## Math

| Code | Error | Comment |
| :--- | :--- | :--- |
| 0 | ADD\_OVERFLOW |  |
| 1 | SUB\_OVERFLOW |  |
| 2 | SUB\_UNDERFLOW |  |
| 3 | MUL\_OVERFLOW |  |
| 4 | ZERO\_DIVISION |  |
| 5 | DIV\_INTERNAL |  |
| 6 | X\_OUT\_OF\_BOUNDS |  |
| 7 | Y\_OUT\_OF\_BOUNDS |  |
| 8 | PRODUCT\_OUT\_OF\_BOUNDS |  |
| 9 | INVALID\_EXPONENT |  |

## Input

| Code | Error | Comment |
| :--- | :--- | :--- |
| 100 | OUT\_OF\_BOUNDS |  |
| 101 | UNSORTED\_ARRAY |  |
| 102 | UNSORTED\_TOKENS |  |
| 103 | INPUT\_LENGTH\_MISMATCH |  |
| 104 | ZERO\_TOKEN |  |

## Shared pools

| Code | Error | Comment |
| :--- | :--- | :--- |
| 200 | MIN\_TOKENS |  |
| 201 | MAX\_TOKENS |  |
| 202 | MAX\_SWAP\_FEE\_PERCENTAGE |  |
| 203 | MIN\_SWAP\_FEE\_PERCENTAGE |  |
| 204 | MINIMUM\_BPT |  |
| 205 | CALLER\_NOT\_VAULT |  |
| 206 | UNINITIALIZED |  |
| 207 | BPT\_IN\_MAX\_AMOUNT |  |
| 208 | BPT\_OUT\_MIN\_AMOUNT |  |
| 209 | EXPIRED\_PERMIT |  |

## Pools

| Code | Error | Comment |
| :--- | :--- | :--- |
| 300 | MIN\_AMP |  |
| 301 | MAX\_AMP |  |
| 302 | MIN\_WEIGHT |  |
| 303 | MAX\_STABLE\_TOKENS |  |
| 304 | MAX\_IN\_RATIO |  |
| 305 | MAX\_OUT\_RATIO |  |
| 306 | MIN\_BPT\_IN\_FOR\_TOKEN\_OUT |  |
| 307 | MAX\_OUT\_BPT\_FOR\_TOKEN\_IN |  |
| 308 | NORMALIZED\_WEIGHT\_INVARIANT |  |
| 309 | INVALID\_TOKEN |  |
| 310 | UNHANDLED\_JOIN\_KIND |  |
| 311 | ZERO\_INVARIANT |  |

## Lib

| Code | Error | Comment |
| :--- | :--- | :--- |
| 400 | REENTRANCY |  |
| 401 | SENDER\_NOT\_ALLOWED |  |
| 402 | PAUSED |  |
| 403 | PAUSE\_WINDOW\_EXPIRED |  |
| 404 | MAX\_PAUSE\_WINDOW\_DURATION |  |
| 405 | MAX\_BUFFER\_PERIOD\_DURATION |  |
| 406 | INSUFFICIENT\_BALANCE |  |
| 407 | INSUFFICIENT\_ALLOWANCE |  |
| 408 | ERC20\_TRANSFER\_FROM\_ZERO\_ADDRESS |  |
| 409 | ERC20\_TRANSFER\_TO\_ZERO\_ADDRESS |  |
| 410 | ERC20\_MINT\_TO\_ZERO\_ADDRESS |  |
| 411 | ERC20\_BURN\_FROM\_ZERO\_ADDRESS |  |
| 412 | ERC20\_APPROVE\_FROM\_ZERO\_ADDRESS |  |
| 413 | ERC20\_APPROVE\_TO\_ZERO\_ADDRESS |  |
| 414 | ERC20\_TRANSFER\_EXCEEDS\_ALLOWANCE |  |
| 415 | ERC20\_DECREASED\_ALLOWANCE\_BELOW\_ZERO |  |
| 416 | ERC20\_TRANSFER\_EXCEEDS\_BALANCE |  |
| 417 | ERC20\_BURN\_EXCEEDS\_ALLOWANCE |  |
| 418 | SAFE\_ERC20\_CALL\_FAILED |  |
| 419 | ADDRESS\_INSUFFICIENT\_BALANCE |  |
| 420 | ADDRESS\_CANNOT\_SEND\_VALUE |  |
| 421 | SAFE\_CAST\_VALUE\_CANT\_FIT\_INT256 |  |
| 422 | GRANT\_SENDER\_NOT\_ADMIN |  |
| 423 | REVOKE\_SENDER\_NOT\_ADMIN |  |
| 424 | RENOUNCE\_SENDER\_NOT\_ALLOWED |  |
| 425 | BUFFER\_PERIOD\_EXPIRED |  |

## Vault

| Code | Error | Comment |
| :--- | :--- | :--- |
| 500 | INVALID\_POOL\_ID |  |
| 501 | CALLER\_NOT\_POOL |  |
| 502 | SENDER\_NOT\_ASSET\_MANAGER |  |
| 503 | USER\_DOESNT\_ALLOW\_RELAYER |  |
| 504 | INVALID\_SIGNATURE |  |
| 505 | EXIT\_BELOW\_MIN |  |
| 506 | JOIN\_ABOVE\_MAX |  |
| 507 | SWAP\_LIMIT |  |
| 508 | SWAP\_DEADLINE |  |
| 509 | CANNOT\_SWAP\_SAME\_TOKEN |  |
| 510 | UNKNOWN\_AMOUNT\_IN\_FIRST\_SWAP |  |
| 511 | MALCONSTRUCTED\_MULTIHOP\_SWAP |  |
| 512 | INTERNAL\_BALANCE\_OVERFLOW |  |
| 513 | INSUFFICIENT\_INTERNAL\_BALANCE |  |
| 514 | INVALID\_ETH\_INTERNAL\_BALANCE |  |
| 515 | INVALID\_POST\_LOAN\_BALANCE |  |
| 516 | INSUFFICIENT\_ETH |  |
| 517 | UNALLOCATED\_ETH |  |
| 518 | ETH\_TRANSFER |  |
| 519 | CANNOT\_USE\_ETH\_SENTINEL |  |
| 520 | TOKENS\_MISMATCH |  |
| 521 | TOKEN\_NOT\_REGISTERED |  |
| 522 | TOKEN\_ALREADY\_REGISTERED |  |
| 523 | TOKENS\_ALREADY\_SET |  |
| 524 | TOKENS\_LENGTH\_MUST\_BE\_2 |  |
| 525 | NONZERO\_TOKEN\_BALANCE |  |
| 526 | BALANCE\_TOTAL\_OVERFLOW |  |

## Fees

| Code | Error | Comment |
| :--- | :--- | :--- |
| 600 | SWAP\_FEE\_PERCENTAGE\_TOO\_HIGH |  |
| 601 | FLASH\_LOAN\_FEE\_PERCENTAGE\_TOO\_HIGH |  |
| 602 | INSUFFICIENT\_FLASH\_LOAN\_FEE\_AMOUNT |  |

