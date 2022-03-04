# Ukraine Donation Roots

Collects all ETH+USDT transactions from the [Ukraine Donation Address](0x165cd37b4c644c2921454429e7f9358d18a45e14), parses dollar value (ETH = `$2,700`), and generates [merkle root](https://en.wikipedia.org/wiki/Merkle_tree) for use in an airdrop where $1 donated is equal to 1 ERC20 token.

**Config:**

1. Airdropped token has `18` decimals
2. If you had donated at least once before the [airdrop confirmation tweet](https://twitter.com/Ukraine/status/1498911922791583746?s=20&t=br4lOcrEzJT8dWKrdwuKFg), all your donations count as before the tweet
3. If you donated under $1 (for example, `0.045`), your donation is rounded up to a dollar

## Files

- `output/roots.json` — Merkle roots
- `output/airdrop-all.json` — All donators
- `output/airdrop-pre-announce.json` — All donators with _first_ donation before the [airdrop confirmation tweet](https://twitter.com/Ukraine/status/1498911922791583746?s=20&t=br4lOcrEzJT8dWKrdwuKFg)
