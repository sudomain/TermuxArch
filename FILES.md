# FILES.md
files and directories used in TermuxArch
## Directories
### .conf
Contains VERSIONID number, outdated in the SDRausty/TermuxArch repo but up to date in TermuxArch/TermuxArch repo
### .git
standard git repo information
### .github
github .yml files
### .scripts
#### ./scripts/do.sums.bash
creates and checks the sha512.sum file (a checksum) then commits with the current time in epoch seconds (then `git push`es)
#### ./scripts/tgen.bash
creates setupTermuxArch.tar.gz by moving base level bash scripts to gen/ and performing sha512sum on them. Calls do.sums.bash and vgen.sh
TODO: Also does `cp setupTermuxArch.bash setupTermuxArch.sh`, find out the purpose of this
#### ./scripts/vgen.sh
increments the ./conf/VERSIONID number. It must be only used in the TermuxArch/TermuxArch repo because it's outdated in the SDRausty/TermuxArch repo
### gen
an empty directory that ./scripts/tgen.bash uses to bundle the base level scripts into a tar.gz file and checksums
## Files
### .gitignore
tells git to ignore setupTermuxArchConfigs.bash which is an auto generated file
### .gitpod.Dockerfile
### .gitpod.yml
### 404.md
### CHANGE.log
### CONTRIBUTORS.md
### LICENSE
### NOTICE.md
### README.md
### archlinuxconfig.bash

### do.sums.bash
### espritfunctions.bash
### getimagefunctions.bash
### gsa.bash
### init.sh
### knownconfigurations.bash
### maintenanceroutines.bash
### necessaryfunctions.bash
### printoutstatements.bash
### pullTermuxArchSubmodules.sh
### robots.txt
### setupTermuxArch.bash
### setupTermuxArch.sh
### setupTermuxArch.sha512
### setupTermuxArch.tar.gz
### setupTermuxArchConfigs.bash
### sha512.sum
### sitemap.txt
### tgen.bash

