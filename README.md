![GitHub stars](https://img.shields.io/github/stars/ton-blockchain/mytonctrl?style=flat-square&logo=github) ![GitHub forks](https://img.shields.io/github/forks/ton-blockchain/mytonctrl?style=flat-square&logo=github) ![GitHub issues](https://img.shields.io/github/issues/ton-blockchain/mytonctrl?style=flat-square&logo=github) ![GitHub pull requests](https://img.shields.io/github/issues-pr/ton-blockchain/mytonctrl?style=flat-square&logo=github) ![GitHub last commit](https://img.shields.io/github/last-commit/ton-blockchain/mytonctrl?style=flat-square&logo=github) ![GitHub license](https://img.shields.io/github/license/ton-blockchain/mytonctrl?style=flat-square&logo=github)

<!-- omit from toc --> 

# MyTonCtrl

[Данный текст доступен на русском языке.](README.Ru.md)

<!-- omit from toc --> 

## Contents

- [What is MyTonCtrl?](#what-is-myttonctrl)
- [Functionality](#functionality)
    - [List of tested operating systems](#list-of-tested-operating-systems)
- [Installation](#installation)
    - [Installation scripts overview](#installation-scripts-overview)
    - [Installation modes](#installation-modes)
    - [Installation for Ubuntu](#installation-for-ubuntu)
    - [Installation for Debian](#installation-for-debian)
- [MyTonCtrl Documentation](#mytonctrl-documentation)
- [Telemetry](#telemetry)
- [MyTonCtrl installer mode](#mytonctrl-installer-mode)
    - [Web admin panel](#web-admin-panel)
    - [Local copy of toncenter](#local-copy-of-toncenter)
- [Useful links](#useful-links)

# What is MyTonCtrl?

MyTonCtrl is a console application that serves as a convenient wrapper for `fift`, `lite-client`,
and `validator-engine-console`. It has been specifically developed to streamline wallet, domain, and validator
management tasks on the Linux operating system.

![MyTonCtrl Status](screens/mytonctrl-status.png)

# Functionality

- [x] Show TON network status
- [x] Management of local wallets
    - [x] Create local wallet
    - [x] Activate local wallet
    - [x] Show local wallets
    - [x] Import wallet from file (.pk)
    - [x] Save wallet address to file (.addr)
    - [x] Delete local wallet
- [x] Show account status
    - [x] Show account balance
    - [x] Show account history
    - [x] Show account status from bookmarks
- [x] Transferring funds to the wallet
    - [x] Transfer of a fixed amount
    - [x] Transfer of the entire amount (all)
    - [x] Transfer of the entire amount with wallet deactivation (alld)
    - [x] Transferring funds to the wallet from bookmarks
    - [x] Transferring funds to a wallet through a chain of self-deleting wallets
- [x] Manage bookmarks
    - [x] Add account to bookmarks
    - [x] Show bookmarks
    - [x] Delete bookmark
- [x] Offer management
    - [x] Show offers
    - [x] Vote for the proposal
    - [x] Automatic voting for previously voted proposals
- [x] Domain management
    - [x] Rent a new domain
    - [x] Show rented domains
    - [x] Show domain status
    - [x] Delete domain
    - [ ] Automatic domain renewal
- [x] Controlling the validator
    - [x] Participate in the election of a validator
    - [x] Return bet + reward
    - [x] Autostart validator on abnormal termination (systemd)
    - [x] Send validator statistics to https://toncenter.com

## List of tested operating systems

| Operating System                   | Status                                     |
|------------------------------------|--------------------------------------------|
| Ubuntu 16.04 LTS (Xenial Xerus)    | Error: TON compilation error               |
| Ubuntu 18.04 LTS (Bionic Beaver)   | OK                                         |
| Ubuntu 20.04 LTS (Focal Fossa)     | OK                                         |
| Ubuntu 22.04 LTS (Jammy Jellyfish) | OK                                         |
| Debian 8                           | Error: Unable to locate package libgsl-dev |
| Debian 9                           | Error: TON compilation error               |
| Debian 10                          | OK                                         |

# Installation

Full installation manual can be found in the [official TON docs](http://docs.ton.org/participate/run-nodes/full-node).

## Web admin panel

To control the node/validator through the browser, you need to install an additional module:
`mytonctrl` -> `installer` -> `enable JR`

Next, you need to create a password for connection:
`mytonctrl` -> `installer` -> `setwebpass`

Ready. Now you can go to https://tonadmin.org site and log in with your credentials.
git: https://github.com/igroman787/mtc-jsonrpc

# Useful links

* https://docs.ton.org/
