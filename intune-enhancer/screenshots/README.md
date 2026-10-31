# Intune Enhancer screenshots

Every screenshot is the real extension on a fictional tenant (Fabrikam). Nothing here is from a real tenant. Listed highest benefit first; the folders group them by where they appear.

## 1. Devices list

*In the admin center.* Each device shows its primary user, a green, yellow, orange or red check-in light and a flag when free storage is low, right in the admin center's own list.

![Devices list](admin-center/01-devices-list.png)

## 2. Group lists

*In the admin center.* How many devices, users and groups each group holds, beside its name. Empty groups say so.

![Group lists](admin-center/02-groups-list.png)

## 3. Policy lists

*In the admin center.* The number of devices that succeeded and failed sits next to each policy's name, so a failing policy stands out without opening it.

![Policy lists](admin-center/03-policies-list.png)

## 4. App lists

*In the admin center.* The same succeeded and failed counts next to each app.

![App lists](admin-center/04-apps-list.png)

## 5. Adding members to a group

*In the admin center.* In the Add members picker each device shows its primary user and check-in light, so you pick the right one.

![Adding members to a group](admin-center/05-add-members.png)

## 6. Device 360

*Devices.* Every policy, app and script that reaches one device, and why: which group, whether it is excluded, or depends on a filter.

![Device 360](devices/06-device-360.png)

![Device 360 (dark)](devices/06-device-360-dark.png)

## 7. Setting check

*Policies.* Search every policy for a setting and see where it is configured, with its value and who it is assigned to. Spot the same setting set two ways.

![Setting check](policies/07-setting-check.png)

![Setting check (dark)](policies/07-setting-check-dark.png)

## 8. Group impact

*Users and groups.* Everything that references a group, and whether it looks safe to retire: assignments, Conditional Access, licences, role assignments and more.

![Group impact](users-and-groups/08-group-impact.png)

![Group impact (dark)](users-and-groups/08-group-impact-dark.png)

## 9. Compliance breakdown

*Devices.* Which compliance settings fail on the most devices, worst first, with the devices behind each one.

![Compliance breakdown](devices/09-compliance-breakdown.png)

## 10. Recent changes

*Policies.* Policies, scripts and apps by when they were last changed or created, with who they are assigned to.

![Recent changes](policies/10-recent-changes.png)

## 11. Policy cleanup

*Policies.* Policies and apps that do nothing: assigned to deleted or empty groups, exclude-only, or not assigned at all.

![Policy cleanup](policies/11-cleanup.png)

![Policy cleanup (dark)](policies/11-cleanup-dark.png)

## 12. Duplicate policies

*Policies.* Pairs of policies that set the same settings to the same values. Intune only flags a conflict when the values differ, so these often go unnoticed.

![Duplicate policies](policies/12-duplicate-policies.png)

## 13. Compare users

*Users and groups.* Pick two users and see which groups they share and which only one of them is in, direct or nested.

![Compare users](users-and-groups/13-compare-users.png)

## 14. Policy export

*Policies.* One policy's details, assignments and settings, written up as Markdown or CSV for a change record.

![Policy export](policies/14-policy-export.png)

## 15. Compare devices

*Devices.* Two devices side by side: details, groups, and which policies, apps and scripts reach one or both.

![Compare devices](devices/15-compare-devices.png)

## 16. Low storage

*Devices.* Devices with little free disk space, least free first.

![Low storage](devices/16-low-storage.png)

## 17. Stale and duplicate devices

*Devices.* Devices that have not checked in for a set number of days, and device names with more than one Intune record.

![Stale and duplicate devices](devices/17-stale-and-duplicates.png)

## 18. Orphaned users

*Users and groups.* Devices whose primary user is disabled or no longer exists, ready to reassign or retire.

![Orphaned users](users-and-groups/18-orphaned-users.png)

## 19. Group roster

*Users and groups.* A group's members with each device's primary user, compliance, OS and last check-in. Filter, then copy or save.

![Group roster](users-and-groups/19-group-roster.png)

## 20. Hardware report

*Devices.* Memory, storage, TPM, BIOS and more for every device, sortable, and saved as CSV.

![Hardware report](devices/20-hardware.png)

## 21. App versions

*Apps.* Which versions of an app are out there, and the devices running the old ones.

![App versions](apps/21-app-versions.png)

## 22. OS builds

*Devices.* How many devices are on each Windows release, with the devices behind each.

![OS builds](devices/22-os-builds.png)

## 23. Tenant health

*Tenant.* Tokens, certificates and connectors that stop things working when they lapse, with days left.

![Tenant health](tenant/23-tenant-health.png)

## 24. ID decoder

*Tenant.* Paste an ID or an admin center link and find out what it is: device, group, user, policy, app, script and more.

![ID decoder](tenant/24-id-decoder.png)

## 25. Settings

*The extension.* A switch for every addition to the admin center, so each can be turned off.

![Settings](extension/25-settings.png)
