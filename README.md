# LASalvador playbook configuration

## Getting ansible
[Download ansible here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html?extIdCarryOver=true&sc_cid=701f2000001OH7YAAW#installing-ansible-on-ubuntu)

## Pre running

*CHANGE THE VARIABLES IN THE PLAYBOOK.YML*
current_user = current user on machine (ex lucas)
os_release = "lsb_release -cs"

## Running
> sudo ansible-galaxy install gantsign.sdkman
> sudo ansible-galaxy install gantsign.oh-my-zsh
> sudo ansible-playbook -i host playbook.yml

## Post running

*First reopen the terminal*
### Install node and npm

> nvm install <node_version>

you can get the current node LTS version [here](https://nodejs.org/en/)

### Install java 
1. Getting the java versions availables
> sdk list java

2. Install java version
> sdk install java <java_version>

3. Define java home
> sdk home java <java_version>

4. Setup Jave default version
> sdk default java <java_version>


### Install maven 

Get the maven version [here](https://sdkman.io/sdks#maven)

> sdk install maven <mvn_version>

> sdk default maven <mvn_version>


