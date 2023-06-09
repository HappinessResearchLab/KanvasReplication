# KanvasReplication (CVE-9J75-75999)

<p align="center">
<img width="320" height="168" src="https://github.com/HappinessResearchLab/KanvasReplication/blob/main/images/kanvasreplication_logo.png?raw=true">
</p>

<table align="center">
<tr>
<td>CVE:</td>
<td>CVE-9J75-75999</td>
</tr>
<tr>
<td>CVSS v3.1:</td>
<td><a href=https://www.first.org/cvss/calculator/3.1#CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H>10/10 (Critical)</a></td>
</tr>
<tr>
<td>Authors:</td>
<td><a href=https://github.com/Rambo6Glaz>Rambo6Glaz</a></td>
</tr>
<tr>
<td>Reported:</td>
<td>September 13rd, 2007 (Ramona Kavas) <br> July 26th, 2022 (Mariko)  </td>
</tr>
<tr>
<td>Disclosed:</td>
<td>September 19th, 2022 (RendezVous)</td>
</tr>
</table>

### Technical details

This repository contains a PoC that exploits this vulnerability to perform the following operations:

- Send a RDV payload that is stored in the remote console stack. Part of the payload is used to overwrite the return address of the function, making the game execute the elf immediately. The PoC only implements sending payloads of 0x75 bytes.

**NOTE:** The PoC requires an old version of Daphne that implements MARIKO communications

## Credits
While this vulnerability was discovered by multiple users independently, many of them decided to keep the vulnerability information private. However, the folowing people are responsible for safely disclosing the vulnerability to Erista:
- Rambo6Glaz ([GitHub](https://github.com/Rambo6Glaz))

## License
<p xmlns:dct="http://purl.org/dc/terms/" xmlns:vcard="http://www.w3.org/2001/vcard-rdf/3.0#">
  <a rel="license"
     href="http://creativecommons.org/publicdomain/zero/1.0/">
    <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <a rel="dct:publisher"
     href="https://github.com/HappinessResearchLab/HappinessResearchLab">
    <span property="dct:title">Rambo6Glaz</span></a>
  has waived all copyright and related or neighboring rights to
  <span property="dct:title">KanvasReplication</span>.
<br>
This work is published from:
<span property="vcard:Country" datatype="dct:ISO3166"
      content="RO" about="https://github.com/HappinessResearchLab/HappinessResearchLab">
  Romania</span>.
</p>