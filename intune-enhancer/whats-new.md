# Intune Enhancer: what's new

**Note:** new versions may appear on this list before the extension stores have approved the update, so the version in the store can be older than the latest one here.

New features and fixes, newest first. Versions released on the same day are grouped.
Intune Enhancer is read-only: it never changes your tenant, and it only talks to Microsoft Graph.

## 1.47.0 to 1.69.0 - 1 November 2026
- **Settings picker shows what is already configured.** When you add settings to a policy, each setting already set in
  another policy shows "Set in N policies" after its name. Hover to see which policies. It uses the policy list that
  Setting check builds.
- **Dark theme by default.** The workspace now opens in the dark theme. If you have already picked a theme with the
  toggle, your choice is kept.
- **One footer on every tab.** What's new, Privacy policy and a Contact link, with the read-only note, now sit in one
  centred block at the bottom of every tab: at the bottom of the window on a short tab, and below the content on a
  long one.
- **"Related" button on devices.** A new command in a device page's toolbar shows the primary user's other
  devices and the groups the device is in.
- **"Used by" button on groups.** A new command beside Delete on a group's page opens the workspace on what
  uses that group.
- **Progress bar and Stop.** A bar along the bottom of the workspace shows what a long read is doing, with a
  count, a meter and the time so far, and a Stop button for the long ones.
- Compare users shows each person's sign-in name after their name, and device and policy searches list
  their matches alphabetically.
- **New tool, Compliance.** Ranks every compliance setting by how many devices fail it, worst first, and
  lists the devices failing any setting you pick, with copy and CSV export.
- **New menu.** The workspace's tools are now a sidebar grouped by Policies, Groups and users, Devices,
  Apps and Tenant, so they stay easy to find as more are added.
- **New tool, Policy export.** Find a policy by name and get its details, assignments and settings as
  Markdown or CSV, ready to paste into a change record.
- **New tool, Duplicate policies.** Lists policies that set the same settings to the same values, which
  Intune doesn't always flag as a conflict.
- **New tool, Hardware.** Memory, storage, TPM, BIOS, battery and more for every device in one sortable
  list, with copy and CSV export.
- **New tool, Compare devices.** Two devices side by side: their details, their groups, and which
  policies and apps reach one or both.
- **Activity light on the device page.** The coloured light now also appears beside "Last check-in time"
  on a device's own Overview page.

## 1.42.0 to 1.46.0 - 31 October 2026
- **New tool, Low storage.** Every device under 10 GB or 5 GB free, worst first, with CSV export.
- **New tool, Orphaned users.** Devices whose primary user has been disabled or deleted.
- **New tool, Tenant health.** Apple push certificate, VPP and ADE tokens, Managed Google Play and
  connectors, with the days left before each expires.
- **New tool, Device 360.** Everything that applies to one device and why, with the groups it and its
  primary user are in.
- **New tool, Compare users.** Two users' groups: the ones they share, and the ones only one of them is in.

## 1.35.0 to 1.39.0 - 30 October 2026
- **Remediations: dates and sort.** The Remediations list shows when each script package was
  created and last modified, with a Sort by dropdown (modified or created, newest first).
- **Activity light is sharper.** Green means checked in within the last 8 hours, yellow within 7
  days, orange within 30 days, red longer or never.
- Last check-in now reads "Checked in 5 hours ago" for the first day, then "3 days ago", so it
  matches the coloured light.
- **App versions:** the device list shows each device's primary user and last check-in, and a new
  button lists every device across all versions of an app.
- Fixed: App versions "List devices" showed no devices.

## 1.32.0 to 1.34.0 - 29 October 2026
- **Device quick facts: More details.** One click adds serial number, manufacturer, memory,
  storage, encryption, TPM, Windows edition, IP and MAC address, enrolment and join type.
- **New tool, App versions.** Search discovered apps to see every version in use and how many
  devices run each. Flag versions older than one you choose and list the devices on them, with
  copy and CSV export.
- New column width slider for the Script package name column.
- Fixed: a policy's failed count could be double what Intune's own Overview shows.
- Fixed: the group size pill in a policy's assignments could look empty.

## 1.23.0 to 1.31.0 - 28 October 2026
- **Policy status.** In Devices > Configuration, each policy shows how many devices it succeeded
  on and failed on. Click to open the policy. Choose all, failures only, or off.
- **Policy name width.** A new Settings slider widens the Policy name column.
- **Much faster pills.** Policy, app and group counts load in a fraction of the time and are
  remembered for 30 minutes, so each visit no longer starts from scratch.
- A fresh neon sky blue look across the pills, icon and dark theme.
- Pills are easier to read on the portal's light and dark themes, and plain pills blend with the
  row's hover and selection colours. Empty group pills turn the same pink as a failed app or
  policy.
- Settings: the four column width sliders sit two to a row.
- Fixed: dragging the App name column now moves the rows as you drag, not only on release.
- Fixed: Cleanup could treat a group it couldn't size as not empty. It now tells you how many it
  couldn't check.
- Fixed: Setting check could say "not configured" when Intune hadn't returned a template.
- Fixed: a check-in time slightly ahead of your clock showed "-1 days ago".
- Fixed: overlapping searches (Setting check, Group impact, Group roster) could show an older
  answer over a newer one.
- Fixed: Settings sliders jumping back while the device list was first loading.
- Fixed: switching tenants during a list build could leave the list empty.
- Fixed: Friendly OS versions could keep a stale tooltip when a list row was reused.

## 1.10.0 to 1.22.0 - 27 October 2026
- **Settings tab** with a plain-language disclosure and per-feature switches. A new install opens
  on it, so nothing runs until you agree. It also shows your session and device list status, with
  Refresh device list and Clear stored data buttons.
- **App install status.** App lists show how many devices installed each app and how many
  failed. Click to open the app. Choose all, failures only, or off.
- **Column width sliders** for Device name, Group name and App name columns. The width you drag to
  in the portal is saved.
- **Activity light** gets four colour steps that match how stale a device is.
- **Group impact and Group roster** search with Enter or a Search button.
- **ID decoder** identifies what an ID copied from a portal link points to.
- Last logged-on user is a small person icon after the device name.
- Group size pills open the group when clicked.
- Filter rules show on hover, and refresh as filters change.
- The toolbar icon opens the workspace straight away (no popup), reusing a workspace tab that's
  already open.
- Smoother scrolling in long lists, and in-portal colours follow the portal's light or dark theme.
- Settings uses dropdowns and grouped sections, and an "off" note and toolbar badge show until you
  turn the extension on.
- Renamed to Intune Enhancer, with a new icon.
- Fixed: the first request straight after agreeing could be refused as "turned off".

## 0.1.0 to 1.9.0 - 24 to 26 October 2026
- **Workspace tools** in a full browser tab, with light and dark themes: Setting check, Group
  impact, Group roster, OS builds, Stale and duplicate devices, Cleanup, ID decoder.
- **Recent changes.** Every policy, profile, script and app by modified or created date.
- **Deprecated settings finder.** Lists configured settings Intune has marked deprecated. Setting
  check also explains why fewer policies are searched than listed: apps, scripts and similar have
  no settings.
- **Device lists:** primary user labels where a list doesn't show one, an activity light and
  compliance shield before device names (the shield hides where Intune already has a Compliance
  column), a low storage flag (orange under 10 GB, red under 5 GB), and the last logged-on user
  when it isn't the primary user.
- **Device quick facts.** Click a label for a card with compliance, OS, last check-in, enrolment,
  ownership and model, plus Open in Intune. An icon on group member rows jumps to the device's
  Intune record.
- **Friendly OS versions.** `10.0.26100.4349` reads as `Win11 24H2 (26100.4349)`.
- **Group size hints and links** in policy and app assignment tables, in a slim column just past
  the table, lined up with each row and readable on the dark theme. The Group column opens 50%
  wider and can be dragged narrower or wider, with every row following.
- Full device names instead of cut-off ones, and the activity light sits in the Last check-in
  column where there is one.
- Policy and app links open the right page in Intune.
