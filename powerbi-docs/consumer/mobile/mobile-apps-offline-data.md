---
title: View your data offline in the Power BI mobile apps
description: Learn about how you can view your data in Power BI mobile apps when you’re not connected to a network.
author: paulinbar
ms.author: painbar
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-mobile
ms.topic: conceptual
ms.date: 10/19/2021
---

# View your data offline in the Power BI mobile apps

Applies to:

| :::image type="icon" source="./media/mobile-apps-offline-data/iphone-logo-50-px.png"::: | :::image type="icon" source="./media/mobile-apps-offline-data/ipad-logo-50-px.png"::: | :::image type="icon" source="./media/mobile-apps-offline-data/android-phone-logo-50-px.png"::: | :::image type="icon" source="./media/mobile-apps-offline-data/android-tablet-logo-50-px.png"::: | :::image type="icon" source="./media/mobile-apps-offline-data/win-10-logo-50-px.png"::: |
|:--- |:--- |:--- |:--- |:--- |
| iPhones |iPads |Android phones |Android tablets |Windows devices |

>[!NOTE]
>Power BI mobile app support for **phones using Windows 10 Mobile** was discontinued on March 16, 2021. [Learn more](/legal/powerbi/powerbi-mobile/power-bi-mobile-app-end-of-support-for-windows-phones)

One advantage of viewing Power BI in a mobile app rather than in a mobile browser is that you can see your data even when you're not connected to a network.

:::image type="content" source="./media/mobile-apps-offline-data/power-bi-iphone-no-network.png" alt-text="Screenshot that shows Power BI mobile app with 'No network' message.":::

By default, Power BI refreshes the data frequently so you get up-to-date answers to your business questions any time, even while commuting or roaming.

## Data access while you're offline

While you're offline, you can access and interact with dashboards you've accessed previously from the mobile app.

You also have read-only access to any Power BI reports you've accessed previously from the mobile app. You can see the full report, but not filter, cross-filter, sort, or use slicers on it.

>[!NOTE]
> Reports based on DirectQuery or live connection are not cached and are not available offline.

## Background data refresh

Background refresh updates your favorite dashboards, plus dashboards and reports you've viewed in the last two weeks, with the data on the Power BI service (not the data source). If you're connected to Wi-Fi, background refresh updates every 2 hours. Otherwise, if you're on a 3G network, Power BI updates the content every 24 hours.

You can turn off background refresh, for example, to avoid network usage. Check the settings on your device.

> [!NOTE]
> If you use the Power BI mobile app on an iOS device and your organization has configured Microsoft Intune MAM, then background data refresh is turned off. The next time you enter the app, Power BI refreshes the data from the Power BI service on the web.
>
> For more information, see [Configure mobile apps with Microsoft Intune](../../enterprise/service-admin-mobile-intune.md).

## Offline indicators

Power BI provides clear indicators when you go in and out of offline mode, as well as indicators for missing dashboards, reports, and tiles that aren't available offline.

## Considerations and limitations

When you're offline with Power BI on your mobile device:

* Power BI can cache up to 250 MB of data offline.
* Reports based on DirectQuery or live connection aren't cached and aren't available offline.
* Some tile types require an active server connection, so they aren't available offline. For example, Bing map tiles and some custom tiles.
* Whole Excel workbooks in Power BI aren't available offline.
* You can see Reporting Services mobile reports and KPIs offline, if you viewed them while connected. They don't refresh in the background. They refresh every time you open them.
* In the Power BI mobile apps, you can't see Power BI Desktop (PBIX) files saved to Power BI Report Server.
* Paginated reports (RDL) are not available while the network is offline.

## Next steps

Your feedback helps us decide what to implement in the future, so don't forget to vote for other features you'd like to see in Power BI mobile apps.

* [What are the Power BI mobile apps?](mobile-apps-for-mobile-devices.md)
* Follow [@MSPowerBI](https://twitter.com/mspowerbi) on Twitter
* Join the conversation at the [Power BI Community](https://community.powerbi.com/)
* [What is Power BI?](../../fundamentals/power-bi-overview.md)
