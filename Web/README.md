> check out my hashcat rule project at: https://github.com/clem9669/hashcat-rule

<!-- ABOUT THE PROJECT -->
## About The Project

While pentesting it is sometime hard to find a good worldlist to run with *dirb, wfuzz, gobuster, ffuf and others*.

This project aims to give a good and complete wordlist for discovery (including French words). Put extensions accordingly to your webapp.

For extensions file, I recommand the [Raft file extensions](https://github.com/danielmiessler/SecLists/tree/master/Discovery/Web-Content).

I have removed weird and "difficult" to type letter:
```sh
sed -i '/ï/d' decouverte.txt
sed -i '/ö/d' decouverte.txt
sed -i '/ä/d' decouverte.txt
sed -i '/ü/d' decouverte.txt
sed -i '/û/d' decouverte.txt
sed -i '/ô/d' decouverte.txt
sed -i '/î/d' decouverte.txt
sed -i '/â/d' decouverte.txt
sed -i '/â/d' decouverte.txt
sed -i '/ê/d' decouverte.txt
sed -i '/é/d' decouverte.txt
sed -i '/è/d' decouverte.txt
sed -i '/ë/d' decouverte.txt
sed -i '/ù/d' decouverte.txt
sed -i '/µ/d' decouverte.txt
```

The size of the wordlist is about:
```sh
wc -l decouverte.txt 
331570 decouverte.txt
```

### Built With
The main part of the list come from various place of internet but many thanks to :
* Dirbuster: directory-list-2.3-medium.txt
* Dirb lists: common + large
* Seclist > Discovery > Web-content: Raft
* French dictionnary
* API routes & scraps

The following projects could interest you:
  - https://github.com/nil0x42/duplicut
  - https://github.com/fuzzdb-project/fuzzdb
  - https://github.com/danielmiessler/SecLists
  - https://github.com/swisskyrepo/PayloadsAllTheThings
  - https://wordlists.assetnote.io/
  - https://github.com/clem9669/hashcat-rule


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
