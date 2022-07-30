# mac-raspberrypi-bootstrap

Ansible playbook to programatically image an SD card (bootstrap) with DietPi (https://dietpi.com/) on Mac. Simply configures basic DietPi options in files/dietpi/dietpi.txt. You don't necessarily need to run this playbook and could simply use https://www.balena.io/etcher/ to flash the image and copy dietpi.txt onto the imaged SD. However I may use this in future for other raspberry pi distributions.

Note: the playbook ensure homebrew is installed on the Mac to manage packages.


## Installation

    1. Run `ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
    2. Run `ansible-playbook main.yml --ask-become-pass` inside this directory. Enter your macOS account password when prompted for the 'BECOME' password.


## Configuratio Defaults

defaults.config.yml contains the settings variables for bootstrapping.
files/dietpi/dietpi.txt contains dietpi autosetup configuration, see: https://dietpi.com/docs/usage/#how-to-do-an-automatic-base-installation-at-first-boot-dietpi-automation


References used in development:
https://github.com/geerlingguy/mac-dev-playbook
https://galaxy.ansible.com/geerlingguy/mac
https://formulae.brew.sh/formula/balena-cli
https://github.com/balena-io/balena-cli
https://forums.balena.io/t/command-line-option/7171/8

