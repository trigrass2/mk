## build a Machinkekit jessie 4GB USB stick

```bash
$ sudo apt-get -y install grml-debootstrap apt-cacher
```
```bash
$ sudo vi /etc/apt-cacher/apt-cacher.conf
```
uncomment
```
#allowed_hosts = *
```
next, build and run machinekit-jessie.img:
```bash
$ time sh x &> stick-jessie.log
$ sh y # run in qemu
```