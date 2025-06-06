---
title: Using Browser Extensions and NIP-07
---

# 🔌 Using Browser Extensions and NIP-07 Securely

## 📖 What is NIP-07?

**NIP-07** defines a standard that allows browser-based Nostr clients to **request cryptographic actions (like signing events)** from a browser extension — **without ever accessing your private key (`nsec`) directly**.

Think of it like **MetaMask for Nostr**: a secure layer between your identity and the app.

---

## 🔐 Why This Matters (Security & Privacy)

### 🚨 Risks of Pasting Your `nsec` into Browsers

- **Full access**: Any site where you paste your `nsec` can now fully control your identity.
- **Client compromise**: Even trusted sites can be hacked or serve compromised JavaScript.
- **Browser behavior**: Some browsers cache form inputs, which may store sensitive data unintentionally.
- **Extension leaks**: Malicious browser extensions or plugins could access clipboard or memory data.

> ⚠️ **TL;DR:** Pasting your private key into a browser is like typing your bank PIN into a public blog post.

---

## ✅ Safer Alternative: Use a NIP-07 Extension

NIP-07 extensions let web clients securely ask for signing without ever seeing your private key.

### 🧰 Examples of NIP-07-Compatible Extensions

| Extension       | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| **Nos2x**       | Most popular Nostr signing extension. Works seamlessly with many clients.  |
| **Alby**        | Originally for Lightning; now supports Nostr identity and zap integration.  |
| **Nostr Connect (WIP)** | Future option to delegate signing across devices securely.         |

---

## 🧭 Popular Clients Supporting NIP-07

| Client           | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Primal.net**   | Leading Nostr client with full-featured social experience and NIP-07 support. |
| **Snort.social** | Feature-rich web client built for speed and extensibility.                 |
| **Iris.to**      | Privacy-focused client with clean UI and progressive enhancements.         |
| **Coracle.social** | Lightweight, responsive client focused on performance.                   |
| **Nostr.band**   | Primarily an explorer, but supports write actions through NIP-07.          |

---

## 🔒 Summary

> Use **NIP-07** browser extensions like **Nos2x** to safely sign events in clients like **Primal**, **Snort**, or **Iris**, without ever exposing your private key.

Do **not** paste your `nsec` into browser fields — it’s a major security and privacy risk.

---

## 🔗 Related Pages

- [Protecting Your Private Key (`nsec`)](./protecting-your-nsec.md)
- [Best Practices for Nostr Security](../tips/best-practices.md)
- [Client Overview – Primal](../clients/primal.md)
