The GPL source is created for ASUS wireless router related products. Please visit the ASUS support site (http://support.asus.com) to get the latest GPL tarball.It has a lot in common with many wireless router open source projects, including Oleg/Tomato/DD-WRT/OpenWRT. Thanks the developers of those projects for making the source code available.

Set Up Environment(Tested in Fedora 8/9 and Ubuntu)
    1. prepare environment
	Ubuntu
	Install the following packages
	sudo apt-get install libncurses5 libncurses5-dev m4 bison gawk flex libstdc++6-4.4-dev g++-4.4 g++ gengetopt \
	git zlib1g-dev autoconf autopoint libtool shtool autogen mtd-utils intltool sharutils docbook-xsl-* libstdc++5 \
	texinfo dos2unix xsltproc uboot-mkimage device-tree-compiler qemu gperf liblzo2-dev uuid-dev build-essential \
	lzma-dev liblzma-dev lzma binutils-dev patch cmake intltool libglib2.0-dev gtk-doc-tools

	If you are using Ubuntu amd64, you may need to install 32-bit packages listed below.
	sudo apt-get install libc6-i386 lib32stdc++6 lib32z1 libelf1:i386 libncurses5:i386 ia32-libs libc6-dev-i386

   2. prepare source to, ex, $HOME/asuswrt

   3. setup development system
	please check /opt/toolchains/ delete all file under it, please all the file under this directory

   4. build firmware.
	[rt-ac86u]
		cd release/src-rt-5.02hnd
		make rt-ac86u
