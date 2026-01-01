# Considering Pi-Hole vs. Using Safer Browsing

[Pi-Hole](https://pi-hole.net/) is an interesting approach to increasing privacy and reducing ads
for the devices in your network. It could be used instead of or in addition to the approaches
laid out in the [Safer Browsing](./safer-browsing-2026.md) article.

**My overall recommendation** is to use the Safer Browsing approach because it provides a smoother and
more secure experience in terms of blocking trackers as well as ads, both at home and on the go, with
less worrisome configuration that might require being a power-user who knows about networking.
However, it does not help non-browser cases like [phone apps](./browsers-vs-apps.md). More details below.

## Pi-Hole Experience

I previously installed Pi-Hole in my network in 2023 but only configured its IP address as the DNS for
a couple of my machines including a phone and a computer to check out the experience before making the
decision whether to expand Pi-Hole to my whole network. I didn't use the [Pi-Hole + VPN](https://docs.pi-hole.net/guides/vpn/openvpn/)
approach for blocking when not on my home network, as I use a commercial VPN for my devices (see
[discussion](./safer-browsing-2026.md#vpns) in Safer Browsing article).

I ran it in conjunction with all of the browser [add-ons](./safer-browsing-2026.md#browser-extensionsplugins)
add-ons noted in the Safer Browsing article, as well as with those extensions turned off in Brave's settings.
I only used it with a couple of phone apps from my phone (a browser and an airline app) which does not give
me a strong sense of results there.

### Pros

* Less need to configure [Safer Browsing](./safer-browsing-2026.md) on each of the devices in your network,
  since Pi-Hole blocks access to ad networks. However, it was unclear whether it was also blocking trackers.
* Can block ad accesses for phone apps that, as noted in [Browsers vs. Apps](./browsers-vs-apps.md), contain
  their own internet access code that is different from but often similar to browsers and do not allow
  plug-ins or extensions like Brave does. Note however that the app may respond oddly to the inability to
  contact internet domains that it expects to be able to reach but that are blocked by Pi-Hole.

### Cons

* Pi-Hole requires some networking know-how. The installation instructions are straightforward
  but debugging problems or uninstalling it can run into trouble that require power-user capabilities.
* Pi-Hole is only on your network, not available during travel without exposing your home
  router's VPN endpoint to drive your phone's network traffic throgh your Pi-Hole. Enabling
  that VPN endpoint and debugging problems are even more of a power-user problem than just plain
  installing the Pi-Hole.
* Produces some odd web page rendering results including error messages about broken network domains.
  [Safer Browsing](./safer-browsing-2026.md) approaches produce fewer such oddities as the blocking
  is done from within the browser. When I was using it this would appear as black boxes instead of
  ads, or empty spaces with error messages like `Unable to contact foo.com`.
* Doesn't block some types of ads that in-browser plugins can block, such as those sent from the
  web site itself.
* May not block Facebook and other trackers that are used to track your browsing across the internet,
  since those trackers may come from facebook.com or other allowed network domains. Safe Browsing
  plugins, including Brave's default Shields feature, do this with more ease since they can see the
  web page contents and see and remove links to those trackers.
* As noted above, may break some apps that are not expecting to fail to contact ad servers.

