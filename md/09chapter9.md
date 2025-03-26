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


# 9. The Obsessive Utopia of Mesh Networks 

‘The sleeping beauty of mesh has been kissed into life by the
community’, explains Elektra in her book. The community has made it
possible to have decentralized wireless networks which connect small
local cells, automatically by intelligent software (Aichele 2007, p.
15). In this chapter, a closer look at developments around mesh networks
is taken, based on a study trip to Barcelona, supplemented by further
research. This chapter also asks the difficult question, how the
mystifications of technology might be overcome. Are better mesh routing
protocols really the answer to all problems?

In one of the previous chapters I stated that there is a significant
difference between town and countryside. In many rural areas, it is
virtually impossible go get affordable broadband internet. This problem
has actually furthered the growth of wireless community networks in the
countryside. A widely shared view is that it is much more difficult to
mobilize people for wireless community networks in urban areas where a
variety of possibilities for network access exists and where the urban
topology makes networking difficult. This, however, while broadly true,
may not always be the case. In some areas in Barcelona, wireless
community networks are growing, and they are developing and using the
latest mesh network technologies.

Routing is generally a very interesting area. Dijkstra’s algorithm is
one of the earliest path finding algorithms, written by computer
scientist Edsger W. Dijkstra in 1956 and published in 1959.\
The Dijkstra algorithm is something as basic for the current political
and cultural system as cars – or traffic lights – were for the previous
one, but nobody knows it, except for experts, computer scientists,
techies. It would not surprise me if it was included in the *Evil Media*
book,[^09chapter9_1] since this is something that has become part of the
technological unconscious. It has an agency of its own, as a repressed
force. This is definitely the case with the information infrastructure.

The process of forwarding *packets* from one node to the next on the Net
is called routing. The politics thereby deployed concern fundamental
freedoms and rights. Until now, the neutrality of these protocols has
been maintained, because they are jointly developed by the IETF and
IEEE. The commonality of the Net depends on neutrality on some layer.
And even in the turbo-capitalist world we live in this is still
safeguarded. Mesh routing protocols are improvements of *normal* routing
protocols.

[]{#__DdeLink__10802_299379148 .anchor}Pau Escrich is one among a team
of researchers working on the Confine project and he is also a Guifi
activist:

I realized that in my district, a Barcelona neighborhood which is called
Sants, there was not any node of the Guifi.net project. So, following
the approach – think globally, act locally – I started contacting people
from the neighborhood. We built a nice group of folks interested in
building a free network, and after having some meetings we started
deploying nodes. Now, four years after this, we have around 50 nodes in
this area.

Pau and colleagues started using new technology based on mesh routing
protocols. Most of Guifi.net does not use mesh protocols, but standard
routing technology such as the Border Gateway Protocol (BGP). In such a
network, a group of routers under a single administrative policy – an
Autonomous System (AS) – is managed using BGP for interior and exterior
routing. If you compare an AS with a country, the router controls
entrance and exit to that country. The benefit is that for nodes inside
this *country* it is not necessary to know the route to each and any
other node on the net, it only needs to know the nearest gateway router.

![](media/image1.jpeg){width="4.4118055555555555in"
height="3.3090277777777777in"}Fig. 29. Paul Baran, Network Topology.

The resulting network topology is one that could be described as
decentralized, according to the classification of Paul Baran’s seminal
study from the early 1960s (see image above). A decentralized topology
is a mixture between a hierarchical, star-shaped network and a
completely distributed or mesh network, without any nodes taking on a
notion of a center.

In Catalonia, Guifi.net has a decentralized topology with SuperNodes
which are connected with each other and to which are connected many
Nodes, which are only connected to the SuperNode, but not to each other.
This works reasonably well but does not fulfill the criteria of the
wireless community network dispositif which demands a more egalitarian
topology. Pau Escrich:

The SuperNode network creates what we call the Backbone, and this
Backbone network is decentralized, but the level below (the Nodes layer)
is very centralized, and it represents more than 80% of the network
devices. So this is an actual control point; the groups, individuals or
companies controlling these SuperNodes are the actual managers of the
network. This is what we are trying to skip by developing and using QMP.

QMP stands for Quick Mesh Project, a GNU/Linux distribution based on
OpenWRT and specifically made for mesh networks. QMP is based on a
predecessor project which was developed in the context of another
community network initiative. In 2007, a small group in Gracia, a
pleasant neighborhood in Barcelona, which extends from just behind
Sagrada Familia into a more leafy and hilly area, started a small mesh
network called GSF. Roger Baig, a key figure in Guifi.net, was involved
in this. Roger Baig, according to his self-description, had been
involved in free software since the 1990s and ‘installed a server in
each village around my area. Initially’, he said, ‘I was not so skilled
in networks, still learning, so OpenWRT was fresh air for me.’

The group looked for funding and managed to win a contest organized by a
foundation named PuntCat (dot-cat are Top Level Domain managers). They
received 15,000 Euros to start the project, reports Pau Escrich.

The development of QMP then started seriously after 2010, when a small
group of convinced mesh networkers dedicated themselves to building a
new distribution from scratch. Part of this group was the German Axel
Neumann who at the time also lived in Gracia. After three years they
launched the first stable release, and QMP is now used at many places
around the world.[^09chapter9_2] Axel Neumann is key developer of BMX6,[^09chapter9_3] one
among a number of the latest incarnations of B.A.T.M.A.N.,[^09chapter9_4] a mobile
ad hoc mesh network protocol.

Axel Neumann is writing software for the Confine project. He is helping
to run the testbed, Community Lab. He is also main developer of BMX6,
one of a number of B.A.T.M.A.N. forks. Axel was fascinated with complex
problems early on, problems such as how to make a map of a landscape
that constantly changes; or how to have routing tables in a network
where constantly nodes appear and disappear? Axel was getting interested
in B.A.T.M.A.N. through Freifunk. Pau Escrich:

B.A.T.M.A.N. was born in Berlin as an alternative to OLSR. Its approach
is different for a node running the routing protocol; instead of knowing
all the network topology (as OLSR does), in B.A.T.M.A.N. every node only
knows its new best step to reach any other node in the network. So if
all the network participants are doing the same, the user data will be
routed from one side to the other following always the best path. This
approach is called distance vector.

B.A.T.M.A.N. is actually an acronym and stands for *better approach to
mobile ad-hoc networking*. The initial idea came from Corinna *Elektra*
Aichele, who also started developing it, and was soon joined by Axel
Neumann in this effort. To cut a long story short, after B.A.T.M.A.N.
emerged as an alternative to OLSR – the latter the first mesh protocol
which became more widely used by the community – a rivalry developed
which inspired the *Battle of Mesh Networks*. This is a kind of contest,
where community networkers meet to test and compare different
protocols.[^09chapter9_5] Meanwhile, a number of different flavors of B.A.T.M.A.N.
exist besides BMX6.

B.A.T.M.A.N. is a distance vector protocol. OLSR is a link state routing
protocol where every node has a map of the network and can make
decisions about where to send packets first. Distance vector, Axel
explains, is more like I send somebody on a hike without giving him a
map, but telling him to look out for the signs. Distance vector is more
simple, in a certain way, but has other consequences. The signs have to
be put in place and they have to be kept up to date. This is done by
flooding the net with messages from the target node. Axel is now working
on BMX6, trying to improve the way how this flooding of messages is
done. ‘Speaking in the abstract,’ Axel explains, ‘it is like compressing
data.’ Pau Escrich:

We choose BMX6 because it fits our requirements: scalability, good
performance, capable to run on a low-resources machine and IPv6 support.
In addition Axel Neumann, its main developer, is a good friend of the
Guifi.net community and he joined the QMP team, so we are really having
a routing protocol which is very adapted to our needs.

Programmers such as Axel and Pau are deeply fascinated about the
capacities of mesh protocols like OLSR or B.A.T.M.A.N. in terms of
self-organization. In the network topology of Guifi.net as described
above, a SuperNode may control 50 or 100 nodes. While the backbone is
decentralized, the leafs are very centralized. For community network
activists, the network topology is not just a technical issue, it also
expresses a political desire. Pau Escrich:

When I was a kid, I was enthusiastic about Che Guevara, Gandhi and these
people in history who changed the world and fought for the freedom of
ordinary people. I also liked computers a lot. So I found the free
software movement as a perfect scenario to follow my ideas.

The mesh networking community is striving to build a completely
egalitarian, uncensored, free and open network. Axel Neumann believes
that the future belongs to multi-policy routing. Each node decides
autonomously but still everything works together. In Community networks,
it would be too much asking constantly for meetings to make policy
decisions. B.A.T.M.A.N. advanced, the other main B.A.T.M.A.N. fork, uses
Layer 2 of the internet. The user feels like hanging on one switch, but
Axel says he cannot be sure how far this can scale. Axel would propose
to have a cloud using B.A.T.M.A.N. Advanced and BMX for long distance
connections. Locally, the user will be able to move from cell to cell as
with a mobile phone.

Distributions with several mesh protocols are already in actual use in
Spain, Germany, Austria, Argentina, and Nicaragua, in Chile possibly
too. A major effort for a new distribution is called LibreMesh.[^09chapter9_6] It
is an attempt at globalizing the Freifunk firmware undertaken by several
community networks across continents, including Freifunk, Ninux, and
Guifi, together with people in Argentina.

The latest Freifunk distribution, Kathleen, also has B.A.T.M.A.N. and
OLSR installed. It offers a lot of improvements in the direction of
auto-configuration and ease of use and better management of IP spaces
and DNS services.[^09chapter9_7] With regard to the politics of Freifunk, I was
able to make interesting observations when a massive flamewar broke out
between someone, who apparently wanted to use the Freifunk label for his
own cause, and everybody else.

The discussion about what makes a network *free* or *open* was raging on
WLAN-News, one of the main Lists for exchange on Freifunk issues. The
story, which had rumbled already through local Freifunk lists, was that
one wannabe entrepreneur wanted to do something *like* Freifunk and with
its endorsement and under the subdomain, but with policies contradicting
some rules. It seems he wanted to make his own network and use a tall
building, paying someone to have a router there on his balcony.

The ensuing discussion was like a look into the collective psyche of the
Free radio community. The community objected to a whole range of issues,
but one of them was that the other network would not mesh. Admittedly
the *entrepreneur* did not make his own case easier with a very angry
tone, accusing Freifunk of acting like a closed shop. The whole idea
smacked of opportunism. But what I found interesting was the emotional
intensity with which mesh was argued as a political project. Only the
mesh network is really a free network.

On one hand, I do believe that things such as LibreMesh can make a
difference, since it creates the possibilities of a global, independent
infrastructure, the network commons, reclaimed by its users.

In political terms, this could either be described as libertarian, or
anarchist or grassroots, bottom-up, self-organized democracy. The desire
of mesh network developers is to give the net a technical structure
which makes it difficult to impose any top-down control structure.

In my ears, this sounds a bit like the initial idea behind the internet
in the first place. However, as the history of the Net has shown, such a
decentralized structure on the technological level does not make the Net
immune from other forms of centralization and control. Capitalism knows
many ways of bending and taming the liberatory potential of new
technologies. Google is the best example, it can exert control without
directly owning the whole of the Net, it does not need to shape the
traffic flows of the Net at control points such as routers or hubs.

In my conversations with community network activists, I tried to explain
that a decentralized network can also serve top-down organizations and
vice versa, that a centralized network could also serve the struggle of
a movement for freedom. This winter, I visited the Museum of Revolution
in Havana where you can see the radio transmitters built by technicians
for Fidel Castro and Che Guevara. There was nothing decentralized about
this technology, but it served the purposes of the revolutionary
struggle perfectly well. Whenever I try to make such an argument, it
seems I am running against walls.

‘If you have a centralized network you have a weak network; distributed
things are the basis for the freedom of technologies’, Pau insisted. The
*freedom of technologies* is constituted by the three freedoms of Eben
Moglen introduced earlier in this text: free software, free networks,
free hardware. Basically, everyone from Guifi.net whom I interviewed
repeated those three freedoms to me like a mantra.

Pau Escrich and Roger Baig are part of a group of community networkers
and researchers, who work at Universitat Politècnica de Catalunya (UPC),
Barcelona, Spain in the framework of the EU funded project Confine.[^09chapter9_8]
This project brings together community networkers, but also academic
computer scientists and telecommunications researchers, to build
Community Lab, a testbed for many new WLAN applications.

One of them is Llorenç Cerdà-Alabern who is an Associate Professor at
UPC. He also lives in the district of Sants and wanted to contribute
something practical to this project. So he put an antenna on his roof
which has now become a hub in the mesh in Sants built using QMP. Llorenç
thinks that this cooperation between networking enthusiasts and academic
researchers is beneficial because the community is much more oriented
towards practical results whereas researchers can look further into the
future.

Llorenç is using his position in the network topology to conduct some
experimental measurements and to write papers about it.[^09chapter9_9] He has also
written a topology generator, a tool that visualizes the network between
Sants and UPC.[^09chapter9_10]

The community network provides the unique opportunity to have live field
tests running, studying relatively large scale wireless networks under
real conditions. Ivan Vilata-i-Balaguer is also working in the Confine
project. His responsibility is to provide services for the
implementation of the testbed, Community Lab.[^09chapter9_11]

‘We have the community device’, explains Ivan, ‘we chose to run the
experiments on a separate device.’ The community lab testbed is actual
hardware, a device which is put next to nodes at community networks, and
on this device are running some experiments. So they had to ask a lot of
questions, explains Ivan, questions such as ‘How do we manage all this
hardware? We are talking about nodes on the community network which can
be used to run experiments.’

Most research is usually done in controlled environments, by research
groups, but there are no users. In a community network with real users,
explains Ivan Vilata-i-Balaguer,

‘the experiments must not overwhelm the community network with traffic,
must not crash it, when experiments crash, and it also should not affect
node ownership, so we cannot expect total control from the testbed
operator; we had a lot of open topics to think about and we had to find
an architecture that meets all these requirements.

The research devices can be used for different experiments, remotely
controlled from servers hosted at an organization called Pangea.
According to Ivan Vilata-i-Balaguer, in July 2014 there were 120 to 130
research nodes, of which about 90 were in perfect working condition,
‘but we are expanding the testbed and developing the software.’

The maintenance of the research devices is an issue, because most of the
nodes belong to individual node owners, so updating of the software and
keeping the nodes in working-order is precarious. As a result, now most
of the nodes which are connected to a research device ‘are operated by
people who work for CONFINE, so the communication overhead is not so
big’, explains Ivan. Confine merges community network and academia in
the same project. It enables, for example, advanced monitoring
capacities which can be used by Guifi.net to have a transparent network
and enforce the rules and principles of the network commons. It also
enables more experimental topology generators such as the one by Llorenç
Cerdà-Alabern; but this is just a fraction of what is going on.

The project is also providing data sets from those measurements for
other researchers.[^09chapter9_12] This page gives an overview of all the partners
and activities, such as Athens Wireless. Ninux in Italy, Funkfeuer and
many more.[^09chapter9_13] As part of the project, a whole range of social projects
have been added through an open call.[^09chapter9_14] One of those projects is
CONFLATE, which uses ‘the new Research Devices of Ninux.org to deploy a
simple (but practical) OpenFlow based DASH Live Video Streaming service
for real users of Ninux.org,’ informs the website. This and other
projects will be topics of future articles.

However, at the risk of being seen as a party popper, I feel the need to
also share an observation which stems from rather long-term engagement
in the field. It seems that many participants in this movement display
facets of what Joseph Weizenbaum called the obsessive-compulsive
programmer.\
In his 1976 book *Computer Power and Human Reason*,[^09chapter9_15] Weizenbaum, as
a big critic of computer science from within, wrote this famous passage
about the

bright, young men of disheveled appearance, often with sunken glowing
eyes, \[who\] can be seen sitting at computer consoles, their arms
tensed and waiting to fire their fingers, already poised to strike, at
the buttons and keys on which their attention seems to be as riveted as
a gambler’s on the rolling dice.

The real issue here is not about appearances and also not about
finger-pointing at computer enthusiasts or techies, as I prefer to call
them. We should not make techies []{#__DdeLink__10804_299379148
.anchor}culpable for what are actually the contradictions of this
society. In the knowledge economy, almost everyone is quite compulsive
about their work, and in the 21st century many people have become
*hackers* according to McKenzie Wark’s
definition.[]{#footnoteref3_3bpuqfs .anchor}[^09chapter9_16] In *Fun and Software*,
a recent book edited by Olga Goriunova, one of the pioneers of Software
Studies, the authors treat this subject in a more even-handed
way.[]{#footnoteref4_cixn2yq .anchor}[^09chapter9_17] Wendy Hui Kyong Chun and
Andrew Lison argue that there is a dialectic at work between fun and
exploitation.[]{#footnoteref5_kghw1ug .anchor}[^09chapter9_18] Techies such as
Linus Torvalds write software *just for fun* but their political naivety
makes them also subject to exploitation. For some, the fascination with
technology, which itself is not the real problem, can turn into a
compulsive obsessive disorder.

The real problem seems to be not the obsession, which is actually
driving innovation, but the one-sided belief that there is a
technological fix for each and any social ill. The bigger question
rumbling throughout this book is whether community networks can alter
the course of technology and whether a different relation between
technology and society can emerge which could help to make society more
democratic. The simple answer to the first part of the question is
almost certainly a bold Yes!, of course. Community Lab certainly helps
to generate a lot of data to improve mesh protocols and develop new
methods and services. Yet the second part of the question is much more
complex and demands further explanations.

In capitalist societies a heightened division of labor develops which
drives people into increasing specialization. As a result, information
and communication technology (ICT) is for most people a black-box. They
use it, but have no idea how it works. This allows to create what
Critical Theory used to call the *mystifications of technology*.
Societies get ever more fragmented, whereby small elites command a lot
of power by using money and technology. To ordinary people then it looks
like they are controlled by technologies, mistaking social relations for
relations between things. As technology becomes *mystified* in this way,
the solution to the problem appears to be to create even better
technology.

While techies, as individuals and citizens, might actually disagree with
the political status quo and desire a free and egalitarian society, the
course of technology as such – driven by their own free labor, produced
out of their obsession with creative computing – exacerbates those
divisions between powerful elites and ordinary user-citizens. Techies
passionately belief that Free and Open Source Software (FLOSS) will help
to counter such developments. But while those technologies are
transparent to experts, for ordinary people they are as opaque as a
brick wall. Social mechanisms intrinsic to the techie community actually
make matters worse.

The idealistic techie communities who produce FLOSS tend to have a
missionary zeal about them and are very tightly knit *communities of
practice* who have created their own rules and codes, literally and
metaphorically. This world, as highly complex as it has become, of
practices and ethics, has few connections with the rest of society – it
works well within the community, where everybody carries the same rules
and values, but is completely impregnable for non-members.

Just to give an example, it is completely beyond me why the testing of
different mesh protocols has to be called *battle mesh*. People who are
otherwise really nice and sensible are using, without further
questioning it, a militarized language. This is a put-off for many
people who may otherwise be interested in joining those communities. The
problem goes even further. Mobile ad-hoc networks have initially been
developed by the US military. The new and improved mesh network
protocols are almost certainly used by the military again. Mesh
protocols can be used for creating swarms of semi- or fully automated
weapons in a battle field. These are issues that most people involved
would want to avoid. When directly asked, they give evasive answers.

The *mystifications of technology* could be reversed by a two-way
process which I tentatively call the socialization of technology. If
more people learn about how ICT works, it will become much less easy to
use and abuse those technologies by the powers that be. The
socialization of technologies would also imply that there are closer
links between the people who develop technology and those who use it.
This was the idea behind participatory design which was pioneered in
Sweden in the 1970s. Community networks in principle carry great hopes
for initiating and furthering such processes of participatory design and
socialization.

In reality, however, when I tried to find empirical evidence for those
claims, I mostly gathered evidence to the opposite. I wanted to find out
what drove people to work on those issues and how they developed the
criteria for their code. And the answer was in 90 percent of cases that
the criteria were implicit, that they were following a shared tacit
consensus according to which the coders developed the code. The question
of a *user* of a software lies at the bottom of concerns, as the
developers – or like-minded people – are the users themselves.

This self-referentiality of community network activists extends to the
three *laws* of Guifi.net. When asked about the freedom in free
networks, everybody was quick to come up with the answer that this
freedom was based on the open, free, and neutral character of the net.
The reality is that the initial utopia of self-provision of networks is
not really attainable. Most networks are built and maintained by
professionals and the users, by participating in such networks, learn
little or next to nothing about the technology. It remains a black-box
and thus mystified.

Yet for exactly that reason, *mesh* is so important in upholding the
decentralized utopia. If every node can mesh, you do not need expert
knowledge at each node. The dream of mesh, however, is a Promethean
fantasy inherent to all such technology, it is a form of the automatic
utopia. The idea is that community networks will proliferate freely once
mesh software is perfectly working and available.

In the meantime however, the actual problems and possible impediments
come from the social sphere, where lobby groups and continued
neoliberalism lead to a difficult environment for community networks. At
the time of writing, Freifunk in Germany finds itself in a renewed
battle against *Störerhaftung*, the law according to which a node owner
is responsible for anything that a user might do. This law seems to have
been created particularly to support the interests of the copyright
industry. Now, the German coalition government is drafting a new law
which, if passed, would make wireless community networks next to
impossible.[^09chapter9_19] The problem is a political one, not one of the
efficiency of battling mesh networks.[[]{#page-title36
.anchor}]{#__RefHeading___Toc109002_349971531 .anchor}

[^09chapter9_1]: Matthew Fuller and Andrew Goffey, *Evil Media*, MIT Press 2012.

[^09chapter9_2]: Quick Mesh Project (qMp), https://qmp.cat/.

[^09chapter9_3]: Bmx6 in OpenWRT, n.d., archived December 2013,
    https://web.archive.org/web/20131220025032/http://bmx6.net/projects/bmx6.

[^09chapter9_4]: Open-Mesh: B.A.T.M.A.N.,
    https://www.open-mesh.org/projects/open-mesh/wiki.

[^09chapter9_5]: The Wireless Battle Mesh is an ongoing annual convention: Wireless
    Battle Mesh, https://www.battlemesh.org/.

[^09chapter9_6]: LibreMesh, https://libremesh.org/.

[^09chapter9_7]: For a history of Freifunk firmware releases, incl. Kathleen, see
    Freifunk, Berlin: Firmware
    https://wiki.freifunk.net/Berlin:Firmware.

[^09chapter9_8]: Confine Project (2012-2015), archived October 2015,
    https://web.archive.org/web/20151003180403/https://www.confine-project.eu/.

[^09chapter9_9]: For instance: D. Vega, L. Cerda-Alabern, L. Navarro, and R.
    Meseguer. *Topology Patterns of a Community Network: Guifi.net*. In
    2012 IEEE 8th International Conference on Wireless and Mobile
    Computing, Networking and Communications (WiMob), 612–19, 2012.
    doi:10.1109/WiMOB.2012.6379139.

[^09chapter9_10]: The resulting page is definitely worth studying: Bmx6 Wireless
    Mesh, Sants-UPC, http://dsg.ac.upc.edu/qmpsu/index.php.

[^09chapter9_11]: For those more technically interested, there are some slides
    here: Ivan Vilata-i-Balaguer, Community-Lab: Exploring the Future
    Internet on Community Networks, slides of talk at FOSDEM 2014,
    archived May 2016,
    https://web.archive.org/web/20141126225209/http://wiki.confine-project.eu/\_media/pub:community-lab-intro\_fosdem-2014.pdf.

[^09chapter9_12]: Confine Wiki, Open Data Sets, archived November 2014,
    https://web.archive.org/web/20141126212934/http://wiki.confine-project.eu/experiments:datasets.

[^09chapter9_13]: Community Lab, archived December 2014,
    https://web.archive.org/web/20141217005023/http://community-lab.net/.

[^09chapter9_14]: Confine Wiki, Selected Open Call 2 experiments, archived November
    2014,
    https://web.archive.org/web/20141126212458/http://wiki.confine-project.eu/experiments:opencall2.

[^09chapter9_15]: Joseph Weizenbaum, *Computer Power and Human Reason: From
    Judgement to Calculation*. W.H. Freeman & Company, 1976.

[^09chapter9_16]: McKenzie Wark, *A Hacker Manifesto*. Harvard University Press,
    2009.

[^09chapter9_17]: Olga Goriunova, Fun and Software: Exploring Pleasure, Paradox and
    Pain in Computing. Bloomsbury Publishing USA, 2014.

[^09chapter9_18]: Wendy Hui Kyong Chun and Andrew Lison *Fun Is a Battlefield:
    Software between Enjoyment and Obsession*. In *Fun and Software:
    Exploring Pleasure, Paradox and Pain in Computing*, 175–96. London /
    New York / Paris: Bloomsbury Publishing USA, 2014.

[^09chapter9_19]: To support the Freifunk campaign against the new draft law,
    follow this link: ‘Christian Heise, Wir brauchen eure Hilfe – Helft
    mit die Störerhaftung für WLANs zu stürzen!’, 10 March 2015,
    https://freifunkstattangst.de/2015/03/10/wir-brauchen-eure-hilfe-helft-mit-die-stoererhaftung-fuer-wlans-zu-stuerzen/.
