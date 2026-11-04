# Privacy policy: Intune Enhancer

_Last updated: 4 November 2026_

## The short version

**No data is sent to the developer, or anywhere other than Microsoft.** Intune Enhancer only
talks to Microsoft Graph (graph.microsoft.com, or the US Government equivalents if you choose to
allow them), the same service the Microsoft Intune admin center itself uses. The developer runs no server for this extension and receives nothing from
it.

## What the extension accesses

After you accept the disclosure on the extension's Settings page (it opens when you install):

- **US Government clouds (optional).** By default the extension works only on the commercial
  Intune admin center (intune.microsoft.com). If your tenant is on a US Government cloud (GCC High or DoD),
  you can allow it in the workspace's Settings, and your browser then asks for access to the government
  Intune admin center (intune.microsoft.us), the Azure Government portal (portal.azure.us) and the
  Microsoft Graph addresses graph.microsoft.us and dod-graph.microsoft.us. Nothing is requested or used
  until you allow it, and you can remove it again there. Everything else in this policy applies to those
  clouds in the same way.
- **Sign-in tokens.** It reads the Microsoft Graph access tokens that the Intune admin center
  already holds for your sign-in, so it can make requests as you. It does not read refresh
  tokens, ID tokens or passwords, and it never asks for your password.
- **Device information from Microsoft Graph.** For each Intune managed device: its id, name,
  serial number, Microsoft Entra device id, operating system and version, model, total and free
  storage, compliance state, ownership, enrolment and last sync time, its primary user's id, display
  name and user principal name, and the display name and user principal name of the user who last
  logged on (Windows devices). For Entra device lists, it may look up which Entra object ids are devices.
- **Hardware details** (the workspace's Hardware report, only when you click "Read hardware for all
  devices"): for each device, its manufacturer, model, serial number, operating system and edition,
  memory, storage, encryption state, TPM and BIOS details, battery health, IP address, and Wi-Fi and
  Ethernet MAC addresses. This report is saved on your computer (see below).
- **Policy information** (workspace tools): the names, configured settings, assignments and
  created / last modified dates of Intune policies, profiles, scripts, apps and similar objects.
- **Group information**: member counts of groups shown in the admin center (group size hints),
  and, in the workspace, group names, descriptions, membership rules, owners and members, and,
  for Group impact, the Conditional Access policies, enterprise app assignments, licences and
  Intune role assignments that reference a group.
- **Group memberships and user search** (Device 360, Compare devices, Compare users and the Related
  button): the groups a device or user belongs to, directly and through other groups, and the names and
  user principal names of users you search for.
- **Compliance results** (Compliance breakdown): for each compliance setting, how many devices pass and
  fail, and for a setting you open, the failing devices with their names, primary users and state.
- **User account status** (Orphaned users): whether each device's primary user still exists in Microsoft
  Entra and is enabled.
- **Tenant health**: the Apple push certificate (Apple ID and expiry), Apple VPP and enrolment tokens (names
  and expiry), the Managed Google Play binding (owner user principal name), and certificate connectors
  (names, state and last contact).
- **Assignment filters**: filter names, platforms and rules, to show a filter's rule on hover.
- **App install counts**: for each app shown in an app list, how many devices it installed on
  and failed on (Intune's app status report).
- **Policy status counts**: for each policy shown in the Configuration list, how many devices
  it succeeded and failed on (Intune's device status reports).
- **Installed app versions and device details**: in the workspace's App versions tool, the discovered
  apps whose name you search for, with their versions and device counts, and the devices running a
  version you pick; in Device quick facts, when you click "More details", one device's hardware, storage
  and network details (serial number, memory, storage, encryption, TPM, IP and MAC address, enrolment).
  Both are read from Microsoft Graph and are not stored beyond the 30 minutes below.
- **Remediation script dates**: when each script package in the Remediations list was created and last
  modified.
- **Any ID you paste** into the ID decoder, which is looked up in Microsoft Graph.

It can only access what your own account and Intune role can already access.

<!-- Update this list as each new feature ships, before it is published, and copy this file to
     systmworks/app-docs (intune-enhancer/privacy-policy.md), which is the public copy. -->

## Where data goes

- **To Microsoft Graph only.** All network requests go to `https://graph.microsoft.com`. If you use a US
  Government cloud and choose to allow it in Settings, requests go to `https://graph.microsoft.us` or
  `https://dod-graph.microsoft.us` instead, and only to the one for the cloud you are signed in to. Nothing is
  allowed until you grant it. The extension's code refuses to send a request to any other address.
- **To no one else.** Nothing is sent to the developer or any third party. There are no
  analytics, tracking, advertising, licensing checks or error reports.

## What is stored, and where

- **Device list and policy list:** stored in this extension's local browser storage (IndexedDB) on your computer,
  separately for each tenant, so lists can be labelled and searches answered instantly. The device list
  includes each device's serial number and storage figures. You can delete them at any time with "Clear
  stored data" on the Settings page, or by removing the extension.
- **Hardware report:** if you run it, the report's rows (including serial numbers, IP addresses and MAC
  addresses) are saved in the same local storage with the date they were read, so the report is there the
  next time you open the workspace. "Clear stored data" deletes it, and so does removing the extension.
- **Not stored:** group reports, rosters, comparisons and decoded IDs exist only while the workspace tab
  shows them, and in any CSV you choose to save.
- **Recent lookups:** the group sizes, app and policy status counts, remediation script dates, policy names and filter rules
  shown in the admin center are kept on your computer for up to 30 minutes, so lists you reopen
  show them straight away. "Clear stored data" deletes them, as does removing the extension.
- **Sign-in tokens:** kept in memory and in the browser's session storage, which is memory only
  and cleared when the browser closes. Never written to disk by the extension.
- **Settings:** which in-portal features are switched on and how they show (for example display
  names or user principal names), and the column widths you choose or drag (extension storage),
  and the workspace's light or dark theme and the tool you last had open (the workspace page's own storage).

## Changes to your tenant

None. The extension is read-only.

## Children

The extension is a tool for IT administrators and is not directed at children.

## Changes to this policy

If a future version changes what is accessed or where it goes, this policy will be updated
before that version is published.

## Contact

systmworks@outlook.com
