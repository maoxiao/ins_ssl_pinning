
# ins_ssl_pinning


[Instagram V78](https://www.apkmirror.com/apk/instagram/instagram-instagram/instagram-instagram-78-0-0-11-104-139906-release/)

This is inspired by [Instagram_SSL_Pinning](https://github.com/pouyadarabi/Instagram_SSL_Pinning) and [How to bypass Instagram SSL Pinning on Android](https://plainsec.org/how-to-bypass-instagram-ssl-pinning-on-android-v78/)

Make sure you have a rooted android device

### steps
* pick your apk here [Instagram](https://www.apkmirror.com/apk/instagram/instagram-instagram/instagram-instagram-78-0-0-11-104-139906-release/) (check your device via `adb shell getprop ro.product.cpu.abi`)
* open Instagram app on your device, make sure `/data/data/com.instagram.android/lib-zstd/libliger.so` exists
* download related __.so__ file from current [repo](https://github.com/maoxiao/ins_ssl_pinning)
* run `adb push libliger.so /data/data/com.instagram.android/lib-zstd/libliger.so`
* setup Burp Suite (please use latest [jdk](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html) to run Burp Suite  `java -jar burpsuite_community.jar`) to intercept requests

