## Hi-OP 系统 自定义源码
```
sudo apt-get -y install build-essential asciidoc binutils bzip2 gawk gettext git libncurses5-dev libz-dev patch python3 python2.7 unzip zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs git-core gcc-multilib p7zip p7zip-full msmtp libssl-dev texinfo libglib2.0-dev xmlto qemu-utils upx libelf-dev autoconf automake libtool autopoint device-tree-compiler g++-multilib antlr3 gperf wget curl swig rsync qemu-utils android-sdk-ext4-utils
```
```bash
./scripts/feeds update -a
./scripts/feeds install -a
make

```
```
git add .
git commit -m "set some change by default"
git format-patch -s -1,2...

cat *.patch | patch -p1
```

