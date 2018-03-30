# vagrant-hardenedbsd-rust: a Vagrant box for building Rust binaries for HardenedBSD

# WARNING

This box is likely to break as HardenedBSD breaks ABI with FreeBSD, unless someone begins maintaining a dedicated HardenedBSD target for rustup.

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-hardenedbsd-rust

# EXAMPLE

```console
$ cd test
$ vagrant up
$ vagrant ssh -c "cd /vagrant && rustc hello.rs && ./hello"
Hello World!
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-hardenedbsd-rust.box
```
