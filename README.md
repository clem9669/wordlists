<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/clem9669/wordlists/">
    <img src="https://s.rfi.fr/media/display/f19b9c3c-1723-11ea-b771-005056bf7c53/w:310/p:16x9/dictionnaire_5_0.jpg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">French Wordlists</h3>

  <p align="center">
    Crack french people password
  </p>

> check out my hashcat rule project at: https://github.com/clem9669/hashcat-rule

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)

<!-- ABOUT THE PROJECT -->
## About The Project

It is easier to crack password for english people because it is le langue of internet. And there is good ressource as rockyou, hashorg2019, etc...

This project aim to provide french word list about everything a person could use as a base password.
If you are cracking with the list above, please also **use a rule in hashcat or john**.

I have already removed `œ,ï,ö,ä,ü,û,ô,î,â,ë,ù,µ` which are difficult to type chars even if they are present in french alphabet.

### Secondary

In the folder **WEB**, you can found a wordlist for pentesting purpose wich is design to find ressources for french people too. 
Read more at [WEB_readme](https://github.com/clem9669/wordlists/blob/master/Web/README.md)

### Built With
The main part of the list come from various place of internet but many thanks to :
* [Wikipedia](https://www.wikipedia.org/)
* [Grammalect](https://grammalecte.net/download.php?prj=fr)
* [SublimeText](https://www.sublimetext.com/)
* [Python](https://www.python.org/)

The keyboard walk are generated with https://github.com/hashcat/kwprocessor.

<!-- USAGE EXAMPLES -->
## Usage

I let the end user use at their will the lists. 
You could use only certains or all lists depending on your scope.
See the release section in github for a uniq version compiled.

```bash
awk '!a[$0]++' all > all_uniq
```

I recommand running hashcat rule on the wordlist then crack avoiding to have duplicate hash calculation (ex: password & password1 will be computed twice in hashcat with the rules.)

> **Warning**: the list sum is ~ 700'000 words.
> Multipled with the rule at https://github.com/clem9669/hashcat-rule (\~ 12'000), you have roughly 8'400'000'000 passwords.

The lists could have **duplicates** so do not forget to **deduplicate** before cracking. (https://stackoverflow.com/questions/9377040/remove-duplicate-entries-in-a-bash-script)

⚠️⚠️⚠️

I have recently heard of https://github.com/nil0x42/duplicut ! 

It aims to uniq huge wordlist ! I recommand you to give it a try.


The following projects could interest you:
  - https://github.com/mxrch/penglab: Abuse of Google Colab for Cracking
  - https://github.com/danielmiessler/SecLists/: Tons of Lists
  - https://github.com/hashcat/hashcat: Hashcat
  - https://github.com/openwall/john: John (jtr)
  - https://github.com/nil0x42/duplicut: Remove duplicates in huge lists

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/clem9669/wordlists/issues) for a list of proposed features (and known issues).

### If a wordlist is missing please raise an issue ! 

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
