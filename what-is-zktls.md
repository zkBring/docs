# What is zkTLS?

## 🛡️ About zkTLS

zkTLS (Zero-Knowledge Transport Layer Security) is a new cryptographic protocol that allows users to **prove something about a webpage they visit—without revealing the actual content**. It's the foundation for secure, private web-based verification on zkBring.

***

### Why zkTLS matters

Most on-chain verifications today rely on centralized APIs, logins, or screenshots. zkTLS changes that:

* ✅ **Private** — no need to expose credentials or personal data
* ✅ **Secure** — built with cryptographic zero-knowledge proofs
* ✅ **Universal** — works with **any HTTPS website**
* ✅ **Local-first** — all verification happens in your browser
* ✅ **Composable** — webproofs can be verified by smart contracts like those on zkBring

With zkTLS, users stay in control of their data, while projects can onboard **real, verifiable users** from the broader web.

***

### zkTLS at zkBring

zkBring uses [**zkPass**](https://zkpass.org/) to power zkTLS verification.\
zkPass pioneered the concept of **zkTLS Webproofs**—a system that allows users to generate cryptographic proofs from any HTTPS website without exposing private information.

When a user begins verification:

1. The **zkPass TransGate extension** launches a secure browser session.
2. It connects to the website via TLS and locally intercepts the session data.
3. Instead of uploading anything, zkPass uses **MPC-TLS (Multi-Party Computation over TLS)** to decrypt and parse the session.
4. This parsed content is then passed into a **zero-knowledge circuit** that outputs a zkTLS proof.

> Everything is computed **locally in the browser**. No credentials, cookies, or personal content is ever exposed or shared.

**Key aspects of zkPass’s zkTLS architecture:**

* 🧠 **MPC-TLS Protocol** – decrypts TLS 1.3 in a trust-minimized way
* 🔐 **ZK Circuit Generation** – translates user-defined conditions into zero-knowledge logic
* 🌐 **Universal Web Support** – works with virtually any HTTPS site, no API access required
* 🛠️ **Proof Output** – a compact zk proof that can be verified on-chain by smart contracts (like zkBring)

This system lets zkBring support rich, flexible eligibility logic like:

> “Reddit user has 5+ karma,” or “Spotify user listened to a track,”\
> —without needing Reddit or Spotify to expose an API or user credentials.

***

### Learn more about zkTLS

* 🚀 [Crypto’s AirTag Moment: Unlocking Mass Adoption with Web Proofs (Nascent)](https://nascent.xyz/posts/web-proofs)
* 📖 [zkPass Technical Overview](https://zkpass.gitbook.io/zkpass/overview/technical-overview-v2.0)
* 🔬 [zkTLS Protocol Overview by zkPass](https://zkpass.gitbook.io/zkpass/overview/what-is-zktls)
* 📝 [Proving new worlds with zkTLS (Telah VC)](https://www.telah.vc/articles/proving-new-worlds-with-zktls)
* 🌐 [zkTLS: Building A Verifiable and Private Web (Oasis Protocol Blog)](https://oasisprotocol.org/blog/zktls-building-a-verifiable-and-private-web)
* 📌 [What is zkTLS? A Complete Guide to the Tech (Blocmates)](https://blocmates.com/blogmates/what-is-zktls-guide/)
* 🔑 [zkTLS Crypto Use Cases: Securing Decentralized Transactions (ZKON)](https://zkon.com/blog/zktls-crypto-use-cases)
* 💡 [Why zkTLS is an opportunity now (Mechanism Capital on ChainCatcher)](https://chaincatcher.com/zk-tls-opportunity-now/)
