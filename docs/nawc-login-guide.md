# Logging into Websites with Your Nostr Account 🔑

You can now use your **Nostr identity** to log into websites — no email, no password required.

This method is called **NAWC**, short for **Nostr Auth with Capability**. It’s a way for websites to verify *you are you* by asking your Nostr client or extension to cryptographically sign a message — just like making a post or a zap.

---

## 🧠 Why Use Nostr for Login?

- ✅ No accounts to create  
- ✅ No passwords to remember  
- ✅ You stay in control of your identity  
- ✅ No third-party logins or platform lock-in

With NAWC, your `npub` (public key) becomes your **universal login**.

---

## 🧰 What You Need

To log into sites using NAWC, you’ll need one of the following **Nostr signing tools**:

| Tool         | Type        | Notes                                      |
|--------------|-------------|--------------------------------------------|
| **Alby**     | Browser extension | Popular, integrates with Lightning & Nostr |
| **Nos2x**    | Browser extension | Lightweight Nostr signer for logins      |
| **NsecBunker** | Remote signer    | Great for mobile or secure setups        |

These tools manage your keys **securely** and let you sign login requests without copying/pasting anything.

---

## 🚫 Why You Should **Not Paste Your `nsec`** Into Sites or Apps

Your `nsec` is your **private key** — it controls your Nostr identity. Anyone who has it can post, zap, or impersonate you.

### Copy-pasting your `nsec` is risky because:

- The site might **store or steal** your key
- You might accidentally paste it in the wrong place (like a public post)
- Some fake “Nostr apps” are built just to collect `nsec`s

Instead, always use a **signing extension** like Alby, Nos2x, or a remote signer like NsecBunker. These tools sign messages **without exposing your private key** to any site.

> 🔐 Rule of thumb: If a site asks you to paste your `nsec`, **don’t trust it.**

---

## 🚀 How It Works (Simplified)

1. You visit a website that supports **Nostr login**
2. The site asks your browser to “sign in with Nostr”
3. Your Nostr signing tool (like Alby) asks you to approve
4. Once you sign, the site knows it's really *you* (your `npub`)

No passwords. No accounts. Just one identity you own across the web.

---

## 🔄 Using Different `nsec`s (Switching Identities)

You can log into websites using **different Nostr accounts** if you want to keep certain activities or identities separate.

How to switch depends on the signing tool:

### If you're using **Alby**:
- Click the Alby extension in your browser
- Go to **Settings → Nostr** and paste a different `nsec`
- Save and refresh the login page  
> Tip: Back up each `nsec` before switching!

### If you're using **Nos2x**:
- Click the Nos2x icon and paste a different `nsec`
- It will remember the new identity for future logins

### If you're using **NsecBunker**:
- Set up multiple identities on the backend
- Switch between them via the UI or parameter in the login URL

> Just remember: **each identity is completely separate** — followers, notes, zaps won’t carry over unless you migrate them manually.

---

## 🔐 Is This Secure?

Yes — as long as you protect your private key. Signing tools like Alby or Nos2x never expose your key to websites — they just verify your identity on your behalf.

Always check the site before signing anything. If in doubt, don’t sign.

---

## 🧭 Where Can I Try This?

- [nsec.app](https://nsec.app)  
- [nostrudel.ninja](https://nostrudel.ninja)  
- Some Nostr-based app dashboards, forums, or profile pages

More sites are adding support for Nostr login every week.

---

## 🙋‍♀️ FAQ

### Can I use this on mobile?

Yes, but you'll likely need a mobile-compatible signer like **NsecBunker** or a browser extension that works on mobile (if available).

---

### What happens if I lose access to my key?

You won’t be able to log into sites using that Nostr identity anymore — this is why **backing up your `nsec`** is critical.

---

### Can someone else log in as me?

Only if they have your **private key (`nsec`)**. Never share it. Use password managers or trusted extensions to manage it safely.

---

## ✅ Summary

- NAWC lets you log into websites using your Nostr account
- You keep your keys — sites just ask for a cryptographic signature
- Signing tools like Alby or Nos2x make this process secure and simple

This is one more step toward a **decentralized internet where you own your identity**.
