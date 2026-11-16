<p align="center"><a href="https://buymeacoffee.com/systmworks"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="45" alt="Buy me a coffee"></a></p>

> I have spent many, many hours creating and testing this. If it helps you please consider buying me a Coffee :)

# AVD Enhancer: what's new

**Note:** new versions may appear on this list before the extension stores have approved the update, so the version in the store can be older than the latest one here.

## 1.5.0 to 1.21.0 - 16 November 2026
- **Clearer Size and cost note (1.21.0).** The note under the Size and cost table is now four short lines that say what Running and Idle mean, where the price comes from, that the costs assume a full 24 hours (scaling plans make the real cost lower) and when your Settings rate is used.
- **Idle cost uses Microsoft's prices (1.20.0).** The Idle hosts tile on the Dashboard now works out its cost a day from Microsoft's public price for each VM size (in the currency you pick in Settings), so you no longer need to type an hourly rate. The rate in Settings is only used for a host where no price is found.
- **Running cost per day (1.19.0).** The Size and cost table has a new column for what the hosts that are on would cost over a full day, next to the idle cost. Scaling plans switch hosts off, so the real cost is lower. The first-run disclosure now says the extension asks Microsoft's public price list for VM prices.
- **Real VM prices in Size and cost (1.18.0).** The Size and cost report now looks up Microsoft's public pay-as-you-go hourly price for each VM size in each region and uses it for the idle cost; the hourly rate in Settings is used only where no price is found. The table shows the price an hour. Settings lets you pick the currency (USD by default); Microsoft converts the price, nothing else is used. Prices are list prices and a rough guide only. The table now has a row for each size in each region.
- **Wider Pools table (1.17.0).** The tiles on the Dashboard are a little narrower, which gives the Pools table more room, and the table no longer has a sideways scrollbar: a long pool name is cut short with an ellipsis (hover for the full name).
- **Sidebar sorted A to Z (1.16.0).** The tools in each sidebar section are in alphabetical order, and All reports is now the first item under Reports.
- **Four more reports (1.15.0).** Reports now has Capacity (sessions against capacity, pool by pool), Versions (agent and OS builds, and hosts on an old agent), Size and cost (VM sizes, idle hosts and a rough daily cost from the hourly rate you set in Settings) and Coverage (pools without a scaling plan and hosts without a maintenance window). Each has charts, a table, Copy Markdown and Save HTML.
- **Reports (1.14.0).** The sidebar has a new Reports section. Fleet health shows how many hosts are on, which need attention and why, with bar charts and a table, for the subscription you picked on the Dashboard; Copy Markdown and Save HTML write it out. All reports lists the reports in AVD Enhancer and links to Azure's own reports for Azure Virtual Desktop (Insights, workbooks, Cost analysis, Advisor, Policy and more). More reports are coming.
- **Pool quick links (1.13.0).** Settings has a new Sidebar pool links card: pick up to six host pools and they appear under a Pools heading in the sidebar. A link opens the Dashboard on just that pool. The Pools heading folds like the others.
- **Wider sidebar, folding sections (1.12.0).** The left sidebar is a little wider. Click a heading (Monitor, Tools) to fold its tools away and click again to open them; the tool you are on stays visible, and AVD Enhancer remembers which sections you folded.
- **Six themes (1.11.0).** The theme button now opens a menu of six themes: Light (Blue, Grey, Pink) and Dark (Blue, Green, Red). Your earlier light or dark choice carries over.
- **Tidy-up (1.10.0).** Internal clean-up: the page's code is split into smaller files. Nothing changes in how AVD Enhancer looks or works.
- **New icon colours (1.9.0).** The icon's grid of host-health squares now has one green square, with blue and yellow beside the amber and red ones.
- **Keyboard and screen readers (1.8.0).** The tools in the sidebar can now be moved through with the arrow keys (Up and Down, Home and End), only the open tool takes a Tab stop, and screen readers hear each tool and its page properly named.
- **Fixes (1.7.0).** The Capacity used tile no longer says all hosts are off when hosts are on but their pool limits could not be read. Two refreshes in a row can no longer show an older answer after a newer one, or leave the Refresh button disabled. Exported CSV files now also guard a formula hidden behind a leading tab.
- **Tidy-up (1.6.0).** Internal clean-up and extra safety checks; nothing changes in how AVD Enhancer looks or works.
- **Fix (1.5.0).** Scan sessions and Check my access now tell you when they leave something out. A scan reads the first 300 hosts and Check my access the first 40 resource groups; before, the rest were dropped without a word.

## 1.0.0 to 1.4.0 - 14 November 2026
- **Fix (1.1.0).** After the extension was updated, an Azure portal tab that was already open showed no sign-in until you reloaded it. The extension now picks the sign-in up in the open portal tabs straight after an update.
- **AVD Enhancer 1.0.0: the first public release.** Everything under Initial development below, in one version: the Dashboard with its tiles, pool list and host table, host and pool details, scan sessions, Inventory with scaling plans and maintenance windows, Tags, PIM roles, Check my access, custom cards, saved views and exports, stars, light and dark themes, and the new icon. It is read-only, talks only to Azure, and sends no data to the developer.

## Initial development
Versions 0.1.0 to 0.39.0, built before the first public release.
- **New icon (0.39.0).** The extension has a new icon: a monitor showing the pool as a grid of green, amber and red host-health squares.
- **Fix (0.38.0).** A host's details now link to the host's virtual machine in the Azure portal ("Open VM in Azure portal") as well as to its session host entry in Azure Virtual Desktop. The single link used to open only the session host entry.
- **Try Intune Enhancer (0.37.0).** A card at the bottom of the sidebar links to Intune Enhancer, my companion extension for Microsoft Intune, in the store that matches your browser (Chrome Web Store, Edge Add-ons or Firefox Add-ons).
- **Spacing (0.36.0).** There is more space between the stacked tables on Inventory, so each title no longer crowds the table above it.
- **Custom cards (0.35.0).** Custom cards now sit in a third row under the eight tiles, so the tiles stay where they are and the pool list grows to match. The card choices are Session hosts and Hosts with a tag, as the other numbers are already tiles.
- **Fix (0.35.0).** The pool list shows five pools at a time again: the name and the details button are on one line.
- **Sidebar stars (0.34.0).** Star the tools you use most with the star beside each name, then press Starred only to show just those. Your stars are remembered.
- **Pool and scaling plan details (0.33.0).** Click a pool on Inventory, a scaling plan on the schedules table, or the small i beside a pool on the Dashboard to open its details on the right: the pool's type, size mix, scaling plan, application groups and hosts, or the plan's time zone, pools and schedules. Click a host in the list to open it.
- **Scaling plans (0.33.0).** The separate Scaling plans table on Inventory is gone: the plan's time zone and pools are now columns of the Scaling plans and schedules table.
- **Tidier tables and top bar (0.32.0).** The Save HTML, Copy table and Save CSV buttons are small icons (hover for the name) and only appear on tables worth exporting, so the Dashboard pool list shows more pools. Reset to defaults moved into the Settings page heading. Demo sits next to Settings, and the account and Refresh are spaced evenly across the top bar. Opening another tab closes the host details panel.
- **PIM roles (0.32.0).** New Reader, Contributor and Operator pills, and the Eligible label on a role opens the Azure page where you activate it.
- **Fix (0.30.0).** Errors on the Inventory tab now link to the Azure portal when the cause is a missing sign-in, like errors elsewhere.
- **PIM roles (0.29.0).** A new PIM roles tab, under Tools, lists the Azure roles you hold now and the ones you can activate, with Active now and Eligible pills, how long an activation has left and when your eligibility ends. It only reads: activate roles in the Azure portal. Entra directory roles and group roles are not shown.
- **Dashboard cards (0.28.0).** Settings can add up to four cards in a row above the Dashboard tiles. Each shows a built-in number (such as Idle hosts or Session hosts) or how many hosts have a tag you name, with an optional value. Click a tag card to see those hosts.
- **Tags tab (0.28.0).** Lists every tag on the VMs behind your session hosts, with how many hosts have each. Pick a tag to list its hosts, then narrow by value with pills (the tag set, each value such as True or False, or not set). Click a host to open its details, which now include its tags.
- **Maintenance windows (0.27.0).** Inventory has a new Maintenance windows table of your Azure maintenance configurations: the days, start, end, length and time zone, and how many VMs and AVD hosts each one covers. When you open a host, its details show its maintenance window. Windows applied through a dynamic scope are not listed.
- **Scaling plan schedules (0.27.0).** Inventory has a new Scaling plan schedules table: the days, and the ramp-up, peak, ramp-down and off-peak times of every schedule, and whether users are logged off at ramp-down.
- **Left sidebar (0.26.0).** The Dashboard, Inventory, Tags, PIM roles, Links and Console tabs moved from the top bar to a sidebar. The signed-in account is now centred in the top bar. The selected tab is highlighted again.
- **Fix (0.25.0).** The Application groups table on Inventory failed with "Query is invalid". It loads again.
- **Sign-in errors link to the portal (0.25.0).** When the extension cannot find a sign-in, the message links straight to portal.azure.com.
- **Check my access (0.24.0).** A button in Settings shows what your account is allowed to do on the resource groups that hold your pools and hosts: see them, power hosts on and restart them, drain mode, log off users, remove hosts, change pool settings. It only reads, and covers your active roles only.
- **User sessions in the page export (0.24.0).** After Scan sessions, Save HTML and Copy Markdown include the user sessions as filtered and sorted on screen.
- **A fuller demo (0.23.0).** The demo on sample data has 8 pools, Pooled and Personal, 29 hosts, application groups, workspaces and scaling plans.
- **Greyed-out pills (0.22.0).** Filter pills that match no hosts are greyed out.
- **Saved page looks like the Workspace (0.21.0).** Save HTML writes the Dashboard in the Workspace's light look, ready to print. Search and Scan sessions moved to the top row, and the filter pills sit directly above the host table beside its export buttons.
- **Fix (0.20.0).** The Columns, Export and Saved views menus now close when you click elsewhere or press Escape.
- **One table everywhere (0.20.0).** Every table (hosts, pools, scanned user sessions and the Inventory tables) has the same title bar: a filter box and Save HTML, Copy table and Save CSV buttons, with sortable columns. Copy Markdown and Save HTML at the top right save the whole Dashboard.
- **Cards and a pool table (0.18.0 to 0.19.0).** The Dashboard lists host pools in a scrolling table (type, powered on, total, sessions) beside eight cards: Host pools, Active sessions, Capacity used, Idle hosts, Needs attention, Old agent, Drain mode and Powered off. Click a pool to see only its hosts.
- **Console tab (0.16.0).** Shows errors and events from the extension, to help when something goes wrong. Copy or save it when reporting a problem.
- **Fix (0.15.0).** The Inventory tab no longer fails as a whole when Azure refuses one read, and it shows Azure's reason.
- **Fix (0.14.0).** Tile text is centred, and switched-off hosts are no longer shown in red.
- **Fixes (0.13.0).** Host pools now show, and switched-off hosts are no longer flagged as problems. A new Issue column says what is wrong with a host.
- **Toolbar badge and idle cost (0.11.0).** The toolbar icon can show how many hosts need attention, and the Idle hosts card can show a rough daily cost.
- **Inventory tab (0.10.0).** Shows each pool's image and VM size mix, scaling plans, application groups and workspaces.
- **Columns, saved views and exports (0.9.0).** Choose your columns, save named views, and copy or save the table.
- **Scan sessions (0.8.0).** Finds disconnected users. Also bookmarkable views, keyboard shortcuts and a Reset to defaults button.
- **Stale hosts (0.7.0).** Running hosts whose agent has stopped reporting are flagged.
- **Subscription picker (0.5.0).** Focus the Dashboard on one subscription.
- **Idle hosts, old agents and pool capacity (0.4.0).** Spot running hosts with no sessions and out-of-date agents, and see how full each pool is.
- **Host details (0.3.0).** Click a host to see its details and who is signed in.
- **Look and feel (0.2.0).** The same light and dark themes as Intune Enhancer, a theme toggle, a Demo on sample tenant button and a footer.

---

**Sharing & responsibility** - Built for the community, shared with good intentions. Use at your own risk. The author accepts no responsibility for any outcomes resulting from the use of this software. Test in a safe environment first. If you find an issue or have a suggestion, contributions are welcome.
