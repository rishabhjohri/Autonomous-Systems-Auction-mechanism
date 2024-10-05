This programming exercise has been adapted from Problem 8 (Chapter 7, Multiagent
Systems by Gerhard Weiss)

Consider the following combinatorial auction scenario: a professor wants to supplement his
or her income by auctioning off advertising space on his or her lecture slides. 

The professor decides to use VCG as an auction mechanism and to offer two goods: a top banner space
and a sidebar space. Every advertiser’s type has two parts: vi
, which specifies its utility for an allocation that satisfies it; and fi ∈ {t, s, b}, which specifies what must happen for it to
be satisfied.

An agent with fi = t will be satisfied if it wins the top banner space, regardless of what
happens to the sidebar space.

An agent with fi = s will be satisfied if it wins the sidebar space, regardless of what happens
to the top banner space.

An agent with fi = b will only be satisfied if it wins both spaces. (It might only use one
space, but it insists on not having any other ad shown alongside its ad.)

(a) Let v1s denote the first-highest bid for slot s. (Similarly define v1t
, v1b, v2s, v2t
, v2b.)
Express the VCG revenue as a functio nof these values. Assume that the values are 0
if there is no corresponding bidder. Assume that the auctioneer breaks ties in favour of
bidders who want both slots. Write a program that computes the auctioneer’s revenue
for a given possible bidding scenario.

(b) Consider a setting where one of the agents is capable of creating a second identity (at
some very small cost α), and submitting bids using both identifies. (If it does so it gets
every good won by either identity, and must pay as per VCG norms.) Demonstrate
through experiments that VCG is not dominant strategy truthful in this case.

(c) Consider the following auction mechanism: allocate both goods to whichever advertiser
has submitted the highest bid, and charge him or her the amount of the second highest
bid (ignoring the fi element of their types). Demonstrate through experiments that
this mechanism has the following properties.

– the agents have a dominant strategy of reporting truthfully, using only their true
identities

– in equilibrium, the mechanism generates at least half as much revenue as VCG
would if the agents submitted truthful reports.

You may choose a suitable format of your input data file. The input would comprise
the bids submitted by the participating advertisers (bidders). There can be any number of
bidders.

Your submission must include a report describing the experiments done, source code, and
the input files.
