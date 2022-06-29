# PSAM16
# Methodology and Demonstration of Git-Based Configuration Control in Probabilistic Risk Assessment

this Git repository is for the development of a Git-Based Configuration Control PRA tools
The requirements for Configuration Control, under the ASME/ANS RA-S-1.4 Standard, is to be followed
this repo will include the documentation for version control of SAPHIRE models, similar approach can be used for other PRA tools.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Windows OS (for running SAPHIRE codes only)
- Git

### Installing

#### Installing Git
```
download the latest Git version compabtible with you operating system from https://git-scm.com/
```

#### Creating a branch in the Git repository
```
from Issues --> New issue --> add issue title and description --> submit issue --> create merge request
```

#### Cloning the repository
- Open the command prompt (Win) or terminal (Mac) and write the following commands in it
```
mkdir develop     #create a directory for cloning the repository
cd develop        #accessing the directory
git init          #initialize git in the directory
```
- then clone the repository
```
git remote add origin https://github.com/mostafa-hamza/PSAM16.git
git fetch origin
```
- then move into the branch created from the issue
```
git checkout <branch-name>
```

#### opening SAPHIRE Models
```
open new project named UPDATED 
choose the path ..\develop\models\<model name>\src\
from file --> load/extract
from load --> open
navigate to ..\develop\models\<model name>\src\<model name>\MARD\<model name>.MARD
choose process -if prompt error appeared press no-
```
#### saving SAPHIRE Models
```
from file --> load/extract
from extract --> All project items --> mark --> process
close SAPHIRE
navigate to ..\develop\models\
delete <model name> directory
rename the UPDATED directory to <model name>
```
#### pushing updates to the Git repo
- Open the command prompt (Win) or terminal (Mac) and write the following commands in it
```
git add .                                                           #add all untracked changes
git commit -m "write what changes are made to this push"            #commit all updates with the appropriate comment
git push                                                            #push all changes to the remote Git repo
```
## Authors

Mostafa Hamza

## Acknowledgments

* Mihai Diaconeasa
* Alp Tezbasaran
