# My Mac Provisioning

## Installation

  1. [Install Ansible](http://docs.ansible.com/intro_installation.html).
  2. Ensure Apple's command line tools are installed (`xcode-select --install` to launch the installer).
  3. Clone this repository to your local drive.
  4. Run the command `$ ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
  5. Run `ansible-playbook main.yml -i inventory -u [username] -U [username] --ask-sudo-pass` from the same directory as this README file (substitute `[username]` for your macOS account username). Enter your account password when prompted.

## Testing the Playbook

Many people have asked me if I often wipe my entire workstation and start from scratch just to test changes to the playbook. Nope! Instead, I posted instructions for how I build a [Mac OS X VirtualBox VM](https://github.com/geerlingguy/mac-osx-virtualbox-vm), on which I can continually run and re-run this playbook to test changes and make sure things work correctly.
