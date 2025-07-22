## zap2xml.exe binary compatible with gracenote.com



#### Include

- zap2xml.zap2it.exe

  this is the original `zap2xml.exe` everyone is using now, dated ~2018, on `tvlistings.zap2it.com` and stops working as `zap2it.com` moved to new `gracenote.com`. There is work around to continue with this `exe`(or keep your old current `zap2xml.exe`) , following this ["Cache Spoofing](https://lucidusdev.github.io/2025/05/28/update-zap2xml-for-new-gracenote-com/#Cache-Spoofing)" guide.

- zap2xml.opt.exe

  This is my modified version, uses `tvlistings.gracenote.com` as drop-in replacement for current `zap2xml.exe`. A new `-H` option is also added for future domain change:

  ```
  zap2xml.exe -u user@email.com -p 1234 -H tvlistings.newweb.com ....
  ```

  And here is the detail about [patching the executable binary.](https://lucidusdev.github.io/2025/05/28/update-zap2xml-for-new-gracenote-com/#Patching-the-exe)

#### Update

Due to recent changes, some new options are added:

```
-H set domain
-h set user agent
-v set aid
```

