# 2.4Ghz-Slotted-Waveguide-Antenna

A 2.4 GHz 180 degree slotted waveguide antenna, originally designed for outdoor 802.11b wireless (back in 2001).

I've decided to open source these designs in the hope that someone may find them useful. With the advent of "desktop machining", it should be pretty straightforward for someone to manufacture these antennas at home.

They were manufactured out of 100mm x 50mm x 1000m lengths of extruded aluminium box section. The end-caps were made from aluminium bar.

You'll need the following extra stuff (per antenna):
* 8x M3 x 10mm screws for the end caps
* 4x M3 x 6mm screws for the N-connector
* An N-type panel connector (measure your connector before machining - you might need to change the screw hole position)
* M3 tap to put a thread in the end caps and antenna body
* Silicone caulk to seal the top (leave the bottom unsealed so any water that does get in can drain out).
* Fibreglass tape / kapton tape, another non-metallic tape to place over the slots to keep water & dirt out.
* A U-bolt that will fit. Careful not to overtighten as you can easily bend the soft aluminium. If you need to make it super tight, place a length of steel bar between the pole and the antenna body to stop the aluminium box section from bending.
* A small length of conductive metal rod/tube to be soldered to the N-type connector. You'll need to make sure the stub protrudes into the body of the waveguide by 30.67mm (or as close to this number as you can get it, we used to cut it longer and then file it down).
* The hole above the N-connector is for a tuning screw. The theory is that as you screw in a long screw into this hole, it should adjust the VSWR of the antenna. In reality, this didn't really make any measurable difference. Not sure if I messed up the placement of the hole, however it turned out they didn't really need tuning. We would just screw a 6mm screw in to plug up the hole.

For fittings, stainless steel is recommended as the antenna will likely be outside.

If you want to make an omnidirectional antenna, just machine the slots on both sides.

# History

Back in 2001, when I was young (and my heart was an open book), I was a member of the ["WA FreeNet"](http://members.wafreenet.org/index.php/); a community of IT, radio and communications enthusiasts that set up a metropolitan area network using off-the-shelf 802.11b wifi equipment. This was back when ADSL1 had just been released where we lived, and the vast majority of us only had 56kbps dial-up (so getting a couple of Mbps to a friend's place was a big deal).

One of the members (Chris King) had access to a property in [Kalamunda](http://kalamunda.wa.gov.au), which overlooked the vast majority of the [Perth](https://en.wikipedia.org/wiki/Perth) metropolitan area. This made it an ideal position to place a 180 degree antenna, to enable people from all over the city to place a dish on the roof of their house aiming at this property. This property was known as the "HillsHub".

I used to manufacture and sell these antenna with my best friend Justin Whitten at the time. We sold several hundred of these. We would hire time on a CNC milling machine at a metal work shop, machine them on a CNC. Take them back to Justin's house, manually tap them. Solder up the connectors, assemble. Paint. Test. Package and ship. It was hard work but we thoroughly enjoyed it. Much bourbon was consumed during the making of these.

The following text is from 19 year old me, taken from my (now defunct) website documenting the setup:

_After much research on waveguide antennae, we determined that it should not cost as much as a commercial waveguide to
get one machined. All we needed were the designs. I spent about 3 weeks doing research and drawing up designs in
AutoCAD. After eight revisions, I was finally happy with the design. I sent it off to several engineering companies
for quotations on getting the first prototype machined up._

_After several outrageous quotes (excess of $1000), I was finally put in contact with a company who said they would
machine it up for $250 including materials. After one more design revision, I took the designs over to the company,
and waited for them to machine the first prototype. A couple of weeks later, I went and collected the machined parts.
He had done a good job._

_I took the machined parts home and proceeded to inspect them. The machinist had done a really professional job. All
that was left to do was to clean the swarf out of it, and assemble it. After about 30mins of internal cleaning, the
inside of the waveguide had a mirror finish. The end plates already had a mirror finish from the machining process,
and did not require cleaning._

_To assemble the waveguide, I inserted the two end-plates in each end, and fastened them with their screws. Next, I
made the feeding element on a Dick Smith brand "N-Type" connector, and attached it. The waveguide was ready for
preliminary testing. I had my BR500 set up with a vertical colinear omnidirectional antenna in the room next door, so
I attached a pigtail to the waveguide and plugged it into a Compaq WL110 and proceeded to fire up netstumbler._

_I was disappointed to see that the signal had not changed, and initially I thought that my waveguide wasn't working. Then I rememberd that the waveguide is horizontally polarised, and vertical colinear antenna is vertically polarised. Silly me. So i went into the next room and turned the colinear antenna on its side. When I went back to the waveguide antenna, I could not belive that the signal had jumped up about 20dB! I disconnected the waveguide, gave ChrisK (HH operator) a call, and went for a drive up to the HH._

_We sealed up the waveguide with silicone, and proceeded to climb onto the roof and attach it to the mast. Some spacers were made up out of some old water pipe, placed over the U bolts, and then the nuts were tightened with a "box spanner". Duct tape was placed over the slots to stop dust & dirt ingress. The waveguide was then plugged into the HH access point, and the installation was complete._

_The antenna was taken down again a few days later to be painted and waterproofed, and is now back up, and fully
operational as you read this._

_Since the waveguide antenna worked so well, I decided to start taking orders. I recieved enough orders to get a bulk
batch machined._

_Recently, I was loaned an extremely cool VSWR meter (Anritsu S331B) to test the waveguides with, and I recieved the
first waveguide from the new bulk batch. After tuning the waveguide's tuning screw, and tuning the feed, the
following VSWR reading was obtained. At all points the VSWR is lower than 1.30:1. That is really good. Please see the table below for an explanation of the markers._

| Marker Name | VSWR | Frequency | Channel | Significance |
|-------------|------|-----------|---------|--------------|
| M1          | 1.03:1 | 2412.0 MHz | 1 | Start of 802.11b spectrum |
| M2          | 1.27:1 | 2484.1 MHz | 14 | End of 802.11b spectrum |
| M3          | 1.21:1 | 2445.0 MHz | -  | Taken as common "mid" spectrum |
| M4          | 1.02:1 | 2408.9 MHz | -  | Lowest VSWR at this point |

_For those that don't know what VSWR is, **voltage standing wave ratio (VSWR): In a transmission line, the ratio of maximum to minimum voltage in a standing wave pattern. Note: The VSWR is a measure of impedance mismatch between the transmission line and its load. The higher the VSWR, the greater the mismatch. The minimum VSWR, i.e., that which corresponds to a perfect impedance match, is 1:1.**_

_A friend and I recently went up to [Reabold Hill](https://www.bgpa.wa.gov.au/bold-park/area/reabold-hill) for some antenna testing. The GPS said that we were 25.5km from HH. As soon as we plugged the waveguide in, it picked up the HH, and the signal did not change much as we rotated it around its entire azimuth. Waveguide to waveguide with a distance of 25.5km._

_Another member of the network connected to the HH in Duncraig (29.9km away) with trees in the way. See the HH guestbook for a log of all sucessful connections. You must be logged into the HH to add an entry._
