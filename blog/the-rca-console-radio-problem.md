# The RCA Console Radio Problem, or How Arbitrary Change Breaks People

Think back to historical radio consoles like the RCA wooden furniture model that a family
might sit around for evening radio shows 80 years ago. There were a few dials and buttons,
a bare few readouts, otherwise it was wood wrapping warm tubes and speakers. Everyone in
the family from children to elders soon knew how to turn it on, tune channels, and change
volume. The dials never moved around, the readouts stayed in place and did not suddenly
read out some other information or change fonts, and people could operate it in the dark
if they needed to since their muscle memory could get used to the location and feel
of every control.

<img src="https://upload.wikimedia.org/wikipedia/commons/1/1a/RCA_Model_RC-350-A_%281938%29.jpg">

Same goes for any of many such devices people grew up with up until about the 1980s.
TVs whose channel knobs, volume controls, and even rabbit-ear antennas, familiar from years
of use and muscle memory. Stoves, record players, tape players, CD players, car dashboards,
boomboxes. Even the idea of channels of radio, TV, and cable were a long familiar concept,
easy to understand as the number of channels went from 3 to 300 and the problem became
avoiding commercials by changing channels.

Enter the PC era. Screens first consisting of character grids into which apps could write
their character-mode user interfaces. Competitors would clone the look and feel of each
other's apps, from hotkeys to placement of text fields and controls on the screen, to make
it easier for one app vendor to steal business from competitors by letting people's
"muscle" memory of screen positions and hotkey sequences and app behavior apply while moving
from, say, Lotus 1-2-3 to Excel. Heck, they even sued each other sometimes when look-and-feel
was too similar (the lawsuits generally failed, however). In a way, this was a
deliberate hacking of the RCA radio console pattern back when people were still expecting
consistent behavior and placement of screen controls from their apps in order to minimize
cognitive load and let them concentrate on the actual work at hand.

Then came the GUI, and apps changed their layout, first to take advantage of windowing
systems while placing controls in a similar-but-different configuration on the screen
vs. how it was done in character mode. Those layouts and reimplementation of hotkeys
and other behaviors helped ease the transition from text mode to GUI apps. And Windows
and MacOS took off.

Soon came browsers and the Internet, with page layouts and fonts and hooked hotkeys and button
actions suddenly changeable by saving a new .html file on the server. Fixed formats were out,
experimentation with layouts and frameworks was in, and it took a dozen years just to get to
"grid" style frameworks that could give some guarantee of consistent layouts as long as the
browser window was a similar size and aspect ratio as on another device. More flowable
frameworks followed that made it easier to handle aspect changes and small screens while
maintaining some sort of consistent grid to hang things on.

Yet all this easy changeability ran counter to the experience of generations who grew up with
the concept of muscle memory and other patterns to reduce cognitive load by reusing layouts
and behaviors. Continuing the analogy, the RCA console could, from hour to hour, move its
buttons and dials and readouts and speakers into new locations, add new buttons, remove others,
and change behaviors, at the whim of RCA. Everyone using it would have to pause and relearn the
locations of things and how things functioned up to several times per day. Muscle memory confounded,
cognitive load increased. Would people have bought such a thing back in those days? They might
go to a friend's house and their RCA would act completely differently, so listening to the radio
there was another re-learning. More time wasted, more cognitive load.

You can still occasionally find places, maybe the auto parts store or the library,
where there is still a character-mode interface, or what looks like one but embedded
in a GUI window. The people using those interfaces don't have to think about how to
enter the details of your special order, they type and hit Tab and Enter as fast as
you speak the details without looking at it until the end to verify things.
It's wonderful to see such things, they don't waste their or your time using a mouse
or glancing down to make sure the text controls have not moved since yesterday.

What's the point, you ask? I keep encountering the RCA console problem while helping older people out
with their tech problems. I get panicky help requests for how "email is broken" when it was a case
of a link being moved to a different part of a web page with a new font and color, and the person
used to clicking a certain spot on the screen for a couple of years suddenly was clicking into
some other unexpected page.

I got a lot of complaints when, after people got used to the way Windows 95's desktop and apps behaved,
Windows 98 changed icon shapes and colors and moved things around so that people had to stop and relearn.
Forget Windows 8's complete change of everything everyone knew, since the Metro tile interface
was "so easy" and "everyone would understand it intuitively" when instead it caused massive
support problems for Microsoft and a lesson to the industry. And it wasn't just from older users,
nearly everyone hated that sudden, needless change, so much so that Windows 10 had to put back
most of Windows 7's interface to appease the anger.

OS layouts, web pages... apps! Since many apps are just web pages compiled down into an app wrapper,
it's just as easy to ship layout and font and behavior changes as it is to save new HTML and CSS
files for a browser-based page.

I see it often: The new app update that confounds its users by moving controls around and changing
inter-page flows. The new web page that is missing half the things people would just know how to do
on the old page, now hidden in sub-pages and menus and requiring cognitive load and, in many cases,
retraining in the form of in-person classes or videos to tell people how to do things the New Way.
The new OS update that arbitrarily shuffles default icons and features around to make things
"easier" but in fact making things far more difficult.

And wasting more time and adding cognitive load, unnecessarily.

Heck, there was even some old *Star Trek: The Next Generation* episode that added to the problem
in its own small way, some tech on the bridge was using idle moments to "optimize button layouts"
for "efficiency" but what it really was doing was making someone in the midst of a battle or
emergency have to stop and look around for where the Fire Torpedo button was that used to be
in the bottom right of the Tactical console, but Bridge Dweeb #117 changed it for no
real reason than because he could.

I don't know how to fix this. New web frameworks seem to appear every year, every UX dev
is trained on a subset of frameworks, so you almost have to upgrade the whole site to a completely
new system each time more than trivial changes are needed, and the new designers don't understand
the important behaviors and layouts in the old system, they just proceed as though a wholly new
system is how things ought to be. But for users - more for the older cohort, but also for the young -
the changes just create overhead that would be better spent on real things, real results,
real work, real play.

I've heard a constant drumbeat - the only really constant thing - from various companies that
we need to "embrace constant change" as it's "good for us." But it's not, not at all.

As for elders trying to use their computers or phones or tablets to pay their bills or
read messages from their families? The incessant change can break them, make them give up,
as relearning the equivalents of dials and switches and readouts and behavior every few months
or couple of years becomes too much to take.

So maybe this is a plea to UX designers: Consider incremental updates, not top-down redesigns.
Consider porting behaviors and layouts from one framework to another instead of starting anew.
It might not give you that satisfaction of changing everything to your New Way, it might
make the upgrade less sexy and splashy to sell to management, but have a heart for your users...

Young and old.

And no, that icon doesn't need a change to Cornflower Blue. Just leave it alone.
