<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/clem9669/wordlists/">
    <img src="https://s.rfi.fr/media/display/f19b9c3c-1723-11ea-b771-005056bf7c53/w:310/p:16x9/dictionnaire_5_0.jpg" alt="Logo" width="400" height="200">
  </a>

  <h3 align="center">French Wordlists</h3>

  <p align="center">
    Crack french people password
  </p>

> Check out my hashcat rule project at: https://github.com/clem9669/hashcat-rule

<!-- TABLE OF CONTENTS -->
## Table of Contents

[![Twitter-trends](https://github.com/clem9669/wordlists/actions/workflows/twitter.yml/badge.svg)](https://github.com/clem9669/wordlists/actions/workflows/twitter.yml)
[![Wordlist-news](https://github.com/clem9669/wordlists/actions/workflows/wordlist.yml/badge.svg)](https://github.com/clem9669/wordlists/actions/workflows/wordlist.yml)
[![Music-trends](https://github.com/clem9669/wordlists/actions/workflows/lastfm.yml/badge.svg)](https://github.com/clem9669/wordlists/actions/workflows/lastfm.yml)
[![Release](https://github.com/clem9669/wordlists/actions/workflows/release.yaml/badge.svg)](https://github.com/clem9669/wordlists/actions/workflows/release.yaml)

* [About the Project](#about-the-project)
  * [Downloads](#downloads)
  * [Web discovery](#web-discovery)
  * [Built with](#built-with)
* [Usage](#usage)
  * [Cracking contest](#cracking-contest)
* [Recommanded read](#recommanded-read)
* [Roadmap](#roadmap)
* [Contributing](#contributing)

<!-- ABOUT THE PROJECT -->
## About The Project


It is easier to crack password for english people because it is le langue of internet. And there is good resource as rockyou, hashorg2019, etc...

This project aim to provide french word list about everything a person could use as a base password.
If you are cracking with the list above, please also **use a rule in hashcat or john**.

I have already removed `œ,ï,ö,ä,ü,û,ô,î,â,ë` which are difficult to type chars even if they are present in french alphabet.

### Downloads

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/clem9669/wordlists?label=Release)](https://github.com/clem9669/wordlists/releases/)
![Github Repo size](https://img.shields.io/github/repo-size/clem9669/wordlists?label=Repo%20Size)

Because It might be simpler for you, I already compiled 3 differents versions of wordlists in the [Release](https://github.com/clem9669/wordlists/releases) section of Github

All details are there about wordlists combinaison.

*Update*: The clem9669_wordlist_large is too big for Github Actions. 
The current specs for Github Actions VM is 2-core CPU; 7 GB of RAM memory; 14 GB of SSD disk space.

### Web discovery

In the folder **WEB**, you can found a wordlist for pentesting purpose wich is design to find ressources for french people too. 

Read more at [WEB_readme](https://github.com/clem9669/wordlists/blob/master/Web/README.md)

### Built with
The main part of the list come from various places of internet but many thanks to :
* [Wikipedia](https://www.wikipedia.org/)
* [Grammalect](https://grammalecte.net/download.php?prj=fr)
* [SublimeText](https://www.sublimetext.com/)
* [weakpass.com](https://weakpass.com/)
* [hashes.org](https://hashes.org)
* [hashmob.net](https://hashmob.net)
* [packetstormsecurity.com](https://packetstormsecurity.com/Crackers/wordlists/)
* [danielmiessler/Seclists](https://github.com/danielmiessler/SecLists/)
* [scipag/password-list](https://github.com/scipag/password-list/)
* [xajkep/wordlists](https://github.com/xajkep/wordlists)
* [JustinApplegate/password-cracking](https://github.com/JustinApplegate/password-cracking)
* [Cheroxx/custom-wordlists](https://github.com/Cheroxx/custom-wordlists)
* [decal/werdlists](https://github.com/decal/werdlists)
* [wordlists.dev](https://www.wordlists.dev/)
* [sous-titres.eu](https://www.sous-titres.eu/)
* And more github wordlists ...

The keyboard walks are generated with [kwprocessor](https://github.com/hashcat/kwprocessor).

<!-- USAGE EXAMPLES -->
## Usage

I let the end user use at their will the lists. 
You could use only certains or all lists depending on your scope.
See the release section in github for a uniq version compiled.

```bash
LC_ALL=C.UTF-8; sort -u wordlist >> wordlist_uniq_sorted
```

> **Warning**: the lists can be very big!
> Multipled with the rule at https://github.com/clem9669/hashcat-rule

*N.B: I have recently heard of https://github.com/nil0x42/duplicut, it aims to uniq huge wordlist.*

### Cracking contest

This repo and the [rulelists](https://github.com/clem9669/hashcat-rule/) associated have been used for :
- [Korelogic Password Cracking contest](https://contest-2021.korelogic.com/) at Defcon 2021
- Cracking [haveibeenpwned.com](https://haveibeenpwned.com) by Troy Hunt NTLM releases 

## Recommanded read

The following projects could interest you:
  - [mxrch/penglab](https://github.com/mxrch/penglab): Abuse of Google Colab for Cracking
  - [hashcat/hashcat](https://github.com/hashcat/hashcat): Hashcat
  - [openwall/john](https://github.com/openwall/john): John (jtr)
  - [nil0x42/duplicut](https://github.com/nil0x42/duplicut): Remove duplicates in huge lists
  - [scip.ch/en/?labs.20210415](https://www.scip.ch/en/?labs.20210415): Analysis of Passwords (blog)
  - [crackstation.net/crackstation-wordlist-password-cracking-dictionary](https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm): CrackStation's wordlist
  - [hackingarticles.in/wordlists-for-pentester](https://www.hackingarticles.in/wordlists-for-pentester/): Wordlist guide
  - [Hashcat writeups](https://hashcat.net/events/): Contest writeups

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/clem9669/wordlists/issues) for a list of proposed features (and known issues).

### If a wordlist is missing please raise an issue ! 

<!-- CONTRIBUTING -->
## Contributing

Thanks to everyone in the password cracking scene for inspiration and lists ! 💪

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
