<p align="center"><a href="https://buymeacoffee.com/systmworks"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="45" alt="Buy me a coffee"></a></p>

> I have spent many, many hours creating and testing this. If it helps you please consider buying me a Coffee :)

# Intune Enhancer screenshots

Every screenshot is the real extension on a fictional tenant (Fabrikam). Nothing here is from a real tenant. The Intune admin center first (light theme, as the admin center looks), then the workspace tools (dark theme) in the same order as the workspace's sidebar, top to bottom.

## In the Intune admin center

### 1. Devices list

Each device shows its primary user, a green, yellow, orange or red check-in light and a flag when free storage is low, right in the admin center's own list.

![Devices list](admin-center/01-devices-list.png)

### 2. Group lists

How many devices, users and groups each group holds, beside its name. Empty groups say so.

![Group lists](admin-center/02-groups-list.png)

### 3. Policy lists

The number of devices that succeeded and failed sits next to each policy's name, so a failing policy stands out without opening it.

![Policy lists](admin-center/03-policies-list.png)

### 4. App lists

The same succeeded and failed counts next to each app.

![App lists](admin-center/04-apps-list.png)

### 5. Adding members to a group

In the Add members picker each device shows its primary user and check-in light, so you pick the right one.

![Adding members to a group](admin-center/05-add-members.png)

### 6. Used by button

A Used by command beside Delete on a group's page opens everything that references that group in the workspace.

![Used by button](admin-center/06-group-used-by.png)

### 7. Related button

A Related command on a device's page shows the primary user's other devices and the groups the device is in.

![Related button](admin-center/07-device-related.png)

### 8. Settings picker usage

When adding settings to a policy, 'Set in N policies' appears beside each setting that is already configured, with the policy names on hover.

![Settings picker usage](admin-center/08-settings-picker-usage.png)

## In the workspace

### 9. Settings

*The extension.* A switch for every addition to the admin center, so each can be turned off.

![Settings](workspace/09-settings.png)

### 10. Autopilot failures

*Devices.* Failed Autopilot deployments from the last 1 to 30 days, with one search box for host name, serial number or user, and the enrollment status page apps and policies behind each failure.

![Autopilot failures](workspace/10-autopilot-failures.png)

### 11. Compare devices

*Devices.* Two devices side by side: details, groups, and which policies, apps and scripts reach one or both.

![Compare devices](workspace/11-compare-devices.png)

### 12. Compliance breakdown

*Devices.* Which compliance settings fail on the most devices, worst first, with the devices behind each one.

![Compliance breakdown](workspace/12-compliance-breakdown.png)

### 13. Device 360

*Devices.* Every policy, app and script that reaches one device, and why: which group, whether it is excluded, or depends on a filter.

![Device 360](workspace/13-device-360.png)

### 14. Device explorer

*Devices.* Every device in one table with the columns you choose, such as ownership, join type, manufacturer, encryption and certificate expiry. Filter, sort, copy or save.

![Device explorer](workspace/14-device-explorer.png)

### 15. Hardware report

*Devices.* Memory, storage, TPM, BIOS and more for every device, sortable, and saved as CSV.

![Hardware report](workspace/15-hardware.png)

### 16. Low storage

*Devices.* Devices with little free disk space, least free first.

![Low storage](workspace/16-low-storage.png)

### 17. OS builds

*Devices.* How many devices are on each Windows release, with the devices behind each.

![OS builds](workspace/17-os-builds.png)

### 18. Security posture

*Devices.* Encryption, TPM 2.0, virtualization-based security and Credential Guard across Windows and macOS devices, with how many pass each check and what each device needs.

![Security posture](workspace/18-security-posture.png)

### 19. Stale and duplicate devices

*Devices.* Devices that have not checked in for a set number of days, and device names with more than one Intune record.

![Stale and duplicate devices](workspace/19-stale-and-duplicates.png)

### 20. Policy cleanup

*Policies.* Policies and apps that do nothing: assigned to deleted or empty groups, exclude-only, or not assigned at all.

![Policy cleanup](workspace/20-cleanup.png)

### 21. Duplicate policies

*Policies.* Pairs of policies that set the same settings to the same values. Intune only flags a conflict when the values differ, so these often go unnoticed.

![Duplicate policies](workspace/21-duplicate-policies.png)

### 22. Failed policies

*Policies.* Only the policies that have failures, with the failure percentage, conflicts included, and a Devices or Users switch.

![Failed policies](workspace/22-failed-policies.png)

### 23. Policy export

*Policies.* One policy's details, assignments and settings, written up as Markdown or CSV for a change record.

![Policy export](workspace/23-policy-export.png)

### 24. Recent changes

*Policies.* Policies, scripts and apps by when they were last changed or created, with who they are assigned to.

![Recent changes](workspace/24-recent-changes.png)

### 25. Setting check

*Policies.* Search every policy for a setting and see where it is configured, with its value and who it is assigned to. Spot the same setting set two ways.

![Setting check](workspace/25-setting-check.png)

### 26. App details

*Apps.* How an app is detected and what it requires, its install and uninstall commands, return codes, dependencies and assignments.

![App details](workspace/26-app-details.png)

### 27. App versions

*Apps.* Which versions of an app are out there, and the devices running the old ones.

![App versions](workspace/27-app-versions.png)

### 28. Failed apps

*Apps.* Only the apps that have failures, with the failure percentage and a Devices or Users switch.

![Failed apps](workspace/28-failed-apps.png)

### 29. Compare users

*Users and groups.* Pick two users and see which groups they share and which only one of them is in, direct or nested.

![Compare users](workspace/29-compare-users.png)

### 30. Group assignments

*Users and groups.* Everything that references a group, and whether it looks safe to retire: assignments, Conditional Access, licences, role assignments and more. Buttons for the built-in All devices and All users targets list what is assigned to them.

![Group assignments](workspace/30-group-assignments.png)

### 31. Group roster

*Users and groups.* A group's members with each device's primary user, compliance, OS and last check-in. Filter, then copy or save.

![Group roster](workspace/31-group-roster.png)

### 32. Orphaned users

*Users and groups.* Devices whose primary user is disabled or no longer exists, ready to reassign or retire.

![Orphaned users](workspace/32-orphaned-users.png)

### 33. User 360

*Users and groups.* One user: their devices, the groups they are in, and every policy, app and script that reaches them through those groups or All users, and why.

![User 360](workspace/33-user-360.png)

### 34. All reports

*Tenant.* Intune's own reports in one list, sorted by category, with search and a star for your favourites. Click one to open it in the admin center.

![All reports](workspace/34-all-reports.png)

### 35. Environment overview

*Tenant.* A one or two page summary of your devices with counts and percentages, saved as an HTML page to print to PDF, or copied as Markdown or CSV.

![Environment overview](workspace/35-environment-overview.png)

### 36. Error code lookup

*Tenant.* Type an error code or a few words to see its name, meaning and fix from Microsoft's published Intune, Entra and Windows error tables.

![Error code lookup](workspace/36-error-code-lookup.png)

### 37. ID decoder

*Tenant.* Paste an ID or an admin center link and find out what it is: device, group, user, policy, app, script and more.

![ID decoder](workspace/37-id-decoder.png)

### 38. Tenant health

*Tenant.* Tokens, certificates and connectors that stop things working when they lapse, with days left.

![Tenant health](workspace/38-tenant-health.png)

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
