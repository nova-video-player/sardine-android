# sardine-android

[![Build Status](https://github.com/nova-video-player/sardine-android/actions/workflows/android.yml/badge.svg)](https://github.com/nova-video-player/sardine-android/actions/workflows/android.yml)
[![Version number](https://jitpack.io/v/nova-video-player/sardine-android.svg) ](https://jitpack.io/#nova-video-player/sardine-android)

A WebDAV client for Android, using [OkHttp](https://github.com/square/okhttp) as HTTP client.

This is a fork of [TheGrizzyLabs'](https://github.com/thegrizzlylabs/sardine-android) sardine-android. It seems unmaintained now, but thanks for the fish!

## Getting started

- Edit your app-level `build.gradle` (see top of this page for the latest version):

```

repositories {
  ...
  maven { url 'https://jitpack.io' }
}

dependencies {
  ...
  implementation 'com.github.thegrizzlylabs:sardine-android:<VERSION_NUMBER>'
}
```

- Create a `Sardine` client:
```
Sardine sardine = new OkHttpSardine();
sardine.setCredentials("username", "password");
```

- Use the client to make requests to your WebDAV server:
```
List<DavResource> resources = sardine.list("http://webdav.server.com");
```

## Legacy

Originally forked from [Sardine](https://github.com/lookfirst/sardine)

[Apache HTTP Client](http://hc.apache.org/) was replaced by [OkHttp](https://github.com/square/okhttp)

JAXB was replaced by [SimpleXml](http://simple.sourceforge.net/)

## Alternatives
See [Awesome WebDAV: Java libraries](https://github.com/WebDAVDevs/awesome-webdav/blob/main/readme.md#java)
