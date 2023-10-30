---
title: "Passwords"
date: 2023-10-19T20:21:07+08:00
draft: false
---

# Passwords, Passphrases, Strength of passwords, etc.

### Secure Passwords

A secure password is one that is difficult for an adversary to guess, whether by brute force, educated speculation, or specific knowledge.

Security through obscurity is only as secure as it is obscure, and will only remain obscure for a finite period. It is far better to have a password that is mathematically secure even when the adversary knows exactly how you made it.

Now, for a list of things *not* to do:

Don't use duplicate passwords. If you do, no matter how strong the password, as soon as one account with the password is cracked, all of you accounts with that password are.

Second, use a password (or passphrase) of sufficient lenght or complexity to be mathematically difficult to crack.

Complexity requirements for passwords are bad. They make the password less secure in some ways, because there are parameters that the adversary knows to refine their search, but more importantly, it is more difficult for the user, which means the user will likely do other bad things to circumvent it such as reusing the same password or storing it in an insecure location.

Do not use any personally identifiable info in your password, such as birthdays, pets names, or anything else somebody could find on facebook or other places where a threat actor could obtain information on the internet.

Really, you should not use anything at all for a password that is not randomly generated. Anything that is not, such as regular english phrases, things you come up with in your head, or the items that happen to be on your desk, have patterns and lead to weaker passwords. A randomly generated password has no such patterns. It does have patterns, but for well-known methods those patterns have been determined and added to the process of calculating their security. A known is far better than an unknown in this scenario.

Now how would I know what mathematically complicated is?

Well, it's complicated. ;P

log(2)N is the equation to calculate entropy or randomness (for our purposes here, it's acutally a bit more complicated). This assumes brute force guessing. For an all-lowercase alphabet only password, 

```N=26^l```

where **l*** is the number of characters in the password.
So if we have a 10-character password, N will equal 

```26x26x26x26x26x26x26x26x26x26```

Entering that into our equation, 
```log base 2 of (1.4e14) EDIT```,
we get an entropy value of 47 bits.

This is not a secure password. As of 2023, 90 bits is considered pretty secure. To up the entropy of our password, we can add length (more from our alphabet or character set) or complexity (add more characters to our character set). [Add more examples of better passwords, with the maths. Maybe also add built-in calculator?] This is where the idea of a *passphrase* comes in. Instead of a string of characters, a passphrase is a string of words, such as *correct horse battery staple*. Diceware-style passphrases do both. Diceware uses a set of 7776 words to make a passphrase from. This is as if our alphabet is now 7776 words long. Much better than 26. And if someone assumed we were using the 26 letter alphabet character set (with spaces) then we have lenght too. We can also add a number or symbol to the start or end of one of our words for added complexity


did3o(*d0fds0*0073 vs *correct horse battery staple*
xkcd 936
How passphrase with wordlist is still secure and better than random

#### Password vs Passphrase



*Links*

[useapassphrase.com](https://www.useapassphrase.com)

[xkcd 936](https://xkcd.com/936/)

[Don't pass on the new NIST password guidelines](https://auth0.com/blog/dont-pass-on-the-new-nist-password-guidelines/)

[Diceware](https://theworld.com/~reinhold/diceware.html)

[EFF Dice-Generated Passphrase](https://www.eff.org/dice)

### Password Managers

	- Online passsword managers

		[Bitwarden](https://bitwarden.com)

		A FOSS password manager. Can be self-hosted if desired. Free and premium tiers.

		[1Password](https://1password.com) 

		Not FOSS, but has regular audits and works closely with password cracking community. In this respect it is better than Bitwarden. Starts at $4 a month, no free tier.

	- [KeePass](https://keepass.info) (FOSS, A file format, compatible with many clients)

		[KeePass XC](https://keepassxc.org/) Windows/macOS/Linux (free)

		[KeePass DX](https://www.keepassdx.com/) Android (free)

		[KeePassium iOS](https://keepassium.com/) (paid)


[Don't](https://palant.info/2022/12/26/whats-in-a-pr-statement-lastpass-breach-explained/) use [LastPass](https://infosec.exchange/@epixoip/109585049354200263).

Evaluate password managers based on their handling of sensitive data, transparency with regular third-party audits, cryptography, and competency in response to security incidents when they happen.

Some information, and pros/cons of using them (and why it is worth it to do so).

[EFF](https://ssd.eff.org/module/animated-overview-using-password-managers-stay-safe-online)

[https://lock.cmpxchg8b.com/passmgrs.html](https://lock.cmpxchg8b.com/passmgrs.html)


