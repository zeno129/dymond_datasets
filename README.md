# DYMOND datasets
Datasets used for DYMOND


## Original Dataset Statistics

| **Dataset**     | **Nodes** | **Temporal Edges** | **Time Span**      |
|-----------------|-----------|--------------------|--------------------|
| CollegeMsg      |     1,899 |             59,835 | 193 days           |
| Enron           |    87,273 |          1,148,072 | 5 years (approx.)  |
| EU emails       |       986 |            332,334 | 803 days           |
| DNC emails      |     2,029 |             39,264 | 5 months (approx.) |
| Facebook Wall   |    46,952 |            876,993 | 6 years (approx.)  |

### Subset Statistics

| **Dataset**     | **Nodes** | **Temporal Edges** | **Unique Edges** | **Timesteps**     |
|-----------------|-----------|--------------------|------------------|-------------------|
| CollegeMsg      |     1,083 |             34,328 |            5,589 |                31 |
| Enron           |       785 |              5,794 |            2,517 |                20 |
| EU emails       |       784 |             68,091 |            6,878 |                79 |
| DNC emails      |     1,579 |             33,378 |            3,911 |                23 |
| Facebook Wall   |     2,245 |             23,507 |            4,976 |                43 |

---

## Datasets Description

#### CollegeMsg

This dataset is comprised of private messages sent on an online social network at the University of California, Irvine. Users could search the network for others and then initiate conversation based on profile information. An edge (u, v, t) means that user u sent a private message to user v at time t. Subset is for April 2004.

From Tore Opsahl &mdash;

> The Facebook-like Social Network originate from an online community for students at University of California, Irvine. The dataset includes the users that sent or received at least one message (1,899). A total number of 59,835 online messages were set over 20,296 directed ties among these users. This dataset was the main dataset used in my Ph.D. thesis. This network has also been described in Patterns and Dynamics of Users’ Behaviour and Interaction: Network Analysis of an Online Community and used in a number of articles including Prominence and control: The weighted rich-club effect and Clustering in weighted networks. Although this dataset contains many nodal attributes (e.g., gender, age, and course attended), these are not made available as it would be possible to reverse engineer the anonymisation procedure of users. Self-loops in the longitudinal edgelist signal the time that users registered on the site.

**Sources:** [SNAP](http://snap.stanford.edu/data/CollegeMsg.html) <sup>[9]</sup>, [Original](https://toreopsahl.com/datasets/#online_social_network) <sup>[10]</sup>

---

#### DNC emails

This is the directed network of emails in the 2016 Democratic National Committee email leak. The Democratic National Committee (DNC) is the formal governing body for the United States Democratic Party. A dump of emails of the DNC was leaked in 2016. Nodes in the network correspond to persons in the dataset. A directed edge in the dataset denotes that a person has sent an email to another person. Since an email can have any number of recipients, a single email is mapped to multiple edges in this dataset, resulting in the number of edges in this network being about twice the number of emails in the dump. Subset is April-May 2016.

**Sources:** [KONECT](http://konect.cc/networks/dnc-temporalGraph/) <sup>[1]</sup>, [~~Original~~](http://www.rene-pickhardt.de/extracting-2-social-network-graphs-from-the-democratic-national-committee-email-corpus-on-wikileaks/) (Original page seems hacked)

---

#### Enron emails

The Enron email network consists of 1,148,072 emails sent between employees of Enron between 1999 and 2003. Nodes in the network are individual employees and edges are individual emails. It is possible to send an email to oneself, and thus this network contains loops. Subset of February 2000 is around the mid-timeline of the Enron scandal.

**Sources:** [KONECT](http://konect.cc/networks/enron/) <sup>[1]</sup>, [Original](https://www.cs.cmu.edu/~enron/) <sup>[3]</sup>

---

#### EU emails

This is the email communication network of a large, undisclosed European institution. Nodes represent individual persons. Edges between two persons are directed and denote that at least one email has been sent from one person to the other. All edges are simple: Even if a person has sent multiple emails to another person, the two persons will be connected only by a single edge in that direction. Spam emails have been removed from the dataset. Subset consists of 79 days.

**Sources:** [KONECT](http://konect.cc/networks/enron/) <sup>[1]</sup>, [Original](http://snap.stanford.edu/data/email-Eu-core-temporal.html) <sup>[6]</sup>

---

#### Facebook wall posts

The is the directed network of a small subset of posts to other user's wall on Facebook. The nodes of the network are Facebook users, and each directed edge represents one post, linking the users writing a post to the users whose wall the post is written on. Since users may write multiple posts on a wall, the network allows multiple edges connecting a single node pair. Since users may write on their own wall, the network contains loops. Subset is August-September 2009.

**Sources:** [KONECT](http://konect.cc/networks/facebook-wosn-wall/) <sup>[1]</sup>, [Original](http://socialnetworks.mpi-sws.org/data-wosn2009.html) <sup>[4]</sup>