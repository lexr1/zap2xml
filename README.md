## zap2xml.exe compatible with gracenote.com



This is an updated version of zap2xml.exe. It's used to set TV Guide listing for [Windows Media Center](https://garyan2.github.io/win10.html). And follow [this excellent guide](https://sourceforge.net/p/epgcollector/discussion/1125945/thread/f5e3a54134/) to setup and use zap2xml.

- zap2xml.pl
  the original perl script for referenece.

- zap2xml2.pl

  my modified version support new greacenote.com listing and few extra options.

- zap2xml.exe
  compiled windows executable from the updated *zap2xml2.pl*, available in release.

  

#### What's new

Due to recent changes, some new options are added:

```
-H set domain(it's default tvlistings.gracenote.com but can be changed)
-h set user agent
-v set aid(as aid=____ in web url, default to 'orbebb')
```

Also change the default `sleeptime` , the delay between each http call to 0.5s. 

currently the compiled zap2xml.exe is a drop-in replacement of original zap2xml.exe.
