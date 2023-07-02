
# Building Kali using Ansible

**Make Sure to install Ansible using `pip` you can follow the steps [here](https://docs.ansible.com/ansible/2.9/installation_guide/intro_installation.html#installing-ansible-with-pip)**

## Instructions

- Start Kali Linux, on vmware or virtual box. 
- install Ansible using pip `pip3 install ansible`.
- Clone this repo to your kali linux `git clone`.
- change you current working directory inside `kali-build`.
- run `ansible-galaxy collection install community.general`.
- run `ansible-galaxy install -r requirements.yml --roles-path ./roles --force`.
- get sudo token `sudo whoami`.
- run `ansible-playbook -i inventory.yml main.yml`.

**Screenshot shows how the steps should look like**

![](attachments/Pasted%20image%2020230702173639.png)

## Tools & Features

By applying this REPO to your fresh Kali Linux, you will get following:
- Update & Upgrade Kali.
- Install needed tools:
	- ufw
	- xsel
	- xclip
	- zsh
	- jq
	- pipx
	- ntpdate
	- flameshot
	- exiftool
	- golang
	- rsyslog
	- auditd
- Configure-qterminal - xfce4 
- Configure-konsole - KDE5
- Configure tmux - User & Root
- Configure ZSH - User & Root
- Configure Firefox - addons and burp certificate
- Download & Build github tools:
	- Ruby gem packages:
		- logger
		- stringio
		- winrm
		- builder
		- erubi
		- gssapi
		- gyoku
		- httpclient
		- logging
		- little-plugger
		- nori
		- rubyntlm
		- winrm-fs
		- evil-winrm
	 * Build & install:
		 * Chisel
		 * Linpeas
		 * Winpeas
		 * Chainsaw
		 * Bloodhound
		 * Obsidian
		 * Kerbrute
	 * Python Tools:
		 * Impacket
		 * Crackmapexec
		 * certipy-ad
* Configure-Logging
* Install vscode & add customized settings.json

