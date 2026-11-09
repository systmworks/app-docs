<p align="center"><a href="https://buymeacoffee.com/systmworks"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="45" alt="Buy me a coffee"></a></p>

> I have spent many, many hours creating and testing this. If it helps you please consider buying me a Coffee :)

# Intune Enhancer: what's new

**Note:** new versions may appear on this list before the extension stores have approved the update, so the version in the store can be older than the latest one here.

New features and fixes, newest first. Versions released on the same day are grouped.
Intune Enhancer is read-only: it never changes your tenant, and it only talks to Microsoft Graph.

## 2.78.0 to 2.87.0 - 9 November 2026
- **Secure Boot removed for now (2.87.0).** Security posture no longer lists Secure Boot, because Intune does not
  report it reliably through this route. It will come back once it can be read correctly.
- **Same value in several policies (2.86.0).** Device 360's settings list can now show the settings that several
  policies set to the same value, as well as the conflicts where they differ.
- **Security posture in A to Z order (2.85.0).** The checks are listed alphabetically, with Ready for encryption just
  before Encrypted.
- **Fewer false conflicts (2.84.0).** Device 360's settings list no longer calls these conflicts: several entries of one
  list in one policy, several certificate, VPN or Wi-Fi profiles, or compliance policies.
- **Fix (2.83.0).** Security posture and the Hardware report now show each device's TPM version and Secure Boot state,
  which Intune was not sending before; a device with an older TPM is listed as "TPM 1.2". Read the report again after
  updating.
- **Fix (2.82.0).** In Device 360's settings list and Setting check, a very long value (such as a certificate) is cut
  short so every column fits; Copy table and Save CSV still hold the whole value.
- **Easier to read counts (2.81.0).** In Security posture and Baseline gap, counts of zero are greyed out, so the
  ones that need a look keep their colour.
- **Fix (2.80.0).** Windows update rings no longer show a "not in Intune" label beside their names.
- **Version in the header (2.79.0).** The workspace shows its version beside the Intune Enhancer name at the top
  left, instead of in the footer.
- **Error code lookup updated (2.78.0).** One more Microsoft sign-in error code is now explained.

## 2.53.0 to 2.77.0 - 8 November 2026
- **Tidier code (2.77.0).** Shared code in place of a few copies. Nothing looks or works differently.
- **Update check (2.76.0).** The OS builds tab can now show which Windows devices are behind on updates: each release
  is checked against the newest build on your devices, or a build you type, with the devices that are behind listed
  and ready to copy or save.
- **Tidier sidebar (2.75.0).** The tools in the workspace sidebar sit closer together, and the sidebar's scrollbar only
  appears while the pointer is over it.
- **Small fixes (2.74.0).** Security posture's encryption issues read in plain sentence case; Hardware dates stay on
  one line; badges and check-in lights on the Device 360 and User 360 cards sit inline; User 360 marks a device that
  has two Intune records; and the sample tenant's groups and hardware are more consistent.
- **User 360 (2.73.0).** A new tool under Users and groups: pick a user to see their devices, the groups they are in,
  and every policy, app and script that reaches them through their groups or All users, and why.
- **More in the Environment overview (2.72.0).** The overview now shows how many devices have the firewall on, from
  your compliance policies' firewall check, and how many apps and policies are assigned or not. Build overview now
  gathers everything itself, including each device's security details the first time, so there is no need to run
  another report first.
- **Group assignments sees nested groups (2.71.0).** When a group is a member of other groups, Group assignments now
  also lists the policies, apps and scripts assigned to those parent groups, which its members get too, and which
  group each comes through. A group with nothing assigned directly no longer looks unused.
- **Environment overview (2.70.0).** A new report under Reports: a one or two page summary of your devices, with
  counts and percentages by platform and release, manufacturer and model, compliance, encryption, last check-in,
  ownership, join type and Autopilot, plus TPM, Secure Boot and Credential Guard once the Hardware report has been
  read. Save it as an HTML page and print that to PDF, or copy it as Markdown or CSV.
- **Security posture (2.69.0).** A new tool under Devices: encryption, TPM 2.0, Secure Boot, virtualization-based
  security and Credential Guard across your Windows and macOS devices, with how many pass each check and what each
  device needs attention for. It shares the Hardware report's read, so running either one fills both.
- **Device explorer (2.68.0).** A new tool under Devices: every device in one table with the columns you choose,
  such as ownership, join and enrolment type, manufacturer, encryption and when the management certificate expires.
  Filter, sort by any heading, and copy or save what you see. It loads the whole list, not the first few hundred.
- **App details (2.67.0).** A new App details tool under Apps: find an app and see how it is detected and what it
  requires (including the text of a detection or requirement script), its install and uninstall commands, return
  codes, the apps it depends on or supersedes, and its assignments. Copy it as Markdown or save it as CSV.
- **Why this setting? (2.66.0).** Device 360 now lists every setting that reaches the device, which policy sets it
  and why that policy reaches the device. Where two policies set the same setting to different values, it is marked
  as a conflict. Show only conflicts or everything, filter the list, and copy or save it.
- **Filter checks in Cleanup (2.65.0).** Cleanup now also checks assignment filters: assignments that still name a
  filter that was deleted, filters nothing uses, and for every filter, the policies, apps and scripts that use it.
- **2.64.0.** Behind the scenes: every colour now comes from one theme, ready for more themes later. In the admin
  center's dark theme, the activity dots on the Related card now match the ones in device lists.
- **2.63.0.** When you limit the workspace to one device group, Compare devices and the device lists in App versions
  now show only that group's devices too. All reports has Enrollment and Other quick filters.
- **2.62.0.** Behind the scenes: the workspace page is smaller, with its search boxes and Copy table / Save CSV
  buttons built one way everywhere.
- **2.61.0.** The tool list on the left is a little wider, so every tool name fits on one line.
- **Tidier reports (2.59.0).** Numbers line up in the centre of their columns, report pages use more of the window,
  and results no longer sit right against the button above them. Hardware shows users by name, in the CSV too;
  Compliance breakdown shows them by name (the full address is still in its CSV). App versions highlights "List all devices".
- **2.58.0.** Remediation dates and sort is now off until you turn it on in Settings.
- **Try it on a sample tenant (2.57.0).** A new Demo on sample tenant button at the top of the workspace shows every
  tool working on a fictional company, without touching your tenant. Leave demo takes you back.
- **2.56.0.** Autopilot failures no longer names a lower-priority enrollment status page as expected when it can't
  tell whether a higher-priority page targets the device; it says it can't tell.
- **2.55.0.** Autopilot failures no longer says the Default enrollment status page applies when it can't read another
  page's assignments. Baseline gap and Duplicate policies say when only part of a policy's settings could be read.
  Device 360 and Compare devices open faster, and very large tenants use less memory while reading policies.
- **2.54.0.** Device lists in the admin center redraw with less work while you scroll, and primary user labels
  refresh properly after the feature is turned off and on again.
- **2.53.0.** Friendly names for custom (OMA-URI) settings were removed, making the download about 225 KB smaller.
  Setting check and Policy export no longer show a name and description for them; search them by their path as before.

## 2.40.0 to 2.52.0 - 7 November 2026
- **2.52.0.** Cleanup has a Copy table button like the other reports. Tenant health and Orphaned users grey their
  button while they read. Compliance breakdown says when it shows only the first 2,000 devices.
- **2.51.0.** Behind the scenes: shared code for running searches and reports, with more of it tested. If you look up
  two IDs in quick succession in the ID decoder, you now always see the answer to the second.
- **Matching cards (2.50.0).** Device quick facts and the Related card now look the same, with a blue edge like the
  extension's buttons, on both the light and dark admin center themes.
- **Easier dates (2.49.0).** Check-ins and changes read the same way everywhere: "yesterday", "3 days ago", "2 weeks
  ago", "4 months ago", instead of counting days into the hundreds.
- **2.48.0.** Policy export no longer shows a 1970 date for a policy Intune gives no real date for. Compliance states
  read the same in the workspace as in the admin center's quick facts card.
- **2.47.0.** Behind the scenes: every report table is drawn the same way, so they look and behave alike.
- **2.46.0.** Device quick facts and the Related card share one way of opening and closing, so only one is open at a
  time.
- **One way to search (2.45.0).** Every search box now finds rows that hold all the words you type, in any order, so
  "ann laptop" finds Ann's laptop in Group roster, Recent changes, Autopilot failures and the device and policy
  searches, as it already did in All reports and Setting check. Put words in quotes to keep a phrase together.
- **2.44.0.** The Settings disclosure lists everything the extension reads, with a link to the privacy policy. Stopping
  the Hardware report no longer replaces the last saved full report.
- **Tidier workspace (2.43.0).** Reset to defaults is now a button in the top bar, next to Settings, and asks before
  it does anything. Where the extension's data comes from is under Credits in the footer.
- **Clearer credits (2.42.0).** The Settings page says more precisely where setting descriptions come from: adapted
  from Microsoft Learn and Microsoft's published files, with Microsoft Learn text used under CC BY 4.0.
- **More fixes (2.41.0).** Clear stored data clears everything even while a list is still being read. A click on a
  column's edge no longer changes its saved width. Compare devices and Compare users forget a pick when you type in
  its box. For US Government clouds, the additions in the admin center are set up properly once you allow the
  cloud. In Firefox, the install screen now also lists personal information (names and email addresses), which the
  extension sends only to Microsoft Graph.
- **Fixes.** Group sizes, app install counts and policy status counts now really do refresh after 30 minutes in an
  admin center tab left open for a long time. Saved and copied tables keep negative numbers as numbers (for example
  days left on an expired token in Tenant health). The Autopilot failures filter runs when you press Enter, like the
  other searches. While the extension is turned off, the workspace opens straight on Settings without showing an
  error first.
- **Data sources.** The Settings page now credits where the error codes, custom setting names and baselines come from.

## 2.35.0 to 2.39.0 - 6 November 2026
- **Star your favourites.** Click the star beside a report in All reports, then use the Starred button to see only
  those. Every tool in the workspace's sidebar has a star too, and "Starred only" at the top of the sidebar hides the
  tools you haven't starred, keeping the headings. The sidebar is a little wider.
- **Reset all settings to defaults.** A link at the foot of the Settings tab puts every switch, dropdown, column width,
  star and the theme back to how they were at install. It asks first, and nothing you have stored is deleted.
- **Updating keeps your settings.** Store installs keep them through every update. For a manual install, extract the
  new version over the same folder and reload the extension; the download page explains how.
- **Fixes.** Group sizes and app install counts refresh in an admin center tab left open for a long time. After the
  extension updates, an already-open admin center tab no longer shows a "Dates couldn't be read" note on the
  Remediations list (reload the tab to get the new version). Autopilot failures says it can't tell which enrollment
  status page applies, instead of guessing, for users in very many groups. Clear stored data also clears what the
  workspace was showing, and the ID decoder spaces policy type names properly. Long reports say the same thing when
  they show only part of a list ("Showing the first N of M. Copy and Save CSV include all.").

## 2.4.0 to 2.34.0 - 5 November 2026
- **Fixes.** In Firefox, the Group roster row filter and the App versions "older than" box now apply when you press
  Enter. Settings catalog policies for macOS, iOS and Android open in the right place. Changing the workspace scope
  while devices are loading no longer shows the wrong devices. Compare users keeps the names of the users it compared.
  The workspace copes better when Microsoft Graph is briefly unavailable, and the dark theme's sidebar highlights the
  selected tab again. Orphaned users and Tenant health no longer start a second scan if you click Run twice, and a
  policy export says when a policy's settings couldn't be read.
- **All reports.** A new Reports section in the workspace lists about 50 of Intune's own reports in one place, sorted
  by category and then by name. Click a name to open that report in the Intune admin center. Narrow the list with the
  All, Apps, Compliance, Configuration, Security and Updates buttons, or type three or more letters to search. Nothing is
  read from your tenant to build it.
- **Advanced (experimental) settings.** The Settings card for new and not yet widely tested options is now called
  Advanced (experimental). Baseline gap, Workspace scope and US Government clouds are there.
- **Baseline gap (experimental).** Turn it on under Settings > Advanced (experimental) for a new tool under Devices. Pick a Windows device and a Microsoft security baseline (Windows 11,
  Microsoft 365 Apps or Edge) to see, for each recommendation, whether a policy that reaches the device sets it as
  recommended: Matches, Different, Conflict, Check value or Not configured. It is judged from your Intune policies, so
  Group Policy and scripts are not seen. Save the result as CSV or JSON.
- **Error code lookup.** Type an error code or a few words to see its name, meaning and fix from Microsoft's published
  Intune, Entra and Windows error tables. Works offline, and Autopilot failures shows the codes in each event.
- **Scope the workspace to a device group.** Responsible for one site or team in a big tenant? Turn on Workspace scope
  under Settings > Advanced (experimental), then pick a device group with Scope at the top of the workspace. OS builds, Stale &
  duplicates, Low storage, Hardware, Orphaned users, the device searches and the list of devices failing a compliance
  setting then show only that group's devices (nested groups included). The scope is kept until you clear it with the x.
  It only filters what the workspace shows: nothing in Intune changes.
- **Autopilot failures.** A new report under Devices for troubleshooting failed Autopilot deployments. It lists the
  last 1 to 30 days (7 by default) of Autopilot events, with one search box for host name, serial number or user.
  Open Details on a row for everything Intune reports about it, including the enrollment status page apps and
  policies and the device's Autopilot record. Copy the table or save it as CSV or JSON. New and not yet tried on a
  live tenant.
- **Failed apps and Failed policies.** Two new reports in the workspace, under Apps and Policies. Each lists only the
  apps or policies that have failures, with the failure percentage, and a Devices / Users switch (one at a time).
  Choose a minimum number of fails and a platform. Failed policies also shows conflicts. Click a heading to sort,
  then copy the table or save it as CSV. These are new and not yet tried on a live tenant.
- **Sort the Remediations list by more.** The Sort by menu on the Remediations list now also sorts by Author,
  Status, Without issues, With issues, Issue fixed, Recurred and Total remediated (when the list shows them).
- **Low storage sorts by heading.** Click any column heading to sort, like the Hardware report.

## 1.91.0 to 2.3.0 - 4 November 2026
- **Group assignments.** The Group impact tab is now called Group assignments. It has new All devices and All users
  (licensed) buttons that list every policy, app and script assigned to those built-in targets, with intent and filter.
- **Same export buttons everywhere.** Copy table and Save CSV now appear on every report once it has results, and
  Group assignments has Copy table too.
- **Tidier Compare tabs.** The two search boxes on Compare devices and Compare users have a small gap between them.
- **Version 2.** A new look for the Settings tab, with switches, short descriptions and an i for the full
  explanation, and optional support for the US Government clouds (GCC High and DoD, not yet tried on a
  government tenant). It includes every fix below.
- **Fixes across the workspace.** The Stop button on the progress bar works, administrative template policies are
  compared by the values set inside them, Duplicate policies copes with very large tenants, Clear stored data also
  clears what the reports show, and new policies get their status in the Configuration list within minutes.
- **Lighter on long lists.** Friendly OS versions and Low storage flags do less work while you scroll, and group and
  user search now show the real reason when a search fails.
- **More reliable.** Admins who switch between tenants stay on the right one, settings changed at the same moment
  are all kept, labels come back by themselves after a hiccup, big policies are fully checked in Setting check, and
  Copy table is safe to paste into Excel.
- **Settings tab fixes.** Clicking a setting's name turns it on or off again, the explanation card closes when you
  follow its link or resize the window, and the switches draw properly in Firefox.
- **A tidier Settings tab.** Tick-boxes are now toggles, descriptions are shorter (hover or click the i for the full
  explanation), and settings are grouped by what they do. The footer shows the version you have installed.
- **US Government clouds (experimental).** Settings has one switch to allow GCC High and DoD tenants. The browser asks
  for access to those clouds' Intune admin center and Microsoft Graph addresses only, checked against Microsoft's
  documentation, and nothing changes for anyone who does not use it. It has not been tried on a government tenant
  yet: feedback is welcome.
- **New device view switch.** Settings has a New device view switch (on by default). Off, the extension's open-device
  links use the old device view address instead.

## 1.86.0 - 3 November 2026
- **A "fetching stats" note while pills load.** When the app and policy pills take more than a second to arrive, a
  small "Intune Enhancer: fetching stats..." note shows at the bottom right of the page and disappears when they are
  drawn. It never blocks a click.

## 1.79.0 - 2 November 2026
- **The browser now enforces "Graph only".** The extension's manifest limits its connections to Microsoft Graph, so a
  request to any other site is blocked by Chrome or Edge itself, not just left out of the code.

## 1.47.0 to 1.76.0 - 1 November 2026
- **Clear stored data now clears the Hardware report too.** The saved report (serial numbers, IP and MAC addresses)
  is deleted with the device and policy lists. The privacy policy is updated to describe everything the extension
  reads and keeps.
- **Our buttons look like ours.** The Related and Used by commands are now outlined pills with a blue border, like the
  other additions, so they are easy to tell from Intune's own buttons.
- **Settings picker shows what is already configured.** When you add settings to a policy, each setting already set in
  another policy shows "Set in N policies" after its name. Hover to see which policies. It only works after you have run a search in Setting check,
  which builds the policy list it reads.
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

## 0.1.0 to 1.9.0 - October 2026
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

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
