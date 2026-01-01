# Safer Browsing Recommendations - 2026

Privacy and security are pretty difficult to come by these days. There are a lot of existing pages
recommending various operating systems that are more or less secure or app compatible. There are
also recommendations on this or that browser. This is my recommended browsing configuration and
approach to try to preserve some semblance of privacy. No guarantees here, just what I do or
have recommended others to do.

Also see [Browsers vs. Apps](./browsers-vs-apps.md) since using phone and tablet/iPad apps
have their own problems that can be solved by using browsers consistently.

## Operating Systems

No commerical operating system vendor is trustworthy, as they are subject to governments and
supra-government entities telling them what they must do. The open source ecosystem is vulnerable to
attack by code submissions that break privacy and security, no matter how heroic the efforts to
prevent this among the open source code owners. That said, you have to trust something in the end.

### Windows

I have clients who must use Windows for various reasons. Windows 10 has been deprecated in 2025,
with limited patch support into 2026. Which means you're now subject to the latest permissive Windows
EULA in Windows 11. Good luck. It comes installed with OneDrive and Microsoft Azure cloud links,
which is horrible for privacy as it means all your data is uploaded to some unknown set of servers
where your documents can be analyzed or read by unknown people and AIs inside and outside Microsoft.
(Plus the OneDrive integration into Windows is pretty confusing for users and support personnel,
such as figuring out which Documents or Pictures or Downloads folder someone put something into.)
Personally I don't trust Windows for privacy. And "AI" integration in the hardware and OS with
screenshotting to analyze what you're looking at sounds to me like the NSA's dreams made reality.

Plus the legacy 1980s/90s style of OS that Windows is means it's relatively easy for attackers to
compromise security from within applications or app installers. Microsoft has done some great work
locking down the kernel from attack, and has closed numerous attack vectors and diligently issues
a lot of patches, but there is a lot of code in Windows, meaning a lot of places and ways to attack.
See the size of each Patch Tuesday.

That said, changing to other alternatives is expensive in your local fiat currency (Mac/iPad),
time spent troubleshooting and working around odd configuration problems (Linux), or time for
retraining (all other OSes). Especially difficult for large organizations to do, non-technical
people who have grown used to Windows, or people who don't handle jarring change easily.

### Mac

I don't trust Apple either. They make noises that sound like privacy and security, but they are subject
to the same influence from governments and supra-government entities behind the scenes.
The OS is an 80s/90s design like Windows and Linux, rather permissive in what installers
can do and what apps can affect, though it's a bit more locked-down than Windows by default.
"AI" integration in hardware and software adds even more uncertainty. MacOS at least is rather
usable, and Apple Store support is oddly really good sometimes, so maybe this is a good middle
ground that might work for you if you need a desktop computer experience. Expensive though.

### Linux

I use Linux Mint as one of my work platforms. That said, even as a technical user I've had trouble getting
Mint (and its Ubuntu and Debian underpinnings) to work properly without a lot of internet searches and
hours spent in configuration files. This makes it difficult to recommend to non-technical users. The
confusion of various distros and lineages and package managers makes recommending Linux even more
difficult for non-technical people.

Like Windows and MacOS, Linux is an 80s/90s OS design, lots of code surface area for an installer to attack.
Like Mac it's more locked-down by default than Windows.

But it's also not Windows and not Mac. Which is why I prefer it when I can use it and I need
a desktop computer experience.

### iOS (iPad/iPhone)

I have recommended iPads for people who have no need for a full desktop experience because it's far
more secure of an OS design. See my notes on Apple above, but this OS is at least a 2000s design
hence apps are contained in better "bubbles" that prevent them from destroying or attacking other
apps or the operating system itself quite so easily. It lacks USB ports for moving data around
locally, making it an internet-only device with iCloud connection (yuck!). "AI" integration in
hardware and software also a minus.

Still, it's pretty good if your main use is internet browsing or cloud stuff. A Bluetooth keyboard
and a stand to hold the iPad upright can make it Good Enough for many purposes.

### Android (tablets or phones)

Fair overall. Google put a lot of work into making Linux usable in the way an iPad is.
The OS still lacks the stronger "bubbles" that constrain iPad/iPhone apps, but it's not as bad
as the desktop OSes. I don't trust Google at all just as I don't Apple or Microsoft, so
expect bad EULA terms for privacy and a lack of privacy especially on the phone for location
tracking in real-time. Also varying levels of "AI" integration that throw privacy into doubt.

That said, for budget-constrained people who don't need a full desktop, an Android tablet
can be an OK choice. Like an iPad, adding a Bluetooth keyboard and a stand make things nicer.
And many tablets have USB and MicroSD ports to be able to copy data in and out without using a cloud
provider that would get access to your data.

### Other OSes

QubesOS, BSD variants, and so on are not realistic for regular users to use.
Qubes is a great idea but is behind on hardware support and might be on its last legs.

Using a primary OS like Linux with a Windows or Linux virtual machine that is used
just for browsing is an interesting idea if you're a power user to keep browser attacks
from infecting the rest of your primary OS.

## Browser Choices

No browser vendor is truly trustworthy. You are stuck playing within the limited
set of browser choices, and having to make choices within those browsers' plugin and extension ecosystems.
A browser vendor could easily integrate code that sends what sites you connect to and any other
desired browsing information to a cloud to add to your profile. You have to trust that they are
not doing this.

My winner for several years is [Brave](https://brave.com/). I hope - but cannot prove - that Brave's developers
and company don't slide in a bunch of spyware underneath, or that they don't take in
compromised browser internals through changes to the upstream Chromium codebase they rely on.
Using Chromium at least gives it use of a bunch of useful privacy extensions (see below).

My general rules for choosing a browser:

* Google, Microsoft, and Apple are not trustworthy IMO. I avoid Chrome, Edge, and Safari except where
  I have to use them.
* I used Firefox for many years until the Firefox CEO jumped in on the censorious "Trusted News"
  bandwagon that has caused so many problems for over a decade.
* Opera seems like it's barely holding on, at least last time I looked at it.
* Brave was my choice once Firefox became dodgy. The right claims of privacy etc., even if not actually
  true in reality. Plus it does not have the same intra-browser censoring of some DNS domains that
  other browsers have for some of the more interesting sites on the internet. And its built-in
  Shields help shut down web site trackers like those from Facebook.

## Browser Extensions/Plugins

I've used and discarded many privacy-related extensions over the years as they appeared, grew,
then in some cases were closed down or the authors sold out to ad corporations that wanted to
help drive their ad streams into your browsing.

I'm shaping this discussion in terms of Brave but the same plugins are available for the rest of the
Chromium browsers (Chrome, Edge) and probably for Safari, Firefox, and Opera.

| Extension | Notes |
| --------- | ----- |
| Brave browser's built-in Shields | This replaces some extensions I used to have installed. Not a panacea but pretty good first line of defense. Another reason to use Brave. |
| Privacy Badger | I've used various Electronic Frontier Foundation extensions over the years, and this one remains one of the first I install to avoid Facebook and other trackers from reporting my browing habits to various megacorporations. [Donate to the EFF](https://supporters.eff.org/donate/donate). |
| uBlock Origin | Faster version of the old uBlock extension, great on phone OSes and batteries. Cuts down ads. |
| Ghostery | I turn on `Ad-Blocking`, `Anti-Tracking`, `Never-Consent`, and `Search Engine Redirect Protection` in its settings to get the maximum effect. [Donate to Ghostery](https://www.ghostery.com/become-a-contributor). |

For each of these extensions I enable `Use in Private` since I use private browsing most of the time.

## VPNs

I almost always use a VPN, both on my phone and desktop machines.
At the moment I use ProtonVPN in the hope they are not compromised as is
pretty much everything else these days, plus they have many VPN nodes worldwide
and a pretty nice management app.

A VPN will help avoid people in airports, coffee shops, and your ISP from knowing what
sites you're contacting. It does not provide much additional security for talking to
your bank, email, or other important sites. Your VPN vendor might or might not be storing
your browsing info no matter what their web site says, making VPN an uncertain way to obscure
things.

Using a VPN will often make your bank or other financial institutions block your access,
and some sites will add in CAPTCHAs when using a VPN to reduce attacks coming through the
VPN. You might have to occasionally drop your VPN to contact some sites, then remember to
turn it back on afterward.

On your phone it might allow to you to prevent all contact to the internet except through the VPN.
This is useful to avoid your phone OS from "phoning home" using your unmasked address before
the VPN software starts up while booting up your phone. On the other hand, if you need to drop your
VPN sometimes, you have to at least temporarily disable this setting.

## Browser-Based Syncing

Pretty much every browser allows you to log into it to share your favorite site links, browsing
information, and even WiFi network names and passwords to share across other computers and phones
more easily. I used to use this to make life easier, but stopped about 10 years ago when I realized
how nefarious this can be: You are letting your browser's vendor see a great deal about you and your
preferences by letting this information be uploaded to their cloud. The login itself, which is tied
to an email address, then becomes part of the "profile" of that email address, which in older days
was better called a dossier. This is very valuable tracking and personal information unless your entire
browsing life is spent on MSNBC/MSNOW.

I now use two methods to avoid syncing:

* On my phone, I program in my favorite links one by one into the browser when I install the phone.
  Takes an hour but worth it.
* On my desktops I keep my personal favorite links in a file like `links.html` in which I manually
  place my links using a text editor like Notepad. See the section below for an example file you
  can use to create your own. I copy this file from machine to machine and open it in my browser,
  then `Ctrl+Click` to open each link in a tab. Combined with private browsing (see below) this means
  a fresh set of cookies when I restart my browser or reboot, which denies information to the web sites
  you use.

## Private and Non-Private Browsing

Whenever I reboot my computer or close my browser, I start Brave to get a non-private window, then
click the menu at top right and click `New private window` to get an additional private window.
I segregate my browsing by purpose and use:

* The non-private browser window I use for sites where I want it to remember me. Typically this is for
  sites I log into like email, bank sites, and some social media, so that my cookies last and logging
  in is easier. All of my tabs usually reload when I open Brave so I'm right back where I left off.
* The private window I use for most of my links for regular browsing. This includes blogs but also some
  social media where I don't mind logging in after each reboot, and sometimes my bank when I want to
  make sure I'm not reusing previous cookies and don't mind extra login steps.

See the notes above on `links.html` - I typically open that file in the private browser to get a view
of my favorites, so that when I click them or `Ctrl+Click` I am opening them as a new tab in my private
browser window.

### Why use private browsing?

This gets a bit complex. I use private browsing to break away from any cookie-based tracking a web
site is doing to me. Almost every site on the internet sends a tracking cookie back to your browser
that lets it know where you have been on the site. If you log into the web site, a "token" is kept
in the cookie that represents your login. If you open a site in a non-private browser window,
whatever cookie you previously had on your machine is reused. This is usually fine for email and
banks. But for general internet browsing, that cookie represents a profile - a dossier - on your usage.
If you log in to a site, that information is added to its database of your overall activities on the site.
If you don't log into a site, it represents an "unknown" profile that is not taggable to a specific
person, but is tagged to the address of your computer on the internet and other information.

Pretty much every company sells profile/dossier data like this to middlemen to assemble
profiles that span what you do across the whole internet. It's especially easy to do this when
the profile data is taggable to an email address or other identity - the dossier on you grows and
grows, including links to who you talk and text and chat and message with, and they get to
resell this data to advertisers, governments, attackers, AI vendors, pretty much anyone who
has enough money to buy your information. You can't directly prevent or opt out of this,
it's become part of how the internet works over the last 20+ years.

You may have heard that, "If the app or site you're using is free, *you are the product*." This is
the main way it's done. Facebook, Google, Microsoft, smaller sites - everyone sells your information
to fund their server farms and employees and profit. Everything you do is assembled 24 hours a
day into a dossier tagged to your email, which often is linkable directly to your personal
information without much effort, and to your family and friends beyond that.

I'm a contrarian and like breaking the profiles. Let them track a day or several days of browsing,
then start over with a new profile after a reboot. It doesn't work every time, since they could
use other information like your computer address to link profile information, but at least it
throws up a roadblock. In this day and age that's all you can hope for.

Plus when you combine empty cookies and a VPN it's harder to assemble a profile from your computer's
address. A win-win at the cost of paying for a VPN.

The only real alternative I can think of is to go full tech Luddite and get rid of computers,
phones, smart TVs, and everything else that can gather and send information on you. Good luck
with that in the modern age.

### What about Tor browsing?

I have found it very slow. Feel free to give it a try. It's different from a VPN but has a
similar idea of obfuscating your computer's address.

## `links.html` Example

As promised above, here is a quick guide to creating your own `links.html` file to let you
keep a list of favorite links without using a browser's Sync feature that lets them add
your preferences to the profile/dossier they are keeping on you.

One note, the browser Sync feature deduplicates links and synchronizes them across your
computers and phones. This means there is one master copy of the links. When you use
a `links.html` file, you might have copies of it on two machines and it's your job to copy
links across to the copies when you add, remove, or modify them. Additionally, like any
file belonging to your "stuff," you need to back it up.

I store my `links.html` file:

* In my profile root on Linux: `~/links.html`
* In my Documents folder on Windows. Note if you put it into the 2nd Documents folder that
  exists under the OneDrive folder, you're letting Microsoft see your links, which is like
  disclosing them via browser Sync, though you do get automatic backup. Putting it into
  the "original" Documents folder avoids that, but you have to remember to back it up from there.

You can tell your private browser to open that file by pasting its path directly into the
address bar.

Here's a sample `links.html` with some section headings I use to separate out
different categories of links. Some links I visit daily or weekly so keep those in
specific categories, others I keep in specific categories.

```html
<head>
    <title>Links</title>
</head>
<body>
    <p>
        <h2>Dailies</h2>
        <ul>
            <li><a href="https://youtube.com" target="_blank">YouTube</a></li>
        </ul>
    </p>
    <p>
        <h2>Weeklies</h2>
        <ul>
            <li><a href="https://linux.org" target="_blank">Linux</a></li>
            <li><a href="https://brave.com" target="_blank">Brave</a></li>
        </ul>
    </p>
    <p>
        <h2>Tech Blogs</h2>
        <ul>
            <li><a href="https://nodejs.org/en/blog/" target="_blank">Node.js</a></li>
        </ul>
    </p>
</body>
```

Copy the example to your own file, then feel free to modify to add your own links and new or different
section names. You can use any text editor, from Notepad on Windows to the Text Editor on Linux,
or Visual Studio Code etc.

When you save the file, refresh it in your browser to see and use your new links.
