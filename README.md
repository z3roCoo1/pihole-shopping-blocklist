# pihole-shopping-blocklist

A plain domain list of retail/e-commerce sites, for optional blocking in [Pi-hole](https://pi-hole.net).

## Usage

Subscribe to the raw list as an adlist:

```
https://raw.githubusercontent.com/z3roCoo1/pihole-shopping-blocklist/main/shopping-sites.txt
```

In Pi-hole: **Group Management → Adlists → Add**, paste the URL above.

To make it toggleable independently of your other blocklists:

1. **Group Management → Groups** — create a group (e.g. `Shopping`).
2. Edit the adlist you just added and assign it to that group only (uncheck `Default`).
3. Flip the `Shopping` group on/off whenever you want the list enforced or not, without touching your other adlists.

Run **Tools → Update Gravity** after subscribing, and again any time the list changes upstream.
