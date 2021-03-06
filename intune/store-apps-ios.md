---
# required metadata
title: Add iOS store apps to Microsoft Intune
titleSuffix:
description: Learn about adding iOS store apps to Microsoft Intune. You can assign apps using this method if the apps are free of charge in the App Store.
keywords: Intune
author: Erikre
ms.author: erikre
manager: dougeby
ms.date: 05/20/2019
ms.topic: conceptual
ms.service: microsoft-intune
ms.localizationpriority: high
ms.technology:
ms.assetid: c59514d7-1256-4576-9380-e7a0b85a0378

# optional metadata
#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: mghadial
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure
ms.collection: M365-identity-device-management
---

# Add iOS store apps to Microsoft Intune

[!INCLUDE [azure_portal](./includes/azure_portal.md)]

Use the information in this article to help you add iOS store apps to Microsoft Intune. iOS store apps are apps that Intune installs on your users' devices. A user is part of your company's workforce. iOS store apps are automatically updated.

>[!NOTE]
>Although users of iOS devices can remove some built-in iOS apps, such as Stocks and Maps, you cannot use Intune to redeploy those apps. If your users delete these apps, they must go to the App Store and manually reinstall them.

## Before you start

You can assign apps by using this method only if they are free of charge in the App Store. If you want to assign paid apps by using Intune, consider using the [iOS volume-purchase program](vpp-apps-ios.md).

>[!NOTE]
>When you work with Microsoft Intune, we recommend that you use either the Microsoft Edge or Google Chrome browser.

1. Sign in to [Intune](https://go.microsoft.com/fwlink/?linkid=2090973).
3. In the **Intune** pane, select **Client apps**.
4. In the **Client apps** workload pane, under **Manage**, select **Apps**.
5. In the **Apps** pane, select **Add**.
6. In the **App type** list, under the **Store app** types, select **iOS**.
7. Select **Search the App Store**.
8. In the **Search the App Store** pane, select the App Store country/region locale.
9. In the **Search** box, type the name (or part of the name) of the app.  
    Intune searches the store and returns a list of relevant results.
10. In the results list, select the app you want, and then select **Select**.
11. In the **Add app** pane, select **App information** to configure the app.
12. In the **App information** pane, add the app information. Depending on the app you have chosen, some of the values in this pane might have been automatically filled in:
    - **Name**: Enter the name of the app as it is to be displayed in the company portal. Make sure that any app name that you use is unique. If an app name is duplicated, only one name is displayed to users in the company portal.
    - **Description**: Enter a description for the app. This description is displayed to users in the company portal.
    - **Publisher**: Enter the name of the publisher of the app.
    - **Appstore URL**: Type the App Store URL of the app that you want to create.
    - **Minimum operating system**: In the list, select the earliest operating system version on which the app can be installed. If you assign the app to a device with an earlier operating system, it will not be installed.
    - **Applicable device type**: In the list, select the devices that are used by the app.
    - **Category**: Optionally, select one or more of the built-in app categories, or a category that you created. Doing so makes it easier for users to find the app when they browse the company portal.
    - **Display this as a featured app in the Company Portal**: Select this option to display the app suite prominently on the main page of the company portal when users browse for apps.
    - **Information URL**: Optionally, enter the URL of a website that contains information about this app. The URL is displayed to users in the company portal.
    - **Privacy URL**: Optionally, enter the URL of a website that contains privacy information for this app. The URL is displayed to users in the company portal.
    - **Developer**: Optionally, enter the name of the app developer. This field is visible only to administrators and is not visible to your users.
    - **Owner**: Optionally, enter a name for the owner of this app, for example, *HR department*. This field is visible only to administrators and is not visible to your users.
    - **Notes**: Optionally, enter any notes that you want to associate with this app. This field is only visible an administrator and will not be visible to end users.
    - **Logo**: Optionally, upload an icon that will be associated with the app. This icon is displayed with the app when users browse the company portal.
13. Select **OK**.
14. Select **Add**.

The app you have created is displayed in the apps list, where you can assign it to the groups that you select.

## Next steps

- [Assign apps to groups](apps-deploy.md)
