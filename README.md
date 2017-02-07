# Emotiv SDK - Community Edition

Here is the repository of the Emotiv SDK Community Edition, along with code examples and other development tools.
* Supports EPOC (over Emotiv USB dongle)
* Supports Insight and EPOC+ (over BTLE and Emotiv USB dongle)
* Supports Win32/64, Mac, iOS, Android, iOS, Ubuntu and Debian (armhf)

If you have questions or have knowledge to share, please visit our [forum](https://emotiv.com/forum/) which is the hub for our developer community.

To get the SDK you can either:
* Clone this repository with `git` command line tool or a GUI client like [SourceTree](https://www.sourcetreeapp.com); or
* Click on the "Download ZIP" button (above, on the right) to get the zip archive of the latest version; or
* Go to [releases](https://github.com/Emotiv/community-sdk/releases) and download the archive of a particular release

This repo contains SDK for Win32/64, Mac, iOS, Ubuntu and Debian (armhf).

Android SDK will be updated on [jcenter](https://bintray.com/nguoithichkhampha/maven/community) separately.

## Table of Contents
1. [Changelog](#changelog)
2. [Supported Platforms](#supported-platforms)
3. [Connecting with BTLE](#connecting-with-btle)
4. [API Documentation](#api-documentation)
5. [API Code Example](#api-code-example)
6. [Apps and Tools](#apps-and-tools)
7. [Support](#support)

## Changelog
See [changelog](CHANGELOG.md)

## Supported Platforms
* Insight with Bluetooth SMART (Bluetooth 4.0 or Bluetooth Low Energy) connection currently works with the SDK under:
  * Windows 8 or above
  * Windows 7, **only with Bluetooth adaptor that uses Broadcom BCM20702 chipset**
    (recommended one: Plugable USB 2.0 Bluetooth Adapter, http://plugable.com/products/usb-bt4le)
  * Mac OS X 10.10 or above (check if Bluetooth LMP Version is 0x6 from System Report)
  * iOS 8.0 or above (excluding iOS 8.3 and 8.4)
  * Android 4.4.3 or above (excluding Android 5.0)
  * Ubuntu 14.04 / 15.10 64-bit (see [Connecting on Ubuntu and Debian](doc/Connecting on Ubuntu and Debian.md))
  * Debian 8.3 Jessie (armhf) (see [Connecting on Ubuntu and Debian](doc/Connecting on Ubuntu and Debian.md))

* Insight with Emotiv Universal USB Receiver currently works with the SDK under:
  * Windows 7 or above
  * Mac OS X 10.8 or above
  * Android 4.4.3 or above
  * Ubuntu 14.04 / 15.10 64-bit
  * Debian 8.3 Jessie (armhf)

## Connecting with BTLE
* Windows: Turn on Bluetooth on both Insight and PC, then pair your Insight with Windows built-in Bluetooth service first
* Mac, Android and iOS: Turn on Bluetooth on both Insight and Mac/Android device, then start Emotiv app to use (without first pairing)
* Ubuntu and Debian: See [Connecting on Ubuntu and Debian](doc/Connecting on Ubuntu and Debian.md)

## API Documentation
http://emotiv.github.io/community-sdk/

## API Code Example

Have 2 groups of examples :
 * Examples which could run without SDK license are placed inside folder **examples_basic**
 * Examples which need to have SDK license to run are placed inside folder **examples_extra_prime**

Table below describe examples indetail :

| Name  | Could run without license |Available with language|
|---|---|---|
| AverageBandPowers | Yes | C++, C#, Java, Python |
| EmoStateLogger | Yes | C++, C#, Java, Python|
| FacialExpressionDemo | Yes | C++, Matlab, Android, Mac |
| GyroData | Yes | C++ |
| HeadsetInformationLogger | Yes | C++, C#, Java, Python |
| MentalCommandDemo | Yes | C++, Android, Mac |
| MentalCommandWithCloudProfile | Yes | C++, C#, Java, Python, Android |
| MentalCommandWithLocalProfile | Yes | C++ |
| MotionDataLogger | Yes | C++, C#, Java, Python, Android, iOS, Mac |
| MultiDongleConnection | Yes | C++, C#, Python |
| SavingAndLoadingProfileCloud | Yes | C++, C#, Java, Python, iOS, Mac |
| FFTSample  | Yes | Android, iOS, Mac |
| RollingBall  | Yes | Unity |
| ActivateLicense  | No | C++, C#, Java, Python |
| EEGLogger  | No | C++, C#, Java, Python, Matlab |
| MultiDongleEEGLogger  | No | C++ |
| MultilChannelEEGLogger  | No | C++ |
| PerformanceMetricsDemo  | No | C++, C# |

## Apps and Tools

#### Xavier EmoComposer
 * [Xavier Composer](tools) allows you to send user-defined EmoStates to Emotiv SDK, Xavier EmoKey, or any other application that makes use of the Emotiv API, and simulate the events that could be sent from Emotiv SDK with a real device.
 * Available for Windows 7 or above and Mac OS X 10.8 or above

#### Xavier EmoKey
 * [Xavier EmoKey](tools) translates Emotiv detection results to predefined sequences of keystrokes according to logical rules defined by the user.
 * Available for Windows 7 or above and Mac OS X 10.8 or above

#### CPanel
A web-based Emotiv Control Panel:

https://cpanel.emotivinsight.com

Compatible with Insight / EPOC / EPOC+ via:
* BTLE:
  * Windows 8 or above, with Firefox 43.0
  * Mac OS X 10.10 or above, with Safari 9.0 / Firefox 43.0 / Opera 34.0
* [Emotiv USB Universal Receiver](https://emotiv.com/store/product_9.html):
  * Windows 7 or above, with Firefox 43.0
  * Mac OS X 10.8 or above, with Safari 9.0 / Firefox 43.0 / Opera 34.0

Please follow the instructions to install the Emotiv browser plugin before using the CPanel.

#### Insight App for Android
Requires Android 4.4.3 or later

https://play.google.com/store/apps/details?id=com.emotiv.insightapp

#### Insight App for iOS
Requires iOS 8.0 or later, **excluding iOS 8.3/8.4 due to BTLE data transmission limitation in those versions**

https://itunes.apple.com/us/app/emotiv-insight/id1031805596

## Support

Please check out the topic **Insight** on **Emotiv Help Centre**:

https://emotiv.zendesk.com/hc/en-us/categories/200100495-Insight

Our knowledge base is a good source for further reading:

https://emotiv.zendesk.com/hc/en-us
 
Please also visit our [forum](https://emotiv.com/forum/) for bug reports and feature requests.

Happy coding!

The Emotiv Team
