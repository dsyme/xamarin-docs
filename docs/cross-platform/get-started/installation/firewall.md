---
title: "Xamarin Firewall Configuration Instructions"
description: "A list of hosts that you need to whitelist in your firewall to allow Xamarin’s platform to work for your company."
ms.topic: article
ms.prod: xamarin
ms.assetid: 658f699b-8cca-48f7-ae54-fa956384b6d6
ms.technology: xamarin-cross-platform
author: asb3993
ms.author: amburns
ms.date: 12/02/2016
---

# Xamarin Firewall Configuration Instructions

_A list of hosts that you need to whitelist in your firewall to allow Xamarin’s platform to work for your company._

In order for Xamarin products to install and work properly, certain endpoints must be accessible to download the required tools and updates for your software. If you or your company have strict firewall settings, you may experience issues with installation, licensing, components, and more. This document outlines some of the known endpoints that need to be whitelisted in your firewall in order for Xamarin to work. This list does not include the endpoints required for any third-party tools included in the download. If you are still experiencing trouble after going through this list, refer to the Apple or Android installation troubleshooting guides.

## Endpoints to Whitelist

### Xamarin Installer

The following known addresses will need to be added in order for the software to install properly when using the latest release of the Xamarin installer:

-  xamarin.com (installer manifests)
-  dl.xamarin.com (Package download location)
-  dl.google.com (to download the Android SDK)
-  download.oracle.com (JDK)
-  visualstudio.com (Setup packages download location)
-  go.microsoft.com (Setup URL resolution)
-  aka.ms (Setup URL resolution)

If you are using a Mac and are encountering Xamarin.Android install issues, please ensure that macOS is able to download Java.


### Components Store and NuGet (including Xamarin.Forms)

The following addresses will need to be added to access the Xamarin Component Store
  or NuGet (Xamarin.Forms is packaged as a NuGet):

-  components.xamarin.com (to use Xamarin Components Store)
-  xampubdl.blob.core.windows.net (hosts Components Store downloads)
-  www.nuget.org (to access NuGet)
-  az320820.vo.msecnd.net (NuGet downloads)
-  dl-ssl.google.com (Google components)


### Software Updates

The following addresses will need to be added to ensure that software updates can download properly:

-  software.xamarin.com (updater service)
-  download.visualstudio.microsoft.com
-  dl.xamarin.com

### Xamarin Insights

The following addresses will need to be added to ensure that activity reaches the Xamarin Insights server:

* https://xaapi.xamarin.com


## Xamarin Mac Agent

To connect Visual Studio to a Mac build host using the Xamarin Mac Agent requires the SSH port to be open. By default this is **Port 22**.

## Summary

This guide covered the endpoints to whitelist to allow Xamarin products to install and update properly on your machine.