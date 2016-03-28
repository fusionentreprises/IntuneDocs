---
title: Windows 10 configuration policy settings in Microsoft Intune
ms.custom: na
ms.reviewer: na
ms.service: microsoft-intune
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 00a602d9-b339-4fd8-ab70-defbf6686855
author: robstackmsft
---
# Windows 10 configuration policy settings in Microsoft Intune
Use the Microsoft **general configuration policy** for Windows 10 to configure settings for enrolled Windows 10 desktop, and Windows 10 Mobile devices:



## Password

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Require a password to unlock devices**|Require a password on supported devices.|Yes|Yes|
|**Required password type**|Specifies the type of password that will be required, such as numeric only, or alphanumeric|Yes|Yes|
|**Required password type** - **Minimum number of character sets**|There are four character sets, lowercase letters, uppercase letters, numbers, and symbols. This setting specifies how many different character sets must be included in the password.|Yes|Yes|
|**Minimum password length**|Specifies the minimum number of characters the device password must contain.|No|Yes|
|**Number of repeated sign-in failures to allow before the device is wiped**|Wipes the device if this number of login attempts fail.|Yes|Yes|
|**Minutes of inactivity before screen turns off**|Specifies the length of time a device must be idle before the screen is locked.|Yes|Yes|
|**Password expiration (days)**|Specifies the length of time after which the device password must be changed.|Yes|Yes|
|**Remember password history**|Specifies whether you want to restrict the end user from creating previously used passwords.|Yes|Yes|
|**Remember password history** - **Prevent reuse of previous passwords**|Specifies the number off previously used passwords remembered by the device.|Yes|Yes|
|**Allow picture password and PIN**|Lets you use simple gestures on a picture, or a simple PIN to login.|Yes|No|
|**Require a password when the device returns from an idle state**|If enabled, the user must enter a password to unlock the device from an idle state.|No|Yes|

## Encryption

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Require encryption on mobile device**|Enables encryption on targeted devices.|No|Yes|

## System

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow screen capture**|Let's the user capture the device screen as an image.|No|Yes|
|**Allow manual unenrollment**|Lets the user manually delete the workplace account from the device.|Yes|Yes|
|**Allow manual root certificate installation**|Specifies whether the user can manually install root certificates|No|Yes|
|**Allow diagnostic and usage data to be sent to Microsoft**|Determines the amount of diagnostic and usage data that is sent to Microsoft from devices.<br>**No** - No data is sent to Microsoft<br>**Basic** - The device sends only limited information to Microsoft<br>**Enhanced** - Sends enhanced diagnostic data to Microsoft<br>**Full (recommended)** - Sends the same data as **Enhanced**, plus additional data about the device state|Yes|Yes|


## Account and synchronization

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow Microsoft account**|Lets the user associate a Microsoft account with the device.|Yes|Yes|
|**Allow adding non-Microsoft accounts manually**|Lets the user add email accounts to the device that are not associated with a Microsoft account.|Yes|Yes|
|**Allow settings synchronization for Microsoft accounts**|Allow device and app settings associated with a Microsoft account to synchronize between devices.|Yes|Yes|

## Email settings

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Make Microsoft account optional in Windows Mail application**|Configure this to remove the requirement for a Microsoft account in Windows Mail.|Yes|No|



## Microsoft Edge

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow web browser**|Allow the use of the Edge web browser on the device.|No|Yes|
|**Allow search suggestions in address bar**|Lets your search engine suggest sites as you type search phrases.|Yes|Yes|
|**Allow sending intranet traffic to Internet Explorer**|Lets users open intranet websites in Internet Explorer.|Yes|No|
|**Allow do not track**|Configures the Edge browser to send do not track headers to websites that users visit.|Yes|Yes|
|**Enable SmartScreen**|Enables the SmartScreen browser setting on devices.|Yes|Yes|
|**Allow active scripting**|Allows scripts, like Javascript to be run in the Edge browser.|Yes|Yes|
|**Allow pop-ups**|Enables or disables the browser pop-up blocker.|Yes|No|
|**Allow cookies**|Allow or disable cookies.|Yes|Yes|
|**Allow Autofill**|Allow users to change autocomplete settings in the browser.|Yes|No|
|**Allow Password Manager**|Enable or disable the Edge Password Manager feature.|Yes|Yes|
|**Enterprise Mode site list location**|Specifies where to find the list of web sites that will open in Enterprise mode. Users cannot edit this list.|Yes|No|

### Apps

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow application store**|Allow the user to access the app store on the device.|No|Yes|



## Cellular

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow data roaming**|Allow roaming between networks when accessing data.|Yes|Yes|
|**Allow VPN over cellular**|Controls whether the device can access VPN connections when connected to a cellular network.|Yes|Yes|
|**Allow VPN roaming over cellular**|Controls whether the device can access VPN connections when roaming on a cellular network.|Yes|Yes|

## Hardware

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow camera**|Specifies whether the device camera can be used.|Yes|Yes|
|**Allow removable storage**|Specifies whether external storage devices such as an SD card can be used with the device.|Yes|Yes|
|**Allow Wi-Fi**|Allows the use of the devices Wi-Fi capability.|No|Yes|
|**Allow internet sharing**|Allow the use of Internet connection sharing on the device.|Yes|Yes|
|**Allow manual Wi-Fi configuration**|Controls whether the user can configure their own Wi-Fi connections, or whether they can only use connections configured by a Wi-Fi profile.|No|Yes|
|**Allow automatic connection to free Wi-Fi hotspots**|Lets the device automatically connect to free Wi-Fi hotspots and automatically accept any terms and conditions for the connection.|Yes|Yes|
|**Allow geolocation**|Specifies whether the device can use location services information.|Yes|Yes|
|**Allow NFC**|Allows the device to use it's Near Field Communications capabilities.|Yes|Yes|
|**Allow Bluetooth**|Enables the use of Bluetooth capabilities on the device.|Yes|Yes|
|**Allow Bluetooth discoverable mode**|Let's this device be discovered by other Bluetooth-enabled devices.|Yes|Yes|
|**Allow Bluetooth advertising**|Allows devices to receive advertisements over Bluetooth.|Yes|Yes|
|**Allow Bluetooth connectable mode** **Important:** |This setting is no longer supported by Windows 10 and will be removed in the future.|Yes|Yes|
|**Allow phone reset**|Controls whether the user can factory reset their device.|Yes|Yes|
|**Allow USB connection**|Controls whether devices can access external storage devices through a USB connection.|Yes|Yes|
|**Allow AntiTheft mode**|Configure whether Windows Antitheft mode is enabled.|Yes|Yes|

## Features

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|----------------------|---------------------|
|**Allow copy and paste**|Enable or disable the use of copy and paste on the device.|No|Yes|
|**Allow voice recording**|Enable or disable the voice recording features on the device.|No|Yes|
|**Allow Cortana**|Enable or disable the Cortana voice assistant.|Yes|Yes|
|**Allow action center notifications**|Enable or disable action center notifications on the device lock screen.|No|Yes|

## Defender

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|-|-|
|**Allow real-time monitoring**|Enables real-time scanning for malware, spyware, and other unwanted software.|Yes|No|
|**Allow behavior monitoring**|Lets Defender check for certain known patterns of suspicious activity on devices.|Yes|No
|**Enable Network Inspection System**|The Network Inspection System (NIS) helps to protect devices against network-based exploits by using the signatures of known vulnerabilities from the Microsoft Endpoint Protection Center to help detect and block malicious traffic.|Yes|No
|**Scan all downloads**|Controls whether Defender scans all files downloaded from the Internet.|Yes|No
|**Allow script scanning**|Lets Defender scan scripts that are used in Internet Explorer.|Yes|No
|**Monitor file and program activity**|Enable this setting to allow Defender to monitor file and program activity on devices.|Yes|No
|**Days to track resolved malware**|Lets Defender continue to track resolved malware for the number of days you specify so that you can manually check previously affected devices. If you set the number of days to **0**, malware remains in the Quarantine folder and is not automatically removed. |Yes|No
|**Allow client UI access**|Controls whether the Windows Defender user interface is hidden from end users.<br>When this setting is changed, it will take effect the next time the end user's PC is restarted.|Yes|No
|**Schedule a daily quick scan**|Lets you schedule a quick scan that occurs daily at the time you select.|Yes|No
|**Schedule a system scan**|Lets you schedule a full or quick system scan that occurs regularly on the day and time you select.|Yes|No
|**Limit CPU usage during a scan**|Lets you limit the amount of CPU that scans are allowed to use (from **1** to **100**)|Yes|No
|**Scan archive files**|Allows Defender to scan archived files such as Zip or Cab files.|Yes|No
|**Scan email messages**|Allows Defender to scan email messages as they arrive on the device.|Yes|No
|**Scan removable drives**|Lets Defender scan removable drives like USB sticks.|Yes|No
|**Scan mapped network drives**|Lets Defender scan files on mapped network drive.<br>If the files on the drive are read-only, Defender will be unable to remove any malware found in them.|Yes|No
|**Scan files opened from network shared folders**|Lets Defender scan files on shared network drives (for instance, those accessed from a UNC path.<br>If the files on the drive are read-only, Defender will be unable to remove any malware found in them.|Yes|No
|**Signature update interval**|Specify the interval at which Defender will check for new signature files.|Yes|No
|**Allow cloud protection**|Allow or block the Microsoft Active Protection Service from receiving information about malware activity from devices you manage. This information is used to improve the service in the future.|Yes|No
|**Prompt users for samples submission**|Controls whether files that might require further analysis by Microsoft to determine if they are malicious are automatically sent to Microsoft.|Yes|No
|**Files and folders to exclude when running a scan or using real-time protection**|Add one or more files and folders like **C:\Path** or **%ProgramFiles%\Path\filename.exe** to the exclusions list. These files and folders will not be included in any real-time, or scheduled scans.|Yes|No
|**File extensions to exclude when running a scan or using real-time protection**|Add one or more file extensions like **jpg** or **txt** to the exclusions list. Any files with these extensions will not be included in any real-time, or scheduled scans.|Yes|No
|**Processes to exclude when running a scan or using real-time protection**|Add one or more processes of the type **.exe**, **.com**, or **.scr** to the exclusions list. These processes will not be included in any real-time, or scheduled scans.|Yes|No| 


## Updates settings

|Setting name|Details|Windows 10 Desktop|Windows 10 Mobile|
|----------------|---------------|----------------------|---------------------|
|**Allow automatic updates**|Enable this setting to allow automatic updates. Then, configure one of the following settings to control update behavior:<br /><br />**Notify download**<br /><br />**Auto install at maintenance time**<br /><br />**Auto install and reboot at maintenance time**<br /><br />**Auto install and reboot at scheduled time** **Note:** When this option is selected, you can also configure the following settings:  **Suppress notification to end user** and **Define install day for scheduled updates**.|Yes|No|



### See Also
[Manage settings and features on your devices with Microsoft Intune policies](manage-settings-and-features-on-your-devices-with-microsoft-intune-policies.md)
