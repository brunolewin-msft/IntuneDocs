---
# required metadata
title: What's new in Microsoft Intune
titleSuffix: "Intune on Azure"
description: Find out what's new in the Intune Azure portal
keywords:
author: brenduns  
ms.author: brenduns
manager: angrobe
ms.date: 07/25/2017
ms.topic: get-started-article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 791ed23f-bd13-4ef0-a3dd-cd2d7332c5cc

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer:
ms.suite: ems
#ms.tgt_pltfrm:
ms.custom: intune-azure
---

# What's new in Microsoft Intune

[!INCLUDE[azure_portal](./includes/azure_portal.md)]

Learn what’s new each week in Microsoft Intune. You can also find out about [upcoming changes](#whats-coming), [important notices](#notices) about the service, and information about [past releases](whats-new-archive.md).

> [!Note]
> Many of these features will eventually be supported for hybrid deployments with Configuration Manager. For more information about new hybrid features, check out our [hybrid What’s New page](/sccm/mdm/understand/whats-new-in-hybrid-mobile-device-management).


<!-- Common categories:  
  ### Role-based access control
  ### Device enrollment
  ### Device management
  ### App management
  ### Device configuration
-->   

## Week of July 23rd, 2017

### Light and dark modes available for the Company Portal app for Windows 10 <!---676547--->
End users will be able to customize the color mode for the Company Portal app for Windows 10. The user is able to make the change in the Settings section of the Company Portal app. The change will appear after the user has restarted the app. For Windows 10 version 1607 and later, the app mode will default to the system setting. For Windows 10 version 1511 and earlier, the app mode will default to the light mode.

### Enable end users to tag their device group in the Company Portal app for Windows 10 <!---807046-->
End users are now able to select which group their device belongs to by tagging it directly from within the Company Portal app for Windows 10.

## Week of June 26th, 2017

### Role-based access control
#### New role-based administration access for Intune admins   <!-- 1099990 -->  
A new conditional access admin role is being added to view, create, modify, and delete Azure AD Conditional Access policies. Previously, only global admins and security admins had this permission. Intune admins can be granted with this role permission so that they have access to conditional access policies.


### Device enrollment
#### Tag corporate-owned devices with serial number <!-- 1215070 -->  
Intune now supports uploading iOS, macOS, and Android serial numbers as Corporate Device Identifiers. You can't use serial numbers to block personal devices from enrolling at this time because serial numbers are not verified during enrollment. Blocking personal devices by serial number will be released in the near future.


### Device management
#### New remote actions for iOS devices <!-- 854689 -->
In this release, we've added two new remote device actions for shared iPad devices that manage the Apple Classroom app:

- 	[Logout current user](device-logout-user.md) - Logs out the current user of an iOS device you choose.
- 	[Remove user](device-remove-user.md) - Deletes a user you choose from the local cache on an iOS device.


#### Support for shared iPads with the iOS Classroom app <!-- 1044681 -->
In this release, we've expanded the support for managing the iOS Classroom app to include students who log into shared iPads using their managed Apple ID.


### App management  

#### Changes to Intune built-in apps <!-- 1332306 -->

Previously, Intune contained a number of built-in apps that you could quickly assign. Based on your feedback, we have removed this list, and you will no longer see built-in apps.
However, if you have already assigned any built-in apps, these will still be visible in the list of apps. You can continue to assign these apps as required.
In a later release, we plan to add an easier method to select and assign built-in apps from the Intune portal.

#### Easier installation of Office 365 apps <!--- 1121362 --->
The new **Office 365 ProPlus** app type makes it easy for you to assign Office 365 ProPlus 2016 apps to devices that you manage which run the latest version of Windows 10. Additionally, you can also install Microsoft Project, and Microsoft Visio, if you own licenses for them. The apps you want are bundled together and appear as one app in the list of apps in the Intune console.
For more information, see [How to add Office 365 apps for Windows 10](apps-add-office365.md).


#### Support for offline apps from the Windows Store for Business <!--- 777044 --->
Offline apps you purchased from the Windows Store for Business will now be synchronized to the Intune portal. You can then deploy these apps to device groups, or user groups. Offline apps are installed by Intune, and not by the store.

#### Microsoft teams is now part of the App-based CA list of approved apps   <!-- 1257019 -->

The Microsoft Teams app for iOS and Android is now part of approved apps for app-based conditional access policies for Exchange and SharePoint Online. The app can be configured through the Intune App Protection blade in the Azure portal to all tenants currently using app-based conditional access.

#### Managed browser and app proxy integration <!-- 1287310 -->
 The Intune Managed Browser can now integrate with the Azure AD Application Proxy service to let users access internal web sites even when they are working remotely. Users of the browser simply enter the site URL as they normally would and the Managed Browser routes the request through the application proxy web gateway. For more information, see [Manage Internet access using Managed browser policies](app-configuration-managed-browser.md).


#### New app configuration settings for the Intune Managed Browser <!-- 682951 -->
In this release, we've added further configurations for the Intune Managed Browser app for iOS and Android. You can now use an app configuration policy to configure the default home page and bookmarks for the browser.
For more information, see [Manage Internet access using Managed browser policies](app-configuration-managed-browser.md)




### Device configuration  
#### BitLocker settings for Windows 10  <!-- 951707 -->
You can now configure BitLocker settings for Windows 10 devices using a new Intune device profile. For example, you can require that devices are encrypted, and also configure further settings that are applied when BitLocker is turned on.
For more information, see [Endpoint protection settings for Windows 10 and later](endpoint-protection-windows-10.md).

### New settings for Windows 10 device restriction profile <!--- 978527,  978550, 978569, 1050031, 1058611,  --->

In this release, we've added new settings for the Windows 10 device restriction profile, in the following categories:

-  Windows Defender
-  Cellular and connectivity
-  Locked screen experience
-  Privacy
-  Search
-  Windows Spotlight
-  Edge browser

For more information about Windows 10 settings, see [Windows 10 and later device restriction settings](device-restrictions-windows-10.md).

## Week of June 12, 2017

### Company Portal app for Android now has a new end user experience for App Protection Policies <!--1305217-->
Based on customer feedback, we've modified the Company Portal app for Android to show an **Access Company Content** button. The intent is to prevent end users from unnecessarily going through the enrollment process when they only need to access apps that support App Protection Policies, a feature of Intune mobile application management. You can see these changes on the [what's new in app UI](whats-new-app-ui.md) page.

### New menu action to easily remove Company Portal <!--1164569-->
Based on user feedback, the Company Portal app for Android has added a new menu action to initiate the removal of Company Portal from your device. This action removes the device from Intune management so that the app can be removed from the device by the user. You can see these changes on the [what's new in app UI](whats-new-app-ui.md) page and in the [Android end user documentation](/intune-user-help/unenroll-your-device-from-intune-android).

### Improvements to app syncing with Windows 10 Creators Update <!--676505-->

The Company Portal app for Windows 10 will now automatically initiate a sync for app install requests for devices with Windows 10 Creators Update (version 1703). This will reduce the issue of app installs stalling during the "Pending Sync" state. In addition, users will be able to manually initiate a sync from within the app. You can see these changes on the [what's new in app UI](whats-new-app-ui.md) page.

### New guided experience for Windows 10 Company Portal <!---1058938--->

The Company Portal app for Windows 10 will include a guided Intune walkthrough experience for devices that have not been identified or enrolled. The new experience provides step-by-step instructions that guide the user through registering into Azure Active Directory (required for Conditional Access features) and MDM enrollment (required for device management features). The guided experience will be accessible from the Company Portal home page. Users can continue to use the app if they do not complete registration and enrollment, but will experience limited functionality.

This update is only visible on devices running Windows 10 Anniversary Update (build 1607) or higher. You can see these changes on the [what's new in app UI](whats-new-app-ui.md) page.

## Week of June 5, 2017

### Microsoft Intune and Conditional Access admin consoles are generally available

We’re announcing the general availability of both the new Intune on Azure admin console and the Conditional Access admin console. Through Intune on Azure, you can now manage all Intune MAM and MDM capabilities in one consolidated admin experience, and leverage Azure AD grouping and targeting. Conditional access in Azure brings rich capabilities across Azure AD and Intune together in one unified console. And from an administrative experience, moving to the Azure platform allows you to use modern browsers.

Intune is now visible without the **preview** label in the Azure console at portal.azure.com.

There is no action required for existing customers at this time, unless you have received one of a series of messages in the message center requesting that you take action so that we can migrate your groups. You may have also received a message center notice informing you that migration is taking longer due to bugs on our side. We are diligently continuing work to migrate any impacted customer.

### Improvements to the app tiles in the Company Portal app for iOS
We updated the design of the app tiles on the homepage to reflect the branding color you set for the Company Portal. For more information, see [what's new in app UI](whats-new-app-ui.md).

### Account picker now available for the Company Portal app for iOS
Users of iOS devices might see our new account picker when they sign into the Company Portal if they use their work or school account to sign into other Microsoft apps. For more information, see [what's new in app UI](whats-new-app-ui.md).

## Week of May 29, 2017

### Change your MDM authority without unenrolling managed devices <!--1103950-->

You can now change your MDM authority without having to contact Microsoft Support, and without having to unenroll and reenroll your existing managed devices. In the Configuration Manager console, you can [change your MDM authority](/sccm/mdm/deploy-use/change-mdm-authority) from Set to Configuration Manager (hybrid) to Microsoft Intune (standalone) or vice versa.


### Improved notification for Samsung KNOX startup PINs <!--1087143-->
When end users need to set a start-up PIN on Samsung KNOX devices to become compliant with encryption, the notification displayed to end users will bring them to the exact place in the Settings app when the notification is tapped.  Previously, the notification brought the end user to the password change screen.


### Device enrollment

#### Apple School Manager (ASM) support with shared iPad <!-- 748864, 770395-->

Intune now supports use of Apple School Manager (ASM) in place of Apple Device Enrollment Program to provide out-of-box enrollment of iOS devices. ASM onboarding is required to use the Classroom app for Shared iPads, and is required to enable syncing data from ASM to Azure Active Directory via Microsoft School Data Sync (SDS). For more information, see [Enable iOS device enrollment with Apple School Manager](apple-school-manager-set-up-ios.md).

> [!NOTE]
> Configuring Shared iPads to work with the Classroom app requires iOS Education configurations in Azure are that not yet available.  This functionality will be added soon.

### Device management

#### Provide remote assistance to Android devices using TeamViewer <!-- 675418 -->

Intune can now use the [TeamViewer](https://www.teamviewer.com) software, purchased separately, to enable you to give remote assistance to your users who are running Android devices. For more information, see [Provide remote assistance for Intune managed Android devices](device-profile-android-teamviewer.md).

### App management

#### New app protection policies conditions for MAM <!-- 679864 -->

You can now set a requirement for MAM without enrollment users that enforces the following policies:

- Minimum application version
- Minimum operating system version
- Minimum Intune APP SDK version of the targeted application (iOS only)

This feature is available on both Android and iOS. Intune supports minimum version enforcement for OS platform versions, application versions, and Intune APP SDK. On iOS, applications that have the SDK integrated can also set a minimum version enforcement at the SDK level. The user will be unable to access the targeted application if the minimum requirements through the app protection policy are not met at the three different levels mentioned above. At this point, the user may either remove their account (for multi-identity applications), close the application, or update the version of the OS or application.

You can also configure additional settings to provide a non-blocking notification that recommends an OS or application upgrade. This notification can be closed and the application may be used as normal.

For more information, see [iOS app protection policy settings](app-protection-policy-settings-ios.md) and [Android app protection policy settings](app-protection-policy-settings-android.md).

#### Configure app configurations for Android for Work <!-- 621621 -->
Some Android apps from the store support managed configuration options that let an IT admin control how an app runs in the work profile. With Intune, you can now view the configurations supported by an app, and configure them from the Intune portal with a configuration designer or a JSON editor. For more information, see [Use app configurations for Android for Work](app-configuration-policies-use-android.md).

#### New app configuration capability for MAM without enrollment <!-- 677969 -->

You can now create app configuration policies through the MAM without enrollment channel. This feature is equivalent to the app configuration policies available in the mobile device management (MDM) app configuration. For an example of app configuration using MAM without enrollment, see  [Manage Internet access using Managed browser policies with Microsoft Intune](app-configuration-managed-browser.md).

#### Configure allowed and blocked URL lists for the Managed Browser <!-- 682960 -->

You can now configure a list of allowed and blocked domains and URLs for the Intune Managed Browser using app configuration settings in the Azure portal. These settings can be configured regardless of whether it is being used on a managed or unmanaged device. For more information, see [Manage Internet access using Managed browser policies with Microsoft Intune](app-configuration-managed-browser.md).

#### App protection policy helpdesk view <!-- 1069473 -->

IT Helpdesk users can now check user license status and the status of app protection policy apps assigned to users in the Troubleshooting blade. For details, see [Troubleshooting](./help-desk-operators.md).

### Device configuration

#### Control website visits on iOS devices <!-- 723832 -->

You can now control which websites users of iOS devices can visit using one of the following two methods:

- Add permitted, and blocked URLs using Apples built-in web content filter.

- Allow only specified websites to be accessed by the Safari browser. Bookmarks are created in Safari for each site you specify.

For more information, see [Web content filter settings for iOS devices](web-content-filter-settings-ios.md).

#### Preconfigure device permissions for Android for Work apps <!-- 621614 -->

For apps deployed to Android for Work device work profiles, you can now configure the permissions state for individual apps.  By default, Android apps that require device permissions such as access to location or the device camera will prompt users to accept or deny permissions.  For example, if an app uses the device's microphone, then the end user is prompted to grant the app permission to use the microphone. This feature allows you to define permissions on behalf of the end user.  You can configure permissions to a) automatically deny without notifying the user, b) automatically approve without notifying the user, or c) prompt the user to accept or deny. For more information, see [Android for Work device restriction settings in Microsoft Intune](device-restrictions-android-for-work.md).

#### Define app-specific PIN for Android for Work devices <!-- 728976, 1102534 -->

Android 7.0 and above devices with a work profile managed as an Android for Work device let the administrator define a passcode policy that only applies to apps in the work profile.  Options include:

- Define just a device-wide passcode policy - This is the passcode that the user must use to unlock their entire device.
- Define just a work profile passcode policy - Users will be prompted to enter a passcode whenever any app in the work profile is opened.
- Define both a device and work profile policy - IT admin has the choice to define both a device passcode policy and a work profile passcode policy at differing strengths (for example, a four-digit PIN to unlock the device, but a six-digit PIN to open any work app).

For more information, see [Android for Work device restriction settings in Microsoft Intune](device-restrictions-android-for-work.md).

> [!NOTE]
> This is only available on Android 7.0 and above.  By default, the end user can use the two separately defined PINs or they can elect to combine the two defined PINs into the strongest of the two.

#### New settings for Windows 10 devices <!-- 978585 -->

We've added new [Windows device restriction settings](device-restrictions-windows-10.md) that control features like wireless displays, device discovery, task switching, and SIM card error messages.

#### Updates to certificate configuration <!-- 918991 and 823198 -->

When creating a SCEP certificate profile, for **Subject name format**, the **Custom** option is available for iOS, Android, and Windows devices. Before this update, the **Custom** field was available for iOS devices only. For more information, see [ How to create a SCEP certificate profile] (certificates-scep-configure.md#how-to-create-a-scep-certificate-profile).

When creating a PKCS certificate profile, for **Subject alternative name**, the **Custom Azure AD attribute** is available. The **Department** option is available when you select **Custom Azure AD attribute**. For more information, see [How to create a PKCS certificate profile] (certficates-pfx-configure.md#how-to-create-a-pkcs-certificate-profile).

#### Configure multiple apps that can run when an Android device is in kiosk mode <!-- 662059 -->

When an Android device is in kiosk mode, you could previously only configure one app that was allowed to run. You can now configure multiple apps using the app ID, store URL, or by selecting an Android app you already manage. For more information, see [Kiosk mode settings](device-restrictions-android.md#kiosk).


## Notices

### IP addresses for Intune updated <!-- 1175274 -->

An [updated list of DNS names and IP addresses](/intune/network-bandwidth-use) is available for firewall proxy settings.

### Use Azure Active Directory for conditional access <!-- 967947 -->

Conditional access is available in the Azure Active Directory section of the Azure console and provides a more powerful and flexible framework for setting policies for cloud apps like Office 365 Exchange Online and SharePoint Online.  Use the **Conditional access in Azure Active Directory** blade to configure policies instead of the classic Intune console. Existing policies in the classic Intune console need to be re-created in the Azure console. For more information, see [Create Azure AD conditional access policies](/intune/conditional-access-exchange-create.md#create-azure-ad-conditional-access-policies-in-intune-azure-preview)

### Direct access to Apple enrollment scenarios <!--951869-->

For Intune accounts created after January 2017, Intune has enabled direct access to Apple enrollment scenarios using the Enroll Devices workload in the Azure portal. Previously, the Apple enrollment preview was only accessible from links in the classic Intune portal. Intune accounts created before January 2017 require a one-time migration before these features are available in Azure. The schedule for migration has not been announced yet, but details will be made available as soon as possible. We strongly recommend creating a trial account to test out the new experience if your existing account cannot access the Azure portal.

### Administration roles being replaced in Azure portal

The existing mobile application management (MAM) administration roles (Contributor, Owner, and Read-Only) used in the Intune classic portal (Silverlight) are being replaced with a full set of new role-based administration controls (RBAC) in the Intune Azure portal. Once you are migrated to the Azure portal, you will need to reassign your admins to these new administration roles. For more information about RBAC and the new roles, see [Role-based access control for Microsoft Intune](/intune/role-based-access-control).

## What's coming

### End of support for Android 4.3 and lower <!---1171127, 1326920 --->
Managed apps and the Company Portal app for Android will require Android 4.4 and higher to access company resources. Devices that aren't updated before the beginning of October will no longer be able to access the Company Portal or those apps. By December, all enrolled devices will be force retired in December, resulting in loss of access to company resources. If you are using app protection policies without MDM, apps will not receive updates, and the quality of their experience will diminish over time.


### Platform Support Reminder: Windows Phone 8.1 mainstream support will end July 11, 2017
<!-- 1327781 -->

On July 11, 2017,  the Windows Phone 8.1 platform will reach end of mainstream support. Windows 8.1 PC support is not impacted.

There is no immediate impact to any Windows Phone 8.1 device that is managed by the Intune service. Devices that are enrolled will continue to work and all policies, configurations, and apps will continue to work as expected. Note that there are no improvements targeted for the Windows Phone 8.1 platform within the Intune Service, and for the Windows Phone 8.1 Company Portal app.

We recommend that you upgrade eligible Windows Phone 8.1 devices to Windows 10 Mobile at your earliest opportunity. 

### Changes in support for the Intune iOS Company Portal app  <!-- 1164474  -->


Coming soon, there will be a new version of the Microsoft Intune Company Portal app for iOS that will support only devices running iOS 9.0 or later. The version of the Company Portal that supports iOS 8 will still be available for a very short period of time. However, please note that if you also use MAM-enabled iOS apps we support iOS 9.0 and later, so you'll want to ensure your end users update to the latest OS. 

#### How does this affect me?
We are letting you know this in advance, even though we don't have specific dates, so you have time to plan. Please ensure your users are updated to iOS 9+ and when the Company Portal app releases, request that your end users update their Company Portal app.

#### What do I need to do to prepare for this change?

Encourage your users to update to iOS 9.0 or later to take full advantage of new Intune features.  Encourage users to install the new
version of the Company Portal and take advantage of the new features it will offer.

Go to the Intune on Azure portal and view Devices > All Devices and filter by iOS version to see any current devices with operating systems earlier than iOS 9.

### Improved sign in experience across Company Portal apps for all platforms <!--User Story 1132123-->

We are announcing a change that is coming in the next few months that will improve the sign-in experience for the Intune Company Portal apps for Android, iOS, and Windows. The new user experience will automatically appear across all platforms for the Company Portal app when Azure AD makes this change. In addition, users can now sign in to the Company Portal from another device with a generated, single-use code. This is especially useful in cases when users need to sign in without credentials.

To see screenshots of the previous sign-in experience, the new sign-in experience with credentials, and the new sign-in experience from another device, see [What's new in app UI](/intune/whats-new-app-ui).

### Plan for change: Intune is changing the Intune Partner Portal experience <!-- 1050016 -->

We are removing the Intune Partner page from manage.microsoft.com beginning with the service update in mid-May 2017.  

If you are a partner administrator, you will no longer be able to view and take action on behalf of your customers from the Intune Partner page, but will instead need to sign in at one of two other partner portals at Microsoft.

Both the [Microsoft Partner Center](https://partnercenter.microsoft.com/) and the [Microsoft Office 365 Partner Admin Center](https://portal.office.com/) will allow you to sign into the customer accounts you manage. Moving forward as a partner, please use one of these sites to manage your customers.


### Apple to require updates for Application Transport Security <!--748318-->

Apple has announced that they will enforce specific requirements for Application Transport Security (ATS). ATS is used to enforce stricter security on all app communications over HTTPS. This change impacts Intune customers using the iOS Company Portal apps.

We have made available a version of the Company Portal app for iOS through the Apple TestFlight program that enforces the new ATS requirements. If you would like to try it so you can test your ATS compliance, email <a href="mailto:CompanyPortalBeta@microsoft.com?subject=Register to TestFlight ATS Company Portal app">CompanyPortalBeta@microsoft.com</a> with your first name, last name, email address, and company name. Review our [Intune support blog](https://aka.ms/compportalats) for more details.

### See also
* [Microsoft Intune Blog](http://go.microsoft.com/fwlink/?LinkID=273882)
* [Cloud Platform roadmap](https://www.microsoft.com/server-cloud/roadmap/Indevelopment.aspx?TabIndex=0&dropValue=Intune)
* [What's new in the Company Portal UI](whats-new-app-ui.md)
* [What's new in previous months](whats-new-archive.md)
