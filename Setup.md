Welcome to the hackathon002 wiki!

# Setup a build environment

Install VirtualBox (TODO link)

Make a new folder somewhere

    brew cask install vagrant
    vagrant init hashicorp/precise64
    vagrant up
    vagrant ssh

Now, inside the VM:

    sudo apt-get install -y clang git build-essential tcl
    git clone https://github.com/antirez/redis
    cd redis

Now build the project using clang static analyzer:

    scan-build make -j
    make test


