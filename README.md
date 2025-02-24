# ubuntu_myppa_test
ubuntu_myppa_test is the source code of testing ubuntu PPA.
It is based on a existed debain package(Bluez).

## Introduction

#### Download the source code of that Debian package

'apt source Bluez' is used to get the source code of Bluez debian package.

#### Modification information

On the basis of Bluez Debian package source code, the following modification
have been mode:

'usr/local/bin/testing.sh' is added to print test information.

'debian/hellotest.install' is added to copy testing.sh to '/usr/bin'
in the process of installing hellotest package.

'debian/hellotest.postinst' is added to print test information in the process
of installing hellotest package.

'debian/control' is modified to add hellotest package.

'debian/changelog' is modified to add the new version information of Bluez.
