# Attack Database

Database whith possible attacks and RegEx to match them with network traffic logs.\
Each entry is a yaml file with info about one specific attack.\
Use TEMPLATE.yaml file to create new entry.\
If unfamiliar with YAML use this [validator](http://www.yamllint.com/)
### DB entry structure
```yaml
name: <Attack Name>
description: <Brief description of the attack and its goal>
usefulLinks:
    - <link1>
    - <link2>
CVEs:
    - <CVE1> - <cve.org link1>
    - <CVE2> - <cve.org link1>
RegEx:
    - <regEx1>
    - <regEx2>
```
### Improvements
- [ ] Write script to generate new entry
- [ ] Consider useful extra fields for entries
