Install VirtualBox (TODO link)

Make a new folder somewhere: 

    git clone git@github.com:returntocorp-hackathon/hackathon002.git
    cd hackathon002

Now setup the VM:

    brew cask install vagrant
    vagrant up
    vagrant ssh

Now, inside the VM:

    git clone https://github.com/<REPO YOU ARE WORKING ON>
    cd <NAME OF PROJECT>

Now build the project using clang static analyzer:

    scan-build -o /vagrant_data/scan make

If your project has tests:

    make test


