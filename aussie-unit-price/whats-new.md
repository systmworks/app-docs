# Aussie Unit Price: what's new

New features and fixes, newest first. Versions released on the same day are grouped. Versions
before 3.0.0 were test builds, not public releases.
Aussie Unit Price only reads product names and prices on the shop pages you visit. It never
collects or sends anything.

## 3.0.0 - 26 October 2026
First public release on the Chrome Web Store.
- **Price per item on every product.** A badge under each price shows the price per can, bottle,
  tablet, screw, battery or item, plus the price per litre or per kilo when the size is in the
  product name. Amounts under a dollar show in cents, like "5.6c/tablet". Single items show their
  full price.
- **One line per option.** Where a product has several (single, pack, case, or a deal like "2 for
  $130", "Buy 6 Get 4 Free" or "Buy 5 Pay 3"), each gets its own line, with the cheapest per item in
  bold. Member-only prices are marked **M**.
- **Best value highlighted.** Dark green is the top 10%, light green the top third, with a rank
  such as "#3 of 40 by $/L on page". Products are ranked against others priced the same way (per
  litre, per kilo or per item), so like is compared with like.
- **A toolbar you can move.** Sort the page by best value, price per item or lowest price; turn
  member prices on or off (Dan Murphy's); and load every product first so the sort covers the
  whole list. Drag it by its green header, double-click the header to put it back, and use the "-"
  button to collapse it. It remembers where you left it and stays on screen if the window shrinks.
- **Works on:** Amazon.com.au, Bunnings, Officeworks, Chemist Warehouse, Dan Murphy's, BWS and
  Liquorland. "Load all" works on Dan Murphy's and BWS; Liquorland switches to 80 per page; the
  other stores are paged, so the sort covers the current page.
- Renamed from "Fair Dinkum Unit Price" before release, so no one saw the old name.

## 2.4.0 to 2.9.0 - 25 October 2026
- **Drag the toolbar.** Move it anywhere by its header and it remembers the spot. Double-click the
  header to put it back in the corner.
- **More deals worked out.** "Buy 6 Get 4 Free" and "Buy 5 Pay 3" now get their own line, priced per
  item.
- The toolbar header shows the full name, so it's clearly not part of the shop's page.
- Fixed: "Pepsi Max 375ml x 30" read as 1 can instead of 30.
- Fixed: a size followed by "x" and a number, like "375ml x 24", lost its price per litre.
- Fixed: clicking the toolbar header without dragging stopped the toolbar following the bottom-right
  corner.
- Fixed: the toolbar could end up off screen after the window was made narrower. It now comes back
  on screen, and returns to its spot when there's room.
- Fixed: an interrupted drag could leave the toolbar stuck to the cursor.

## 1.1.0 to 2.3.0 - 24 October 2026
- **Seven stores.** Now works on Dan Murphy's, BWS, Liquorland, Amazon.com.au, Chemist Warehouse,
  Bunnings and Officeworks, and renamed from "Dan's Unit Price" to suit.
- **More than drinks.** Prices per litre or per kilo, and pack counts for tablets, batteries and
  similar items.
- **Loading progress.** "Load all" shows "Loading 130 of 206..." and updates every 2.5 seconds.
- Amounts under a dollar show in cents.
- Single items show their full price as their unit price.
- Fixed: "TCL TAB 11 FE Tablet", a computer, read as 11 tablets.
- Fixed: "Galaxy Tab A9+ 5G" read as 5 grams, which came to $19,800/kg.
- Fixed: "1698 Strong Ale Bottles" read as 1,698 bottles.
- Fixed: "Hahn Super Dry 3.5 Block Can 375mL Pack (30)" read as 5 cans instead of 30.
- Fixed: "24 pack of 250ml Cans" read as 250 cans instead of 24.
- Fixed: "Wagner Vitamin C 1000 Chewable 250 Tablets" read as 1000 tablets instead of 250, and
  similar badges said "/chewable" instead of "/tablet".
- Fixed: Dan Murphy's "$6.99 Each" next to a 12-bottle case was priced as if it were 12 bottles.
- Fixed: Dan Murphy's wines with no size in the name had no price per litre.
- Fixed: BWS prices could read as "$750" instead of $7.50.
- Fixed: Liquorland could read the old "was" price instead of the current one.
- Fixed: Liquorland's load button said "All 80 loaded" when the shop had more. It now says "Max 80
  of 918 loaded".
- Fixed: shop banners with ticking countdowns made the extension re-check every product about once
  a second. It now only re-checks when the product list changes.
- Fixed: "Load all" could stay stuck on "Stop loading" after an error.
- Fixed: saving a setting could fail if the extension had been reloaded with a shop tab open.

## 1.0.0 - 22 October 2026
First version, for Dan Murphy's only.
- **Price per can and per litre** on every product.
- **Sort toolbar** with "Load all", to sort the whole list rather than just what's showing.
- Fixed: the badge sat underneath Dan Murphy's Add to Cart button.
- Fixed: "Load all" couldn't find the "Show 24 more" button.
