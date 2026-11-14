# Privacy policy: AVD Enhancer

_Last updated: 14 November 2026_

## The short version

**No data is sent to the developer, or anywhere other than Microsoft Azure.** AVD Enhancer only
talks to Azure Resource Manager (management.azure.com, which includes Azure Resource Graph), the same
service the Azure portal itself uses. The developer runs no server for this extension and receives
nothing from it. It is read-only: it never changes anything in your tenant.

## What the extension accesses

After you accept the disclosure on the extension's Settings page (it opens when you install):

- **Sign-in token.** It reads the Azure Resource Manager access token that the Azure portal
  (portal.azure.com) already holds for your sign-in, so it can make requests as you. It does not read
  refresh tokens, ID tokens or passwords, and it never asks for your password. From the token it
  shows your sign-in name and tenant on the page. Right after an install or update the extension runs its own pickup
  script once in Azure portal tabs that are already open, so the sign-in is found without reloading the tab.
- **Azure Virtual Desktop information from Azure Resource Graph and Azure Resource Manager.** Host
  pools (name, type, load balancer, maximum sessions, resource group, subscription), session hosts
  (name, AVD status and any issue, agent version, last heartbeat, operating system build, drain mode,
  assigned user), the virtual machines behind them (power state, size, region, Azure tags),
  scaling plans and their schedules, application groups, workspaces, Azure maintenance configurations and
  which machines they are assigned to, and the names of your subscriptions.
- **User sessions.** When you open a host or press Scan sessions: the names or user principal names
  of the users on that host, their session state and when the session started.
- **Your own permissions and roles.** Only when you press Check my access or open the PIM roles tab:
  what your account is allowed to do on the resource groups that hold your pools and hosts, and the
  Azure resource roles your account holds or can activate through Privileged Identity Management.
  Nothing is activated or changed from the extension.
- **Background check (optional, off by default).** If you turn it on in Settings, the extension reads the
  host list at the interval you choose and shows the number of hosts that need attention on the toolbar
  icon. It uses the sign-in the Azure portal last supplied and does nothing without one.

## Where it goes

Only to Azure Resource Manager (management.azure.com), over HTTPS, to read the information above.
Every request passes a check in the code that refuses any other address. Nothing is sent to the
developer, to analytics, advertising or tracking services, or to any other third party. There is no
licensing check and no error reporting. The "Try Intune Enhancer" link in the sidebar is an ordinary
link you click to open a store page in a new tab; the extension makes no request to it.

## What is stored, and where

- **Settings:** the display choices you make: auto-refresh and background-check intervals, the subscription you pick,
  the host table columns and saved views, the custom Dashboard cards, the sidebar stars, and the idle cost
  rate (extension storage), and the workspace's light or dark theme (the workspace page's own storage).
  "Reset to defaults" in Settings removes them; removing the extension deletes them.
- **Consent:** your Agree choice (extension storage).
- **Toolbar badge:** the number of hosts that needed attention at the last read, and when (extension storage).
- **Sign-in tokens:** kept in memory and in the browser's session storage, which is memory only and
  cleared when the browser closes. Never written to disk by the extension.
- **Console log:** a short list (the newest 200 lines) of the extension's own messages: reads Azure refused or
  that failed, sign-in pickup and page errors. Kept in the browser's session storage, which is memory only and
  cleared when the browser closes. Sign-in tokens are removed from it. A line can include the text of an Azure
  error message, which may name a resource. It is never sent anywhere. The Console tab's Clear button empties it.
- **Not stored:** the pools, hosts, user sessions, inventory, tags and roles exist only while the workspace tab
  shows them, and in any file or clipboard copy you choose to make (Save HTML, Save CSV, Copy table).

## Changes to your tenant

None. The extension is read-only: apart from Azure Resource Graph, which is a read-only query sent as a POST,
it only makes GET requests, and the code refuses anything else.

## Children

The extension is a tool for IT administrators and is not directed at children.

## Changes to this policy

If a future version changes what is accessed or where it goes, this policy will be updated
before that version is published.

## Contact

systmworks@outlook.com
