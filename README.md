dev-env
=======

Customized puphpet to create development environment
Config was generated on https://puphpet.com/

#Steps:
- Install Vagrant - https://www.vagrantup.com/downloads
- Install Packer - http://www.packer.io/intro/getting-started/next.html
- Download puphpet box templates - https://github.com/osvarychevskyi/packer-templates
- Go to the directory of the box config
- Edit template.json to have more space on disc(by default 50GB disc).
- Build your box:

    $ packer build template.json

- Add box to vagrant

    $ vagrant box add ubuntu1404-x64-50gb packer_virtualbox-iso_virtualbox.box

- Go to dev-env folder

    $ vagrant up
