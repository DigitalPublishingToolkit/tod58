---
Pr-id: MoneyLab
P-id: INC Reader
A-id: 10
Type: article
Book-type: anthology
Anthology item: article
Item-id: unique no.
Article-title: title of the article
Article-status: accepted
Author: name(s) of author(s)
Author-email:   corresponding address
Author-bio:  about the author
Abstract:   short description of the article (100 words)
Keywords:   50 keywords for search and indexing
Rights: CC BY-NC 4.0
...

---
---


# 4. The Social Technologies of the Network Commons (Freifunk 2)

![](media/image1.jpeg){width="3.8006944444444444in"
height="4.175in"}Fig. 18. Topology and metrics of a local mesh test
network.

The social technologies of the wireless community network are
technologies specifically developed to support social goals, such as
community networking. Typically, new technologies are developed by large
firms or the state. The achievements of wireless community networks
demonstrate that there is an alternative: community based innovations.
This chapter presents the genealogy of some of the key technologies
needed for wireless community networking and discusses their social
content.

A happy accident in June 2003 opened the gates to wireless cornucopia.
Developers on the Linux Kernel mailing list started making comments
about a product of the company Linksys. In March 2003, Cisco Systems had
bought Linksys for US\$500 million. The firmware of the wireless access
point WRT54G included both the Linux kernel and other code released
under the GNU General Public License (GPL). The company had published
the firmware as binary, but not the source code, which was against the
terms of the GPL. As the developer who revealed the GPL violations quite
happily added, this meant that a whole family of chips by one wireless
provider, Broadcom 802.11b/g, supported Linux. ‘Complaints appeared on
discussion boards such as LKML and Slashdot claiming that Linksys was
violating the GPL by not providing source code for certain code used in
its WRT54G wireless access point.’[^04chapter4_1]

The Free Software Foundation stepped in, leading the campaign for
enforcement of the GPL. Cisco was brought to comply by publishing the
source code. This enabled a revolution, albeit one that most people have
never heard of before: the revolution of firmware flashing.

Based on the source code for the Linksys product, a new initiative
called OpenWRT came into existence and began making an increasingly
stable GNU/Linux distribution specifically for small wireless devices.

The WRT54G became the most popular router for community networks, and
this is where OpenWRT has its name from. Meanwhile, OpenWRT works on
many embedded devices such as WLAN routers but also wireless hard-drives
and basically everything that networks.[^04chapter4_2]

Firmware replacement had been the battle-cry of East London
artist-engineers such as Alexei Blinov and Adam Burns in 2003-4. It was
possible, in principle, even before OpenWRT, but it was very hard. At
the time, early ideas for Hive networks were being flouted around. This
project, which went through many instantiations, initially was quite
Utopian.

It was a boldfaced claim that you could make multi-hop networks using
mesh network protocols that use every available snippet of network
connectivity, be it Bluetooth, Wireless, LAN or you have it;
furthermore, those devices should also be self-announcing, if they carry
any services. Taking inspiration from the Zeroconf protocol, the meshing
devices would tell if they offer services such as streams, voice chat,
podcasts, skype, jabber, and others.

With OpenWRT, this utopia came that bit closer, but as this interview
with Sven Ola-Tücke[^04chapter4_3] also attests to, it needed great skill and
tenacity, even with OpenWRT. You needed to create a directory on a Linux
machine for compiling the firmware. To compile one Linux kernel on a
machine for another machine is very difficult, especially if the other
machine is so different. *Cross-compilation toolchain* it was called by
my London friends Alexei and Adam. Once you had built a customized Linux
image for your device, you needed to transfer it to the device and
*flash* it, replace its existing firmware with the new one.

If anything went wrong, you had not flashed it but *bricked* it. The
device’s electronics were as dead as a brick. As Alexei Blinov pointed
out, that is quite unfair against bricks because they can actually be
still useful. A dead WRT54G is really only electronic toxic trash. Once
you have successfully replaced the firmware, you still need to configure
it, all via ssh and shell. Last not least, you had to make the OLSR work
with the firewall. If then everything worked well, you could indeed mesh
using cheap, nearly ubiquitous devices in autumn 2004. The liberation of
hardware to build the network commons through OpenWRT was undoubtedly a
great step, hence now software experimentation could begin.

Another important step was the release of OLSR 0.48. In this
announcement by Elektra,[^04chapter4_4] the advances of this protocol are
explained. The Open Link State Routing protocol was developed initially
as a master thesis by Andreas Tønnesen at UniK – University Graduate
Centre. In the context of Wizards of OS he was invited to give a
presentation at c-base. The conference series Wizards of Operating
Systems was initiated by Volker Grassmuck and ran from 1999 to 2006. In
2004 we made a panel on free networks[^04chapter4_5] and a workshop.[^04chapter4_6] The latter
was organized by the community, that is largely by Elektra and Sven
Wagner. At the main conference Dewayne Hendricks talked about a 2
Gigabit network for California, constantly referring to the
*holodeck*.[^04chapter4_7]

The workshop was dedicated to mesh networking and was to have lasting
repercussions. The Freifunk community started using OLSR, which gave
decisive impulses for its further development. As Elektra writes, as
soon as communities started using mesh networks, the technology started
to flourish. The community networks have the decisive advantage of
having real test conditions. This underpins also project Confine which
has developed a community testbed. Many problems of routing stem from
the wireless medium, which is unpredictable.

At WOS3 a number of MeshCubes from 4G systems were used to create the
network at the conference venue. It was running OLSR and the quality of
service was horrible, according to an online posting.[^04chapter4_8] But within the
space of a few months the metrics used were significantly improved. OLSR
started to use routes according to the actual quality of transmission,
the so called ETX metrics (Expected Transmission Count).

This was the start of a long story of community development of mesh
networking. Who wants to get more into the technology should read *Mesh
– Drahtlose Ad-hoc Netze* by Corinna *Elektra* Aichele.[^04chapter4_9] According to
her, the release of OLSR 0.48 in December 2004 was a major step in mesh
routing. We could say that mesh routing is the paradigmatic technology,
the one which is most expressive of this dispositif, because it brings
together technological and social goals and advantages. It expresses the
ideal that everyone could connect to everyone in a decentralized way.

I will return to the topic of mesh routing but stick to the timeline.
Some of the *technologies* which communities have developed are rather
more like techniques, social technologies in a more direct sense, ways
of doing things. At around 2004-5, Cornelius Keller put the website
OLSR-Experiment online.[^04chapter4_10] This was a website which according to a
logic following Berlin’s postcodes, handed out IP addresses for people
who wanted their wireless router to be part of Freifunk. The visual
logic of this method you can follow here:

![](media/image2.jpeg){width="5.651388888888889in"
height="3.4875in"}Fig. 19. Berlin map by postal codes.

As another snapshot shows, in a series of core meetings, the Berlin
community decided how to use the IP addresses for a Class B Net.[^04chapter4_11]

Last not least, in autumn 2004 Sven-Ola Tücke had started developing
Freifunk Firmware. Initially it was developed for the Berlin Backbone,
but then became the foundation for the whole Freifunk community. The
Freifunk Firmware (FFW) brought together OpenWRT and all software
components you needed to run a Freifunk node, in an easy to use,
web-based installation process.

This is how it works more or less still today. You can buy a device from
a recommended list of compatible devices. Then you go to the Freifunk
webpage and request an IP address. Then you get the automatically
compiled correct installation package for your device. You install the
firmware via the web-interface, enter the IP address and here you go.

In 2005, OpenWRT released the so called White Russian version, which was
the first stable release. The Freifunk Firmware still relies on a
follow-up version of that.

There is no doubt that the Freifunk firmware contributed massively to
the take off of Freifunk in Germany and Funkfeuer in Austria, who made a
customized version, based on the same foundations. As Jürgen Neumann
said in an interview, when he saw Sven-Ola’s Freifunk Firmware for the
first time, he knew that Freifunk was becoming a reality.

The coming together of this assemblage of artifacts – the liberation of
hardware to build the network commons, mesh routing and the Freifunk
Firmware – stimulated a rapid growth of free networks. Other regional
flavors of firmwares were made for Funkfeuer, Guifi, Wireless London. In
the mid-2000s, Freifunk communities mushroomed, many also in former GDR
territory. The availability of small and cheap hardware for Open Source
experimentalism was a great breakthrough. Potentially, you could network
everything with everything, make alternative ad-hoc infrastructures.

Those breakthroughs in peer based innovation fell into a climate that
was thick with promises. The early 2000s were full of techno-political
hopes. The tone had been set by Wizards of OS in 1999, which was the
first significant attempt (to my knowledge) to think through Free and
Open Source Software also as a political project.

*Political* means in this case, it has a social significance beyond that
usually granted to software. The success of GNU/Linux and the things
that could be done with it arrived in the art scene – but also the
intellectuals of social sciences, etc. – to ask questions about what
that freedom or openness was and if and how you could harness that for
other things than software.

Looking back at this period, a number of things happened in close
proximity: Creative Commons was making a breakthrough with having one
million of its licenses used in 2003. Wikipedia was started in 2001 and
was gaining critical mass. Many GNU/Linux distributions appeared for
creative tasks, such as Dyne.org, Puredyne, Knoppix. The protocol
Netsukuku[^04chapter4_12] was developed, a really explicitly political technology,
a peer based routing protocol. It has changed a lot since its first
release in 2005 and now seems to take on a very interesting
direction.[^04chapter4_13]

In 2003 together with FACT, commissioned by Michael Connor, we made a
brochure and DVD, with Kingdom of Piracy.[^04chapter4_14] It was like a toolbox for
free culture, in software, intellectually, in art.

![](media/image3.jpeg){width="3.9756944444444446in"
height="2.9868055555555557in"}Fig. 20. The many-headed hydra of
community mesh.

The early 2000s were an era of rapid growth of the digital commons. The
network commons in practice enabled a range of other creative practices.
At the time, do-it-yourself map making and the larger framework of
locative media was an exciting new topic, debated at the Cartographic
Congress in London 2003 and two workshops organized by RIXC in Latvia.
WLAN technology opened the possibility of so called war-driving, of
driving or cycling or walking through an area with a laptop or similar
device, scanning for networks. Depending on the ethical stance taken by
those doing the scanning, no intrusion happens, but the information
gathered can be used for location based tasks.

![](media/image4.jpeg){width="4.938194444444444in"
height="3.703472222222222in"}Fig. 21. Warwalk.

One thing that can be done is simply measuring the signal strength of
WLAN networks. You can also use the IP addresses for WLAN triangulation
– establishing your own location in relation to geolocative database
information. This enabled art driven, non-commercial projects to
experiment with locative media art, at a time when commercial
applications were still lagging behind. The network commons and locative
media art seemed like a perfect marriage, but it was a short spring.
While OpenStreetmap may have made rapid gains in 2003, Google Street
Maps was also released at around the time. Mapping became part of this
sprawling data monopoly. Many of the ideas that were hatched around the
early to mid 2000s by independents and small groups ended up getting
recuperated by the info-oligarchy.

Around that time the moniker *Web 2.0* was introduced. A lot of the
things that were the product of community based innovations and were
created in a decentralized way, were reunited in a new centrality, the
soon to rise monster of *social media*. As Evgeny Morozov explains, the
capacity to coin those terms gives a lot of interpretative power to
Silicon Valley.[^04chapter4_15]

In my view, you could say that the early 2000s were a time when a
peer-to-peer view of the world was formulated on many layers. Michel
Bauwens and the P2P foundation’s Wiki[^04chapter4_16] may also give testimony to
that. But these were still ideas by a relatively small elite. The
majority of the world was busy with *the war on terror*. As we now know,
it was used as a pretext to build a gigantic surveillance machinery.

Web 2.0 turned out to be the slogan of commodification of
community-based innovation, while under the surface massive data
harvesting is going on. As an economic model, it was not to last.

The banking crash of 2008 reveals a systemic crisis. The informational
paradigm does not see effective demand in the rich countries, there is a
downward pressure on the cost of labor, and all those conditions have
not significantly improved since the crash. The former West is in crisis
and community-based innovation could be a way out of it.

Wireless community networks should not be considered in isolation but as
part of this larger movement for the commons as the last great liberal
utopia. Already before, but now intensified, people start getting
involved in food coops, urban gardening, time sharing economies of all
kinds. Peer based commons production makes sense when capitalist ways of
organization break down. A project to bring wireless community networks
to deprived areas in Detroit, the Digital Stewards project, has received
mainstream media attention recently.

The former motor city is still in a process of de-urbanization. Inner
city communities have appallingly low broadband connection rates, a
digital divide reminiscent of a developing country in the heart of
industrial America.[^04chapter4_17] A project to bring WLAN to a community on the
outskirts of Valparaiso, Chile, has started and gets documented on these
pages here.[^04chapter4_18]

[^04chapter4_1]: Heather J. Meeker, *Open Source and the Legend of Linksys*, Linux
    Insider, 28.06.2005,

    http://www.linuxinsider.com/story/43996.html.

[^04chapter4_2]: Here is a long list of devices on which it is possibly running:
    OpenWrt: Table of Hardware, http://wiki.openwrt.org/toh/start.

[^04chapter4_3]: Fab, ‘Interview mit Sven-Ola Tuecke’, Wireless-Forum, 15 March
    2006, archived October 2007,
    https://web.archive.org/web/20071029082121/http://www.wireless-forum.ch/forum/viewtopic.php?t=16140.

[^04chapter4_4]: Elektra, ‘OLSR 0.48 zum Download freigegeben’, Indymedia, 7
    December 2004, archived February 2005,
    http://de.indymedia.org/2004/12/101054.shtml.

[^04chapter4_5]: rc.fn runcommand reality check freenetworks, panel at WOS3, 10
    June 2004, http://www.wizards-of-os.org/index.php?id=926.

[^04chapter4_6]: Armin Medosch, ‘run command free networks – a reality check’,
    Workshop at WOS3, 10 June 2004,
    http://www.wizards-of-os.org/index.php?id=719.

[^04chapter4_7]: Dewayne Hendricks, ‘One Gigabit or Bust™ Initiative – A Broadband
    Vision for California’, at WOS3, 10 June 2004, Abstract:
    http://www.wizards-of-os.org/index.php?1659; Video:
    https://archive.org/details/3\_do\_t1\_13h\_2-Hendricks/3\_do\_t1\_13h\_2-Hendricks\_hi.mp4.

[^04chapter4_8]: Berlin OLSR Wireless Mesh Testbed at Wizards of OS 3,
    free2air.org, 16.06.2004,
    http://www.free2air.org/story/2004/6/16/103734/486/.

[^04chapter4_9]: Corinna Elektra Aichele, ‘Mesh – Drahtlose Ad-hoc Netze’, Open
    Source Press, München, 2007. Extract available at:
    https://download-master.berlin.freifunk.net/ebooks/mesh\_kapitel4\_leseprobe.pdf.

[^04chapter4_10]: Cornelius Keller, OLSR-Experiment, archived December 2005,
    https://web.archive.org/web/20051211030128/http://olsrexperiment.de/.

[^04chapter4_11]: Freifunk, Ergebnisprotokoll CoreMeeting 2004-10-20, Freifunk
    Wiki, archived February 2005,
    https://web.archive.org/web/20050219235855/http://www.freifunk.net/wiki/CoreMeeting20041020.

[^04chapter4_12]: Wikipedia: Netsukuku, http://en.wikipedia.org/wiki/Netsukuku.

[^04chapter4_13]: Ibid. Netsukuku development and mailing list traffic appear to
    have ceased circa 2009.

[^04chapter4_14]: Kingdom of Piracy (KOP), online workshop, 22 February 2003 – 26
    March 2003, archived March 2016,
    https://web.archive.org/web/20160303075302/http://www.fact.co.uk/projects/kingdom-of-piracy.aspx.

[^04chapter4_15]: Evgeny Morozov: ‘The Meme Hustler’, The Baffler, April 2013,
    http://www.thebaffler.com/salvos/the-meme-hustler.

[^04chapter4_16]: P2P Foundation Wiki, https://wiki.p2pfoundation.net/.

[^04chapter4_17]: Detroit Digital Stewards,
    https://detroitdigitalstewards.tumblr.com/.

[^04chapter4_18]: Ignacio Nieto, ‘Free Mesh Networks. Two Cases from Chile’, The
    Next Layer, 31 May 2015
    https://webarchiv.servus.at/thenextlayer.org/node/1325.html. See
    also section 12.1 of this book.
