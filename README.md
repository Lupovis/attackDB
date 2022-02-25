# Attack Database

Database whith possible attacks and RegEx to match them with network traffic logs.\
Each entry is a yaml file with info about one specific attack.\
Use TEMPLATE.yaml file to create new entry.\
If unfamiliar with YAML use this [validator](http://www.yamllint.com/)
### DB entry file name
Naming rules to structure files and make them easier to find
| **Payload type** | **File name** | **Examples** |
| --- | --- | --- |
| Malware | malware_*<malware_name>*.yaml | malware_mirai.yaml ... |
| Attacks | attack_*<attack_name>*.yaml | attack_buffOverflow.yaml, attack_RCE.yaml, ... |
| Request | req_*<target>*.yaml | req_env_file.yaml, req_robots.yaml, req_HNAP1.yaml, ...
### DB entry template
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
### Future Improvements
- [ ] Write script to generate new entry
- [ ] Consider useful extra fields for entries
