# ossfs

ossfs is a fuse client to mount your [aliyun oss](http://oss.aliyun.com/) bucket under linux

## installation

packages for popular linux distributions are coming soon (or maybe not that soon)

## developer

ossfs is written in perl, please make sure these perl packages could be cound in your enviromnent:

- Fuse
- LWP::UserAgent
- HTTP::Date
- Digest::MD5
- Digest::HMAC_SHA1
- XML::Simple

the OSS.pm, delivered with ossfs, is a simple perl oss sdk module, which could be useful to perl coders. test.pl is a unittest script for this module.

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
