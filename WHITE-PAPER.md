![alt tag](https://cloud.githubusercontent.com/assets/24201238/24583976/ced4c43e-179f-11e7-9c40-c0988c346f55.png)

_**Publish research for free, access research for free.**_

# Aletheia: A blockchain for scientific knowledge with a community management framework

## By Kade Morton and the Aletheia Community
## kademorton@protonmail.com
## contact@aletheia-foundation.io

## Table of Contents
- [Introduction](#introduction)
- [Why is Aletheia important?](#why-is-aletheia-important)
  - [A blockchain journal](#a-blockchain-journal)
  - [The problems with the prestige system](#the-problems-with-the-prestige-system)
  - [A new reputation ecosystem](#a-new-reputation-ecosystem)
  - [A peer to peer journal](#a-peer-to-peer-journal)
  - [A community journal](#a-community-journal)
- [Submitting documents to Aletheia](#submitting-documents-to-aletheia)
  - [Thresholds](#thresholds)
  - [Storage in Aletheia](#storage-in-aletheia)
  - [Voting reputation](#voting-reputation)
- [Acceptance into Aletheia](#acceptance-into-aletheia)
- [Peer review](#peer-review)
  - [Short List peer review](#short-list-peer-review)
  - [Entire Pool peer review](#entire-pool-peer-review)
  - [Anonymity](#anonymity)
  - [Rounds of peer review](#rounds-of-peer-review)
- [Cryptographic Control](#cryptographic-control)
- [The content of Aletheia](#the-content-of-aletheia)
  - [Creative Commons Licenses](#creative-commons-licenses)
  - [Removing non-academic content](#removing-non-academic-content)
  - [Assessing takedown orders](#assessing-takedown-orders)
  - [Complying with takedown orders](#complying-with-takedown-orders)
- [Access and identity management](#access-and-identity-management)
- [The incentivised seeding problem](#the-incentivised-seeding-problem)
- [Community](#community)
  - [What reputation will be scored on](#what-reputation-will-be-scored-on)
- [Smart contracts](#smart-contracts)
  - [Smart contracts for Aletheia's governance](#smart-contracts-for-Aletheias-governance)
  - [Smart contracts for managing the Aletheia Foundation](#smart-contracts-for-managing-the-aletheia-foundation)
- [Revenue model](#revenue-model)
  - [Community fundraising](#community-fundraising)
  - [Computing power](#computing-power)
  - [Paid version](#paid-version)
  - [Paid peer review](#paid-peer-review)
- [Why blockchain?](#why-blockchain)
- [Out of scope but desirable](#out-of-scope-but-desirable)
- [Outlook on blockchain and science](#outlook-on-blockchain-and-science)

## Introduction
Aletheia is a decentralised, open source, open access scientific journal. It is a free client that runs on Windows, Mac and Linux, that allows the user to upload academic papers and datasets, as well as search for academic papers and data sets. The Aletheia client enforces sharing of documents with other uses also running the Aletheia client, forming a peer to peer network. Hashes of documents, metadata for documents, reputation accrued by documents, actions of users and community decisions are stored on the Ethereum blockchain. The community administers Aletheia through a community management framework of smart contracts, making Aletheia a decentralised autonomous organisation ([DAO](https://en.wikipedia.org/wiki/The_DAO_(organization))). Aletheia is a free open source platform that allows users to share and access scientific information without being hindered by paywalls. It encourages peer review and creates its own reputation ecosystem to provide an alternative to the current prestige system that dominates academic publishing with detrimental consequences. Information is stored on the blockchain to allow version control of documents and provide resiliency to the information in the network. Aletheia allows individuals to have a say in the future of the platform and allows the community to administer the platform through direct democracy.

## Why is Aletheia important?
It was estimated in 2010 that roughly 50 million scientific articles had been published to date [1](http://www.ruor.uottawa.ca/bitstream/10393/19577/2/Jinha_Arif_2010_Article_50_million.pdf). It is unclear what percentage of scientific articles are behind paywalls but given a cursory search for scientific articles online will more often than not lead to a paywall, it can be surmised that a large percentage of scientific articles are behind paywalls. That is to say, a large percentage of humanity’s collective knowledge is only accessible by those with financial means. To put the term ‘financial means’ in context, in 2012 the Harvard Library published a letter stating that it was paying close to $3,750,000 USD a year in journal subscriptions and that this state of affairs was financially untenable, meaning the library planned on cutting back the number of journals on offer to students [2](http://gantercourses.net/wp-content/uploads/2013/11/Faculty-Advisory-Council-Memorandum-on-Journal-Pricing-§-THE-HARVARD-LIBRARY.pdf). If Ivy League institutions cannot afford scientific journals, what chance does an institution in a developing nation, or even just your average individual have? Cutting off every person who doesn’t have the financial means to pay exorbitant fees for scientific knowledge is fundamentally wrong. Aletheia is a proposal to go some way to correcting this error while also fostering a movement against paywall journals. 

But open access already exists. Open access journals are scientific journals that do not restrict access to scientific information. While Aletheia adheres to the principles of open access it is different to existing open access journals in a number of ways. Most journals today are not in paper form and papers accessed through the journal's website that allow searching of a centralised database in the background. Aletheia is a downloadable peer to peer client, which prevents centralisation through control of the website or control of the back end database. The information stored in the Aletheia network is spread across all users running the client and the Ethereum blockchain, ensuring Aletheia is not beholden to any single interest and is controlled by the community. Due to its decentralised nature along with providing an alternative to the current prestige system and allowing the community to directly administer the platform, Aletheia contributes something currently lacking from the current open access ecosystem.

### A blockchain journal 
A blockchain is a distributed ledger that through cryptographic means can only be added to, not subsequently changed. For a thorough technical explanation of a blockchain, please see Satoshi Nakamoto’s original paper, [Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf). Aletheia utilises a blockchain to achieve a distributed and tamper proof database of information, storing document metadata, vote topics, vote results and information specific to users such as reputation and certifications. Due to the distributed nature of the stored information, Aletheia is a decentralised application that isn't controlled by any one party, it is administed by the community.

### The problems with the prestige system
The often cited reason existing open access journals don't grow to rival their paywall counterparts is due to the prestige that comes with being published in a large, well established paywall journal. For academics it is often more beneficial for their careers to publish in a large paywall journal [6](https://www.theguardian.com/science/2013/dec/09/nobel-winner-boycott-science-journals). Academia is ruled currently by the prestige system, where prestige is gerated by publishing groundbreaking work in prestigious journals. Doing so will positively influence your research career and posibility for grant funding, allowing you to condunct more research. Journal publishers know all too well this system of incentives binds researchers to them, people risk their careers, their income and future grants if they don't publish in prestigious journals. Since these journals effectively have a monopoly on academic communication, they can largely do what they want. This led to the introduction of paywalls to academic publishing. Publishing in top tier journals attracts prestige due to the stringent editorial and peer review process, but evidence show retraction rates for peer reviewed work is rising [3](https://theconversation.com/what-lesson-do-rising-retraction-rates-hold-for-peer-review-28823). 

There are a number of negative consequences to the prestige system. Human knowledge is concentrated behind paywalls, detrimenting the entirety of humanity by preventing access to scientific knowledge which robs humanity of scientific advancements. The power such journals weild is perpetuated by this concentrtion of knowledge. Academics are incentivised to sit on research that has negative findings or just isn't deemed "groundbreaking", meaning money and time is wasted, along with the fact that humanity's collective knowledge pool isn't added to. The prestige system is a complex socio-economic system perpetuated by journals and researchers themselves by rewarding publication in prestigious journals and punishing a lack thereof. It self-reinforces and is very difficult to remove. 

### A new reputation ecosystem
Aletheia allows reputation to be accrued by users and uploaded academic papers. Aletheia creates a reputation ecosystem that can be drilled down into the show the number of papers uploaded and their quality, number of citations the paper receives, number of reviews performed and their quality, number of decisions participated in and what decision was made. This information is a comprehensive record of a users contribution to science, which is more rigorous and scientific than the prestige model of publishing in top tier journals. While initially encouraging submissions to Aletheia, it's hoped this transparent and quantifiable reputation system could come to be seen as a preferred alternative to the prestige system that constricts academia today. It also offers a pathyway for others without specific scientific experience to engage with academia and have their skills valued and recognised, opening academia and making scientific research more inclusive.

### A peer to peer journal
Peer to peer file sharing is a method of file sharing where peer to peer software is run on a computer, making that computer a peer in a network of peers. This allows the computer to query other peers also running the same software, and once it has found a peer with the desired file it begins downloading a copy [4](https://en.wikipedia.org/wiki/Peer-to-peer). To facilitate the main function of Aletheia, the obtaining of scientific journals, the Aletheia client is a peer to peer file sharing client that allows the submission of academic papers and data sets for sharing through the client. Currently datasets are hard to obtain, often stored in online repositories separate from the papers themselves, one of Aletheia’s goals is to make data easier to obtain to assist with checking the veracity of articles. By downloading and running the Aletheia client you are becoming a peer in the distributed network.

### A community journal
Smart contracts are computer programs designed to execute a predefined action based on inputs. They are typically imagined as legal contracts written as programs [5](https://en.wikipedia.org/wiki/Smart_contract), but they can be used to create a community management framework. Smart contracts can be written to either perform one of two predefined actions, or simply to perform or not perform a predefined action based on number of votes received during a specified time frame. In this waty, the community directly administers Aletheia as a DAO through direct democracy, meaning anyone can take part in this open community and that Aletheia has no key person risk. Every smart contract, along with every time it is invoked and the outcome of the execution of the smart contract is stored on Ethereum to provide a fully transparent audit trail. Aletheia is also open source, allowing people to view the source, verify its security and contribute to it if desired. Because everyone has access to the code, the code can be hosted on any website for download, making Aletheia hard to censor. 

## Submitting documents to Aletheia
Once a user has installed the Aletheia client on their computer, they can upload academic papers and associated data sets to be shared with the Aletheia community. The user need not be one of the authors. Any paper, so long as it is not under copyright, can be uploaded. To facilitate the search function and allow the client to return papers on particular topics or from particular disciplines, metatdata is also required. This can be entered at time of submission to Aletheia, or it can be added at a later date by the community.

The metadata fields in Aletheia are based on the Dublin Core Metadata Element Set along with research author consultation:

* The contributors to the article
* Contributor identifiers, such as ORCIDs
* The date the article was published
* An abstract of the article
* The language the article is written in
* The publisher of the article if published elsewhere previously
* A list of related resources
* The source of the article’s contents
* The title of the article
* Discipline of the article, a drop down from:
  * Performing arts
  * Visual arts
  * Geography
  * History
  * Languages and literature
  * Philosophy
  * Theology
  * Anthropology
  * Economics
  * Law
  * Political science
  * Psychology
  * Sociology
  * Biology
  * Chemistry
  * Earth sciences
  * Space sciences
  * Physics
  * Computer Science
  * Mathematics
  * Statistics
  * Engineering
  * Medicine and health sciences
* Author's contributions
* Author's affiliations
* Funding body
* Keywords
* Publication date range
* Pre-Print indication

For an explanation of the Dublin Core Metadata Element Set please see the [Dublin Core website](http://dublincore.org/documents/dces/). Not all of these terms will be immediately clear to the average user, so they are not mandatory fields. This metadata in its current state is saved to Ethereum with a note that it has not been vetted. This block will be vetted by the community and once done so another block will be added stating that the previous block is now vetted. This forms an audit trail such that any tampering with the metadata will be clearly visible. 

Should any disagreement arise over the vetted metadata, it will be resolved through a community voting mechanism, explained later, the results of which will be again added as a new block to again add to the audit trail. Should part or all of the article be superseded, for example if an article is submitted that relies on a particular mathematical theory and the theory is proven to be incorrect, again a vote will be held and another block will be added to the chain noting the vote and the vote’s outcome with an amendment outlining the superseded information being added to the document itself and version information to show the document’s progression. The entire life cycle of the article will be clear for anyone to see. Vetting metadata will be incentivised through reputation, discussed later. 

## Acceptance into Aletheia
Before the articles become searchable and downloadable through the client, a community vote must be held and carried for the article to be accepted into Aletheia. This is to prevent things other than academic papers and related documents like data sets being uploaded and Aletheia being used as arbitrary external storage. A vote for the document to be accepted into Aletheia is launched at time of sbmission, a deliberately broad question that is a binary yes/no voute: "Do the documents represent academic research or not?". All users can see pending votes through their client, can download the documents associated with the vote to assess them and cast their vote. 

### Thresholds
A reputation threshold will be set and for a vote to pass a number of users that collectively have more than the required reputation must vote yes for the documents to be added to Alethiea. The reputation threshold for the yes vote will be higher than the no vote, deliberately biasing Alethia to make it harder for non academic content to enter Aletheia. Along with a reputation threshold a user number threshold will also need to be met, to ensure a minimum number of users vote on the inclusion of the documents. This ensures it's harder for users who have legitimately ammassed reputation to dictate what does or doesn't come into Aletheia. The final threshold will be a time threshold, votes will remain active for a set period of time, allowing enough time for both a yes or a no vote to accrue. If both yes and no votes reach their reputation and user number thresholds within the timeframe, the vote defaults to no and fails. All three thresholds, reputation, number of users and time elapsed  must be met for a vote to succeed. 

### Storage in Aletheia
If the vote passes the documents are accepted into Aletheia and will be returned in the client through search results. If the vote fails the documents will be deleted and the user notified by way of their client. Acceptance into Aletheia means a hash of the document and the document metadata are added to Ethereum and the Aletheia client will seed the document for download by other users. The hash can be checked against seeds to prevent tampering with documents and help demonstrate version control for papers. Due to current limitations with the amount of information able to be stored on a blockchain, the article itself is not stored on Ethereum. With advances in blockchain and computing it is hoped that a point can be reached where content could be stored on the blockchain itself, making the storage of articles more secure, at which point this new method would be adopted for Aletheia. 

### Voting reputation
Voting will be encentivised through reputation and further reputation will be rewarded for voting with the majority, regardless of if the vote passed or not or if the majority voted one way and the vote went the other way due to thresholds either being met or not. This means people will not be punished by the vote but they will be rewarded by following the crowd. The posed question, "Do the documents represent academic research or not?" is deliberately broad and the crowd in most instances should pick the correct outcome, therefore deliberately trying to skew votes will be punished. To prevent a malicious actor downloading a number of clients and attempting to vote, only users with a set reputation level can vote. That reputation level can be attained by the solving of a one time captcha and/or any other method of proving a user is a human as the technology around bots continues to develop.

## Peer review
To quote the paper [A multi-disciplinary perspective on emergent and future innovations in peer review](https://github.com/aletheia-foundation/aletheia-whitepaper/blob/master/Submitted-Ver-1.pdf) *"Success for any such development (of a new peer review system) relies on reaching a critical threshold of research community engagement with both the process and the platform, and therefore cannot be achieved without a significant change of incentives in research environments. A major part of this relies on research communities recognising that peer review is not a static or singular process, but a constantly evolving, and ideally improving, mechanism of quality assurance. This could greatly reduce friction to the cultural adoption of new models, and lead to a peer review process fit for a modern scholarly communication system."* It's acknowledged at the outset of building Aletheia that current academic publishing is culturally entrenched and will be hard to supplant. But to highlight the point above, *peer review is not a static or singular process, but a constantly evolving, and ideally improving, mechanism of quality assurance*, an open source platform that anyone can iterate upon is perhaps the best place for a peer review system. As such we do not expect the peer review process in Aletheia to remain static and it is therefore hard to quantify in this paper. What follows is a straightforward approach to peer review but will not definitively cover all Aletheia's final features.

Along with the vetting of metadata, the papers and data sets themselves must be vetted. A number of papers will already have undergone a peer review process or will elect to forego a peer review process, so peer review not a mandatory step for submission. The review, regardsless which chosen remains open indefinetly, and should a paper be uploaded without selecting a peer review and at a later stage the author/s wish to instigate a peer review they only need reupload the same document and select peer review at time of submission. The unreviewed paper will we retrivable through the client once submitted and approved, and effectively exists as a preprint at this stage. For many reasons a paper that selects peer review might never receive reviews and effectively the peer review opportunity remains open indefinetly. Should the paper later receive reviews as reviews are performed a hash of the review will be stored as a new block associated with the paper, meaning as and when reviews come in they can also be retrieved through the client. Papers naturally progress from preprint to peer reviewed and the paper's reputation score increases. If the submitter requests the article be peer reviewed they can choose to either have their work peer reviewed by particular users, a short list peer review, or they can open their article up to the entire reviewer pool, an entire pool peer review.

### Short List peer review
In short list review, the submitter will be able to search for users to review their work through their client, either by name or reputation score. The reviewer can see if they have been selected for short list review through their client and can either accept or decline the review. Only selected users can peer review the document.

### Entire Pool peer review
In an entire pool review any user can review the document. 

### Anonymity
Along with choosing the type of review the submitor will also have the option to have all names of authors hidden to reviewers if they so choose, and reviewers can also choose to hide their names. Papers and reviews can accrue reputation through citiations and downloads so the ability to remain anonymous is to mitigate bias based on gender/race/any other criterion. The paper and reviews are only anonymous until at least one round of peer review is completed.

### Rounds of peer review
The submitter is notified via their client when they receive reviews and to go through a round of review another version of the paper is uploaded that addresses the reviews received. The revised paper needs to go through two votes, the aceptance into Aletheia again, and another vote to confirm that the paper has adequetly addressed the reviewers comments. The submitter can write a short statement outlining how the revised paper addresses the reviews and if any reviews where ignored for any reason, such as lack of relevence. Once both these votes pass, the papers are connected in Aletheia as the next version of the initial paper, so people can track the evolution of the paper along with review comments. At this point one round of peer review is complete and the paper can continue to go through multiple rounds of peer review if reviews continue to be made. A round of peer review confers additional reputation on the paper.

## Cryptographic Control
One obvious vulnerability of Aletheia is that an attacker could upload a large number of articles in an attempt to overload and crash the network. A preventative mechanism must be implemented to prevent such an attack, and the mechanism that has been designed is called a cryptographic control. A control is a cryptographic resource issued to users that allow them to upload documents to the network. It is abundant enough that a normal user would not notice the control, but places an upper limit on how many documents can be uploaded per user in a twenty four hour period. The control will be tied to interaction with the network, downloading articles, participating in votes, peer review etc., along with a natural amount that accrues over time that will decay if not used. The decay prevents an attacker registering 'sleeper' accounts to attack the network at some point in future. The control for Aletheia has been dubbed Veris, derived from the word verisimilitude, meaning the appearance or semblance of truth, likelihood or probability. The amount of Veris a user has will determine how many documents they can be upload to Aletheia. 

## The content of Aletheia
Aletheia looks to provide a publishing platform for new academic work as well as form a repository for older work as well. Currently there are simpler models than Aletheia for making scientific articles available to people, such as hosting previously peer reviewed articles regardless of rights or legality and offering them to anyone through their browser, much like a search engine. In effect this is pirating scientific articles. [Sci-Hub](https://sci-hub.bz/) is an example. Aletheia recognises what Sci-Hub does as illegal as it violates the laws of many jurisdictions. Sci-Hub shares exactly the same motivations as Aletheia, making scientific knowledge available to everyone, but due to the fact that Sci-Hub and similar are illegal, publishers advance the argument that what they do is immoral simply because it is breaking the law. 

This is a powerful argument leveraged by publishers, despite the fact that the morality of copyright law, or the morality of profiting from denying people knowledge, profiting from perpetuating ignorance and all that does, is never put under scrutiny. Due to their illegal nature, Sci-Hub and others face challenges, like having their websites taken down periodically and having criminal and civil charges being brought against site administerators. At the time of writing, Alexandra Elbakyan, the creator of Sci-Hub, is wanted for extradition to the United States over charges of piracy [5](https://arstechnica.com/wp-content/uploads/2016/02/sci-hub.pdf). Aletheia has been designed to comply with anti-piracy laws to remove the morality argument from paywall journals against open access projects that aren't purely oulets to publish new work. Aletheia is an attempt to advance the argument against paywalls by creating an alternative to paywall journals that cannot be labelled illegal and immoral. 

### Creative Commons Licenses
Content that has not been published elsewhere that is submitted to Aletheia is offered under a _Creative Commons Attribution-ShareAlike 4.0 International licence_. By publishing through Aletheia you certify that you have permission to publish the submitted content or that the article is already in the public domain. Content that has been published elsewhere and therefore have rights attached to it can still be published through Aletheia as long as it is legal to do so. Again, the user certifies as part of the upload that they are not breaching existing rights by doing so. In the event where rights of work are ambiguous, such as orphan works,  Aletheia offers the work under _Creative Commons Attribution-ShareAlike 4.0 International licence_ until such time as the existing rights become clear and to continue hosting the article would breach these rights. Despite having an identity management system, discussed later, it is clear that under the above system it is possible for someone to submit work in violation of existing rights. 

### Removing non-academic content
While Aletheia has a number of checks and balances in place to weed out non-academic content being hosted through the client, a process needs to be in place to remove non-academic content. A vote to remove anything from Aletheia can be initiated, and the vote will follow the same process as the acceptance vote requiring three thresholds to be met, the question being "Is this non-academic content?". Again the vote will be weighted to the no response in an effort to mitigate attacks designed to remove legitimate content. If the vote passes a secondary check is initiated, users above a set reputation will be able to see through their client all requests to remove content through their client, and they can cast a deciding yes or no vote to remove or keep the contents. If at this second check the volunteer votes no, do not remove, the content remains in Aletheia. If they vote yes to remove the content is deleted from the client. The Ethereum reference will remain but the content itself will be deleted by the client and no longer shared by the network.

### Assessing takedown orders
In a perfect world a system could be built with checks such that it is impossible for someone to upload work to Aletheia illegally. Unfortunately this isn’t a perfect world and Aletheia needs to have a mechanism in place to remove content to avoid running afoul of legal action, or simply to remove content that doesn’t belong in Aletheia. Aletheia takes no responsibility for the actions of users, but will comply with takedown orders if found to be valid. On receiving a takedown order, a notification will be sent to the community through the Aletheia client. A vote will be held on the veracity of the takedown order to weed out vexatious orders. The vote will have the same three thresholds as acceptance of material into Aletheia and will be a similarly broad question "Is this takedown order enforceable by law?" In other words, does the party issuing the order hold the copyright to the claimed material and can they legally enforce the copyright? 

### Complying with takedown orders
If the yes vote wins, that take down is enforceable by law, a block will be added to Ethereum against the document preventing it from being shared. The document will be searchable by the client but will no longer download through the client. Instead, a document will be created by the Aletheia client and returned instead of the taken down paper. The notice will appear in search results for the original paper and will be downloadable. It will state something yet to be decided upon but in the spirit of the below:

_Article [insert name here] has been removed from Aletheia as the Aletheia community has received a takedown order from [insert name here] and found the order to be valid in its assertion that rights to the work have been violated._

_Scientific knowledge should be free for all though, and [insert name here] just deprived you of knowledge. What’s worse, [insert name here] did this legally. While Aletheia complies with the law, we don’t believe all laws are moral and some should be changed. Certain practices, like paywalls, stunt the growth of humanity simply to line the pockets of a select few. Did you know that [insert name here] posted a profit of [insert value here] in [insert year here]?_

_Laws that benefit very powerful vested interests will only be changed if pressure is bought to bare. Things you can do to help add to this pressure while remaining within the confines of the law:_

_Boycott paywalls of all kinds. Do not give them money, hit them where it hurts._

_Call or write to your local, state and federal government representatives expressing that [insert name here] is operating in a legal but unethical manner, and the changing of laws that allow these immoral practices to occur legally is an important issue to you and your vote come election time._

_Call or write to your local educational institutions and express that [insert name here] is operating in a legal but unethical manner, and the educational institution should join you in boycotting them. Suggest the educational institution source articles from open access journals and that this decision will be an important factor in deciding where your future tuition fees are invested._

_Pitch news stories to your local media representatives about the legal but immoral practices [insert name here] engage in._

_You may be able to find the article you are looking for on websites such as Sci-Hub, this is simply a fact, much like saying water is wet, and we do not encourage you to find your article there. Piracy is illegal._

A notice like this adequately expresses Aletheia’s position while not breaching the law. In an effort to prevent abuse of articles being removed from searches of the blockchain, such as if an attacker submitted a takedown order and then performed a majority attack on the subsequent vote, a vote can be held at any time to make the article downloadable again. If such a vote succeeds, another block would be added to the chain indicating the document is again searchable and downloadable.

At this stage it is not planned to introduce a method where the Aletheia blockchain could be forked, though it is recognised that unforeseen circumstances do arise. Should such a circumstance present itself, the question of forking would be put to the community as a vote.

## The incentivised seeding problem
An often cited issue with peer to peer technology is that few people share content, called seeding, purely for the benefit of the peer to peer network. Some networks will hamper people who don't seed at all, called leeches, that take from the network without giving back, to encourage users to seed. What often happens is that only popular content is seeded, that's the content that most people have so therefore that's the content that most people can in turn get. This marginalises less popular content that might have just as much intrinsic worth. There has been a great deal of study around the behavioural economics of peer to peer networks, but the approach Aletheia will take is a simple one. The health of the network is vital for Aletheia's success and all content must be shared equally, therefore Aletheia will enforce seeding. When a user downloads the client they are agreeing to be part of a peer to peer network that will seed academic papers and this will be made explicitly clear. The Aletheia client chooses what content will be seeded, ensuring there will always be content available to all users and all of the content will be equally accessible.

## Community
Aletheia is the embodiment of software that, while it exists as code, it does not function in any real sense removed from a human context. Aletheia’s skeleton may be code, but it’s heart is the human community. Anyone, by downloading the Aletheia client, can be a member of the community and through the client the user will be able to see all the activities they can take part in as a member of the community. 

Below is a basic guide to common community activities:

* Peer review documents – Users are able to see documents pending an Entire Pool peer review. They will be able to upload comments on the document that will go back to the submitter form part of the peer review. It submitters have an issue with any user being able to submit comments, they can either choose a Short List peer review, or no peer review at all
* Localise documents – translate documents into other languages and then upload the document which will be linked to the original, making Aletheia’s content more accessible to a wider audience
* Vet the metadata submitted with articles and datasets – improve the metadata quality to improve search results for papers through the Aletheia client
* Participate in votes – decisions are given over to the global community to vote on
* Audit and contribute to source code – by auditing and contributing to source code users can improve the security of Aletheia and continue its growth

The community exists past the Aletheia client and there may be other ways that the community interacts, such as through the Aletheia Foundation GitHub account, messaging servies, online forums and in person events. The community will be supported by the Aletheia Foundation, an entity created to support all aspects of Aletheia.

### What reputation will be scored on
The below is a basic list of the different things that will impact the reputation of a user:

* Submitting academic papers
* The quality of the paper
* Receiving citations to published papers
* The inclusion of data sets with papers so data sets are stored together with papers, easily locatable and not lost.
* The inclusion of data analysis methodology so research is easily reproducible
* Peer reviewing the papers of others
* The quality of the peer reviews
* Participating in community voting
* Performing code audits
* Contributing to the code base
* Localising academic papers
* Effort will be placed on finding ways to measure contributions from other community members, like though community organising and managing Aletheia's social media presence.

As a general rule of thumb, where an action could infer reputation, but also could be abused, such as performing the action numerous times with no benefit to the Aletheia ecosystem, purely for the purpose of appearing to have made a number of contributions and therefore accuring reputation, a check will be put in place. Before reputation can be incurred a vote is launched to assess the users contribution. This vote will have the same three thresholds as other votes. If the community vote passes, the person will be given reputation. If a number of failed votes are registered against the same user will incur a reputational penalty.

## Smart contracts
The mechanism that Aletheia handles votes and other decisions is through smart contracts. These smart contracts can be separated into two categories, Altheia's governance and management of the Aletheia Foundation. 

### Smart contracts for Aletheia's governance
* Acceptance into Aletheia – should the submitted documents be seeded by the client and should the metadata of the article and data set be searchable to return the documents in a search througn the client
* Confirmation that a document sufficiently included peer review notes in redrafting for resubmission – after a paper has been accepted into Aletheia, peer review notes have been submitted against the document, the document has been redrafted and resubmitted, a vote will be held to assess the peer review to ensure the redrafted paper adequately addresses all points raised.  If the users who performed the peer reviews are not receiving a wage from the Aletheia Foundation and their reviews where included into the redrafting of the paper and not removed for lack of relevence, a portion of any available funds will be routed to the users as payment if the vote is carried. It is understood that paying for peer review is contriversial, the Aletheia community has received for and against arguments from multiple people currently in academia. This is still under active discussion and will be closely monitored to ensure it doesn't detriment the peer review process  
* Confirmation that a code audit was legitimate – If the user is not receiving a wage from the Aletheia Foundation a portion of any available funds will be routed to the user as payment if the vote is carried
* Disagreement with acceptance into Aletheia – If something that is not an academic paper or data set makes it past the previous check a vote can be held to make it unsearchable by the client and removed from seeding, thereby removing it from circulation through Aletheia
* Vetting localisation – for a translated document be accepted onto Aletheia it will need to be approved  by someone who affirms they also speak this language
* Superseded/incorrect information – should an article be found to be partially or wholly factually incorrect, possibly due to an advancement in scientific understanding or any other means, a vote can be held to add a notation to the article stating as such
* Disagreement with a translation – should a user feel a translated document is of poor quality or completely incorrect, a vote can be launched to remove the document from Aletheia
* Acceptance of legitimacy of a takedown order – If Aletheia receives takedown orders, to ensure the order is legitimate the order will be made available to all users to look at. Assessment of the order is a simple series of questions, does Aletheia host the document the order pertains to and was the order issued by a party that legitimately holds the rights to that document.
* Disagreement with a previously accepted takedown order – if information comes to light that a takedown order was spurious, or if the party who issued the takedown order no longer holds the rights to the document, a vote can be held to make the document downloadable once again.
* Maintenance of the platform – users will have the ability to make bug reports through the client. These bugs will be viewable by all users. Users can claim bugs to work on and the user will see the bug report in their client. If the user is not receiving a wage from Aletheia a portion of any available funds will be routed to the user as payment on successful completion of the task once the community verifies the bug is indeed fixed. 
* Vote to verify bug was fixed – avoids bugs being simply marked as completed without being addressed, the community will verify code improvements to confirm the bug has been fixed.
* Development of the platform – as per maintenance of the platform, being feature requests rather than bug reports. 
* Vote to verify feature is now available – as per vote to verify bug fixed, being a feature request instead of a bug report.

### Smart contracts for managing the Aletheia Foundation
The Aletheia Foundation is an entity created to support the Aletheia community and the Aletheia code base. The long term vision is that the Foundation will be run as a DAO, just like Aletheia. Below is the preliminary structure of the contracts that create the Aletheia Foundation DAO.

* Hiring paid staff – users can fill out a form listing all their skills and previous work experience. The form will be accessible by other users and people can endorse one another if they have worked together previously. Based on the quality of the candidate worked out by possessed skills, length of previous work experience and endorsements rated by the reputation of the endorser, the contract will offer a paid position to the best candidate as and when roles become available or workload demands an increase in headcount.
* Allocation of internal work – any user who is a paid staff member of the Aletheia Foundation can submit a work request noting down the team the work is required from. the contract will keep a record of the workload for each team. The contract will allocate to members of the team with the best skills/most capacity. This workload allocation prevents the need of positions purely devoted to workload management of direct reports. This type of work is considered internal work, which needs a vote to sign off on completion from Aletheia Foundation employees but not the wider community.
* Other requirements of the platform – as per maintenance of the platform, but is a catch all contract for things like legal advice, graphic design etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
* Payroll – at a regular interval the contract will check how much work has been completed by each staff member, taking into account the difficulty of the work, and a portion of any available funds will be routed to the user as a regular wage along with an adjusted amount based on work signed off as completed by internal vote, again taking into account difficulty. 
* Budget – at a regular interval the contract will check how much money is available to the Aletheia entity. It will publish this information to Ethereum along with expenses accrued during that period such as wages of staff and payments to volunteers. At the end of each year the system will publish a projection for the coming year based off data from the last year/s.
* Catch-all contract – smart contracts are meant to facilitate work, not dictate it and sometimes computer code just doesn't cover a real world situation. Any staff member can call a vote on whatever the issue happens to be. If the vote passes its agreed work will be carried out contrary to/outside of the scope of existing contracts until that particular subject is addressed. There is potential for abuse in such a contract, however a large percentage of the workforce would need to collude to use this contract maliciously, being a high bar of difficulty. 

## Possible ideas

These consist of ideas that have been considered at one time or another during the development of Aletheia, or have been suggested by the Aletheia community






## Why blockchain?
Aletheia does not use all the properties of a blockchain, and the idea at it's heart is simply a database. The reason a blockchain is used is primarily for its resiliency. Blockchains are resistant to tampering, meaning the information stored in a blockchain is safer than in a traditional database. Blockchains are also decentralised, meaning that anyone with the open source Aletheia client, which can be downloaded from the official website or any other place that chooses to host it, is running part of the blockchain ledger which is constantly syncing with other users to form the whole ledger. Aletheia threatens very powerful, entrenched and wealthy interests and it is expected the network could come under pressure in one way, shape or form. By using a blockchain, to take Aletheia offline an attacker would have to remove clients from a critical mass of users, or simply take a critical mass of users off the Internet, users that reside all across the world in various legal jurisdictions. Such a task is inordinately more difficult than attacking a central server.

##
 Out of scope but desirable
This whitepaper only covers the basics of Aletheia such that a working prototype can be built. There are plenty of other functions Aletheia could have so people are encouraged to participate in discussion around this project. One future feature would be a mechanism to assist researchers analyse large numbers of journals to look at publishing trends and the like in an effort to improve the publishing ecosystem. Another would be the functionality to mass download every indexed and seeded document quickly and efficiently without having to search every individual article and dataset. This final feature forms a fail-safe to Aletheia's library and allows anyone to host the documents on their own service.

## Outlook on blockchain and science
In the course of completing this whitepaper differing opinions in the scientific community on blockchain have become apparent, particularly around the peer review process. Some camps espouse a human actioned/blockchain facilitated peer review process as outlined in this paper. Others say that humans should be eliminated from the peer review process and through semantics, making human written text machine readable, a computer should check the facts in a scientific article against other submitted articles, thereby performing a ‘machine review’. Still others say that humans should be removed even from the collection of scientific fact, with large and complex Internet of Things networks generating data that can be fed into a universal 'blockchain of absolute truth'. Any misunderstanding or misrepresentation of these latter two positions is entirely unintended. This paper outlines the first of these three schools of thought, believing that perfection should not become the enemy of good. If Aletheia is successful it will certainly bring projects of the other two camps closer to realisation, so it is hoped that everyone with an interest in blockchain and/or science can support a project like Aletheia.
