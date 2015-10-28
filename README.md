# Wireshark Challenge - CTF

[![Build Status](https://img.shields.io/travis/aeibrahim/wireshark_challenge/master.svg?style=plastic)](https://travis-ci.org/aeibrahim/wireshark_challenge)
[![Project Status](https://img.shields.io/badge/status-complete-brightgreen.svg?style=plastic)](#)
[![Platform](https://img.shields.io/badge/platform-Ubuntu%2014%2B-lightgrey.svg?style=plastic)](#)
[![Apache](https://img.shields.io/badge/license-Apache-blue.svg?style=plastic)](https://www.gnu.org/licenses/gpl.html)


wireshark_challenge is a self-hosted packet analysis CTF built using CTFd on Ubuntu 14+. [CTFd](https://github.com/isislab/CTFd) is a web application for running a jeopardy style CTF created by [Kevin Chung](https://github.com/ColdHeat) of NYU's Information Systems and Internet Security Laboratory (ISIS Lab). 

This CTF consists of 8 challenges that involve analyzing pcap files and finding the flags. 

###Prerequisites

Ansible is required to use this repo. To install Ansible, see [here](https://docs.ansible.com/ansible/intro_installation.html#installing-the-control-machine).

###Usage
1. clone this repo: `git clone https://github.com/aeibrahim/wireshark_challenge`
2. add the IP address of your server to the file `inventory`
3. set desired options in `group_vars/all`
4. run the playbook: `ansible-playbook site.yml -i inventory -u <remote-user> -k -K`
5. visit ctfd's web interface via your browser: `http://<server's IP address>`
