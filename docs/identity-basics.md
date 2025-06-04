# Nostr Identity Basics 🔐

### Your Keys = Your Identity

Nostr uses public-key cryptography for identity. No accounts, no logins.

| Term    | What it is                                | Like...                     |
|---------|--------------------------------------------|-----------------------------|
| `npub`  | Your public Nostr identity                 | A social media @handle      |
| `nsec`  | Your private key — keep it secret          | Your password + seed phrase |
| `pubkey`| Raw version of your npub (hex format)      | Account number              |
| `nip-05`| Optional human-readable name (`you@site`)  | Display name or email-like  |

---

Your `nsec` is powerful: **anyone who has it can post as you.**  
Store it like a wallet key — ideally in a password manager or on paper (not a screenshot).

You can use a `nip-05` identifier to appear more human-readable. For example:  
`npub1xyz...` → `you@nostrplebs.com`

> Want to try using Nostr? [Start here →](getting-started.md)
