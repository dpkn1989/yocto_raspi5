# yocto_raspi5
Learning Yocto Linux on RaspberryPi5

All steps followed during the learning will be documented here
==============================================================

**************
08.03.2025
**************
Update the system -> sudo apt update
                     sudo apt upgrade -y
Install needed build utilities for Yocto -> sudo apt install -y gawk wget git-core diffstat unzip texinfo gcc build-essential \
                                            chrpath socat cpio python3 python3-pip python3-pexpect xz-utils debianutils \
                                            iputils-ping python3-git python3-jinja2 python3-subunit mesa-common-dev \
                                            zstd liblz4-tool
Clone poky -> cd yocto_raspi5
            git clone https://github.com/yoctoproject/poky.git
Move to scarthgap branch -> cd poky
                            git checkout scarthgap
Build Minimal image -> source oe-init-build-env           -> This creates environment for building and will navigate to build folder
                       bitbake core-image-minimal 

**************
09.03.2025
**************


