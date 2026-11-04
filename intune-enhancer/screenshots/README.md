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

### 10. Compare devices

*Devices.* Two devices side by side: details, groups, and which policies, apps and scripts reach one or both.

![Compare devices](workspace/10-compare-devices.png)

### 11. Compliance breakdown

*Devices.* Which compliance settings fail on the most devices, worst first, with the devices behind each one.

![Compliance breakdown](workspace/11-compliance-breakdown.png)

### 12. Device 360

*Devices.* Every policy, app and script that reaches one device, and why: which group, whether it is excluded, or depends on a filter.

![Device 360](workspace/12-device-360.png)

### 13. Hardware report

*Devices.* Memory, storage, TPM, BIOS and more for every device, sortable, and saved as CSV.

![Hardware report](workspace/13-hardware.png)

### 14. Low storage

*Devices.* Devices with little free disk space, least free first.

![Low storage](workspace/14-low-storage.png)

### 15. OS builds

*Devices.* How many devices are on each Windows release, with the devices behind each.

![OS builds](workspace/15-os-builds.png)

### 16. Stale and duplicate devices

*Devices.* Devices that have not checked in for a set number of days, and device names with more than one Intune record.

![Stale and duplicate devices](workspace/16-stale-and-duplicates.png)

### 17. Policy cleanup

*Policies.* Policies and apps that do nothing: assigned to deleted or empty groups, exclude-only, or not assigned at all.

![Policy cleanup](workspace/17-cleanup.png)

### 18. Duplicate policies

*Policies.* Pairs of policies that set the same settings to the same values. Intune only flags a conflict when the values differ, so these often go unnoticed.

![Duplicate policies](workspace/18-duplicate-policies.png)

### 19. Policy export

*Policies.* One policy's details, assignments and settings, written up as Markdown or CSV for a change record.

![Policy export](workspace/19-policy-export.png)

### 20. Recent changes

*Policies.* Policies, scripts and apps by when they were last changed or created, with who they are assigned to.

![Recent changes](workspace/20-recent-changes.png)

### 21. Setting check

*Policies.* Search every policy for a setting and see where it is configured, with its value and who it is assigned to. Spot the same setting set two ways.

![Setting check](workspace/21-setting-check.png)

### 22. App versions

*Apps.* Which versions of an app are out there, and the devices running the old ones.

![App versions](workspace/22-app-versions.png)

### 23. Compare users

*Users and groups.* Pick two users and see which groups they share and which only one of them is in, direct or nested.

![Compare users](workspace/23-compare-users.png)

### 24. Group assignments

*Users and groups.* Everything that references a group, and whether it looks safe to retire: assignments, Conditional Access, licences, role assignments and more. Buttons for the built-in All devices and All users targets list what is assigned to them.

![Group assignments](workspace/24-group-assignments.png)

### 25. Group roster

*Users and groups.* A group's members with each device's primary user, compliance, OS and last check-in. Filter, then copy or save.

![Group roster](workspace/25-group-roster.png)

### 26. Orphaned users

*Users and groups.* Devices whose primary user is disabled or no longer exists, ready to reassign or retire.

![Orphaned users](workspace/26-orphaned-users.png)

### 27. ID decoder

*Tenant.* Paste an ID or an admin center link and find out what it is: device, group, user, policy, app, script and more.

![ID decoder](workspace/27-id-decoder.png)

### 28. Tenant health

*Tenant.* Tokens, certificates and connectors that stop things working when they lapse, with days left.

![Tenant health](workspace/28-tenant-health.png)

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
