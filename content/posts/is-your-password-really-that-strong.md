---
title: "Is Your Password Really That Strong?"
date: 2021-11-30T16:49:55+01:00
draft: false
mathjax: true
---

The latest **NordPass** "most breached password" of 2021, is a list of 200 most common passwords directly taken from
data breaches and databases of more than *270.000.000 passwords*:

1. *123456*
2. *123456789*
3. *12345*
4. *qwerty*
5. *password*

These are the first 5, and if they don't surprise you, well, **they don't surprise anyone either**. Why then everybody use them?

*Because they are easy to remember*, you would say.

**Yes**, it has to do with that, but also to the fact that the majority of people surfing the web and using webapps are drawn to do that.
Of course we are not talking about building *stupid password rules* (the more password rules a system has, the easier it will be to crack them),
but about the real human nature of not caring about a risk as long as "it's not mine".

However, this is not the topic of this article. So, **"how can I know if my password is strong enough?"** is an excellent question.
The answer to that will be given in a moment, but first we need to set-up some *basic knowledge* about entropy and password security!

## Password Strength and Entropy

Password strength measures the risk of having a certain password **brute-forced** (a process of guessing it trial-by-trial): for this measure to be
as complete as possible we have to keep in mind factors like the use of **numbers, letters, symbols, etc...**.
These factors are counted with a score function that uses *Entropy* bits as the output that we analyze. **Entropy measures how unpredictable a password is**.
This strange measure is just a $log_2$ of the number of all possible passwords, if we assume that every symbol is produced independently.

Thus, the Entropy E for a password of length L is: $$E=L\cdot log_2(R)$$ where $R$ is the size of the *pool* of characters the password exists in.

## What pool are we talking about?

Let's now define a *pool* for commonly used characters for making a password:

| Pool                    | Elements | Pool size | Notes |
| -----:                  | :------  | :-------: | :---- |
| Lowercase latin letters | [a-z]    |    26     |       |
| Uppercase latin letters | [A-Z]    |    26     |       |
| Digits                  | [0-9]    |    10     |       |
| Symbols                 | \`~!@#$%^&*()-=_+[{]}\|;' :",.<>/? | 33 | Whitespace is included |

Now, using the pool and the formula we are able to extract the Entropy from those common *bad passwords*!
We will rank the good/bad password considering the fact that a password that has an Entropy of 19 bits is as strong as
19 bits that are chosen randomly, like in a fair coin toss. This password with an Entropy of 19 bits will require $2^{42}$
brute-force attempts: so, stronger passwords have more Entropy bits (easy peasy!).

Good passwords generally have more than **120 bits of Entropy**, but excellent passwords (like long Diceware passwords), can have
a lot of bits and be easily remembered!

## Examples

| Password    | Entropy    | Is it good?  (>120)  |
|---------------- | --------------- | --------------- |
| 123456    | 19.93    | No    |
| password   | 37.60    | No    |
| ThisPasswordIsSafe1212  | 130.99   | Yes   |
| PasLapq@aop%gvf9mw%*Y#rz87rPEr!aFX8LG&b | 256.22 | Yes, but.. |
| SpyglassPushoverMuskinessSuspendShareCertified | 262.22 | Awesome, a Diceware! |

As you can see from this list we have a note to make about 3 things:

* You can have an excellent password **without adding numbers or special characters**!
* Machine generated passwords are *not* harder to hack as you can see, but surely **impossible to remember**...
* **Character repetition is bad** for your passwords, even if it has an high Entropy.

## Conclusion and acknowledgements

Knowing that you should follow best-practices to avoid making weak passwords (and now you know how!) the biggest
*vulnerability* here is represented by humans and their ability not to leak those password via phishing
or just having that password in a clear file on the desktop (and that, my friends, happens a lot).

If you want to know the Entropy of your passwords without inputting them online you can use [this](https://github.com/grtcdr/paspio) *free and open source* tool.
Then, I still consider **Diceware** passwords to be the best at the job, and you can create them [here](https://diceware.dmuth.org/) or in your password manager (mine is **Bitwarden**)!

Thanks for reading!

*Author: Federico "EvilScript" Torrielli*
