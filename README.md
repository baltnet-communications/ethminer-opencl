# About This Project
This project packages famous [ethminer](https://github.com/ethereum-mining/ethminer) into easily distributable Debian package. This helps to maintain and update the binary.

# Building the Package
1. After cloning the repository, run `git submodule update --init --recursive` to check out all git sub-modules.
2. To update change log file, run `dch -i` and make the edits.
3. Prior building the release, run `dch -r` to update change log for release procedure.
4. For debug builds, execute `dpkg-buildpackage -uc -us` which avoids signing changes and source artifacts.
5. For release builds, run `dpkg-buildpackage` without any arguments.

# Installation
Please visit http://pkg.baltnet.net for instructions how to configure Baltnet repository. To install the package, run following command:

```
	$ sudo apt install ethminer-opencl
```

# Configuration
There is no default working configuration which a daemon can use. Therefore, a custom configuration must be created manually after installation.
