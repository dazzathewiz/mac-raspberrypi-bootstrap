# mac-raspberrypi-bootstrap

1. Run `ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
2. Run `ansible-playbook main.yml --ask-become-pass` inside this directory. Enter your macOS account password when prompted for the 'BECOME' password.

Use balena-cli: https://forums.balena.io/t/command-line-option/7171 
balena local flash /Users/dazzathewiz/Downloads/DietPi_RPi-ARMv6-Bullseye/DietPi_RPi-ARMv6-Bullseye.img