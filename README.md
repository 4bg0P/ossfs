###**_IMPORTANT NOTE_**
**This repository is to be considered _DEPRECATED_ and all efforts are going towards developing the next version of the platform in [aliyun/ossfs](https://github.com/aliyun/ossfs).**

# ossfs

ossfs is a fuse client to mount your [aliyun oss](http://oss.aliyun.com/) bucket under linux.

## installation

### archlinux

run `makepkg` in distro/archlinux, and `pacmann -U ossfs-git-*.pkg.tar.xfz` to install

### ubuntu

make sure at least dependencies are installed:
- libhttp-date-perl
- libfuse-perl
- libxml-simple-perl
- libdigest-hmac-perl

## developer

ossfs is written in perl, please make sure these perl packages could be cound in your enviromnent:

- Fuse
- LWP::UserAgent
- HTTP::Date
- Digest::MD5
- Digest::HMAC_SHA1
- XML::Simple

the OSS.pm, delivered with ossfs, is a simple perl oss sdk module, which could be useful to perl coders. test.pl is a unittest script for this module.

## road map

- review code of rmdir and see if recursively remove object is needed
- optimize memory usage when writing big files
- make OSS.pm a CPAN module
- OSS.pm support multiple part upload
- <del>basic read/write</del>

## reference

- [perl Fuse module](http://search.cpan.org/~dpavlin/Fuse-0.14/Fuse.pm)
- [fuse documentation](http://fuse.sourceforge.net/doxygen/structfuse__operations.html#dc6dc71274f185de72217e38d62142c4)
- [post on aliyun official forum](http://bbs.aliyun.com/read.php?tid=132627)

## author

Li Ruibo
- http://twitter.com/lymanrb
- http://weibo.com/lymanrb

## licence

licensed under the [BSD License](http://www.linfo.org/bsdlicense.html)
