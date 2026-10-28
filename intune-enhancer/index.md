# Privacy policy: Intune Enhancer

_Last updated: 28 October 2026_

## The short version

**No data is sent to the developer, or anywhere other than Microsoft.** Intune Enhancer only
talks to Microsoft Graph (graph.microsoft.com), the same service the Microsoft Intune admin
center itself uses. The developer runs no server for this extension and receives nothing from
it.

## What the extension accesses

After you accept the disclosure on the extension's Settings page (it opens when you install):

- **Sign-in tokens.** It reads the Microsoft Graph access tokens that the Intune admin center
  already holds for your sign-in, so it can make requests as you. It does not read refresh
  tokens, ID tokens or passwords, and it never asks for your password.
- **Device information from Microsoft Graph.** For each Intune managed device: its id, name,
  Microsoft Entra device id, operating system and version, model, compliance state, ownership,
  enrolment and last sync time, its primary user's display name and user principal name, and
  the display name and user principal name of the user who last logged on (Windows devices).
  For Entra device lists, it may look up which Entra object ids are devices.
- **Policy information** (workspace tools): the names, configured settings, assignments and
  created / last modified dates of Intune policies, profiles, scripts, apps and similar objects.
- **Group information**: member counts of groups shown in the admin center (group size hints),
  and, in the workspace, group names, descriptions, membership rules, owners and members, and,
  for Group impact, the Conditional Access policies, enterprise app assignments, licences and
  Intune role assignments that reference a group.
- **Assignment filters**: filter names, platforms and rules, to show a filter's rule on hover.
- **App install counts**: for each app shown in an app list, how many devices it installed on
  and failed on (Intune's app status report).
- **Policy status counts**: for each policy shown in the Configuration list, how many devices
  it succeeded and failed on (Intune's device status reports).
- **Any ID you paste** into the ID decoder, which is looked up in Microsoft Graph.

It can only access what your own account and Intune role can already access.

<!-- Update this list as each new feature ships, before it is published, and copy this file to
     systmworks/privacy-policies (intune-enhancer/index.md), which is the public copy. -->

## Where data goes

- **To Microsoft Graph only.** All network requests go to `https://graph.microsoft.com`. The
  extension's code refuses to send a request to any other address.
- **To no one else.** Nothing is sent to the developer or any third party. There are no
  analytics, tracking, advertising, licensing checks or error reports.

## What is stored, and where

- **Device list and policy list:** stored in the browser's extension storage on your computer,
  separately for each tenant, so lists can be labelled and searches answered instantly. You can
  delete them at any time with "Clear stored data" on the Settings page, or by removing the extension.
  Group reports, rosters and decoded IDs are not stored; they exist only while the workspace tab
  shows them, and in any CSV you choose to save.
- **Sign-in tokens:** kept in memory and in the browser's session storage, which is memory only
  and cleared when the browser closes. Never written to disk by the extension.
- **Settings:** which in-portal features are switched on and how they show (for example display
  names or user principal names), and the column widths you choose or drag (extension storage),
  and the workspace's light or dark theme (the workspace page's own storage).

## Changes to your tenant

None. The extension is read-only.

## Children

The extension is a tool for IT administrators and is not directed at children.

## Changes to this policy

If a future version changes what is accessed or where it goes, this policy will be updated
before that version is published.

## Contact

systmworks@gmail.com
