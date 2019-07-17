# IIS 8.5

This is my full bootstrapped Server 2012R2 VM that I use for sandbox testing, 
This Vagrant file and included scripts will:
* Setup WinRM listener and firewall rules
* Port Forward Guest 80,443 to local ports 8888, 8043
* Install Chocolatey
* Install / Update : PowerShell Core, PowerShell 5.1, NodeJS, VS-Code, Notepad++, Chrome, GIT, PuTTy, AWS PowerShell Module
* Setup a Test user "WMIUSER" with Read-only WinRM permissions to WMI / DCOM (related to prior permissions project)
* Install and Configure IIS
* Setup 5 IIS Test Sites with Self-Signed Certs
* Deploy Host File locally to point all test site references to loopback adapter


### Prerequisites

Built using virtualbox 6.0, vagrant 2.2.4, PowerShell 5.1

### Installing

* Install Vagrant
* Install Virtual Box
* From directory of Vagrantfile run "vagrant up"

## Built With

* [Vagrant](https://www.vagrantup.com/) - VM Orchestration
* [VirtualBox](https://www.virtualbox.org/) - Virtualization Provider
* [Chocolatey](https://chocolatey.org/) - Windows Package Management

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Thank you to anyone and their codes that was used to make this project