# MagPro Android

Releases of the MagPro Android app (APK). Nothing else lives here.

Install it from the `/download` page of your company's MagPro site, for example
`https://zaki.eworkspace.net/download`. That page always serves the latest release.

To publish a build made on EAS (`eas build --platform android --profile apk`):

```sh
gh workflow run publish.yml --repo suplibio/magpro-android \
  -f apk_url=<APK URL from the EAS build page> -f tag=v<version>-<versionCode> -f title="MagPro <version> (<versionCode>)"
```
