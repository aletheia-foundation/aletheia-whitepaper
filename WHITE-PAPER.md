![alt tag](https://cloud.githubusercontent.com/assets/24201238/24583976/ced4c43e-179f-11e7-9c40-c0988c346f55.png)

_**Publish research for free, access research for free.**_

# Aletheia: blockchain for scientific knowledge with a community management framework

### By Kade Morton and the Aletheia Community
### kademorton@protonmail.com
### contact@aletheia-foundation.io

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
- [Revenue model](#revenue-model)
- [Smart contracts](#smart-contracts)
  - [Smart contracts for Aletheia's governance](#smart-contracts-for-Aletheias-governance)
  - [Smart contracts for managing the Aletheia Foundation](#smart-contracts-for-managing-the-aletheia-foundation)
- [Outlook on blockchain and scientific communication](#outlook-on-blockchain-and-scientific-communication)

## Introduction
Aletheia is a decentralised, open source, open access scientific journal. It is a free client that runs on Windows, Mac and Linux, that allows the user to upload academic papers and datasets, as well as search for academic papers and datasets. The Aletheia client enforces sharing of documents with other uses, forming a peer to peer network. Hashes of documents, metadata for documents, reputation accrued by documents, actions of users and community decisions are stored on the Ethereum blockchain to allow version control of documents, track reputation and provide redundancy and resiliency to the information in the network. The community administers Aletheia through a community management framework of smart contracts, making Aletheia a decentralised autonomous organisation ([DAO](https://en.wikipedia.org/wiki/The_DAO_(organization))). It encourages peer review and creates its own reputation ecosystem to provide an alternative to the current prestige system that dominates academic publishing with detrimental consequences. Information is stored on the Ethereum blockchain to allow version control of documents and provide redundancy and resiliency to the information in the network.

## Why is Aletheia important?
_Information is power. But like all power, there are those who want to keep it for themselves. The world’s entire scientific and cultural heritage, published over centuries in books and journals is increasingly being digitised and locked up by a handful of private corporations. Want to read the papers featuring the most famous results of the sciences? You’ll need to send enormous amounts to publishers like Reed Elsevier. - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_

It was estimated in 2010 that roughly 50 million scientific papers had been published to date [1](http://www.ruor.uottawa.ca/bitstream/10393/19577/2/Jinha_Arif_2010_Article_50_million.pdf). However, almost 90% of research articles cannot be accessed freely either through the publisher's website or from other websites[2](https://bmcmedicine.biomedcentral.com/articles/10.1186/1741-7015-10-124), [3](http://www.openaccesspublishing.org/apc8/Personal%20VersionGreenOa.pdf). That is to say, a large percentage of humanity’s collective knowledge is only accessible by those with financial means. To put the term ‘financial means’ in context, in 2012 the Harvard Library published a letter stating that it was paying close to $3,750,000 USD a year in journal subscriptions and that this state of affairs was financially untenable, meaning the library planned on cutting back the number of journals on offer to students [4](http://gantercourses.net/wp-content/uploads/2013/11/Faculty-Advisory-Council-Memorandum-on-Journal-Pricing-§-THE-HARVARD-LIBRARY.pdf). If Ivy League institutions cannot afford scientific journals, what chance does an institution in a developing nation have? What chance does your average individual have? Cutting off every person who does not have the financial means to pay exorbitant fees for scientific knowledge is fundamentally wrong. Aletheia is a proposal to go some way to correcting this error while also fostering a movement against [paywall](https://en.wikipedia.org/wiki/Paywall) journals.

But open access already exists. Open access journals are scientific journals that do not restrict access to their content. While Aletheia adheres to the principles of open access it is different from existing open access journals in a number of ways. Most journals today are offered online and papers are accessed through the journal's website that allow searching of a centralised database in the background. Aletheia is a downloadable peer to peer client, which prevents centralisation through control of the website or control of the back end database. The information stored in the Aletheia network is spread across all users running the client and the Ethereum blockchain, again preventing centralisation. Due to its decentralised nature along with providing an alternative to the current prestige system and allowing the community to directly administer the platform as a DAO, Aletheia contributes something currently lacking from the current open access ecosystem.

### A blockchain journal
A blockchain is a distributed ledger that through cryptographic means can only be added to, not subsequently changed. For a thorough technical explanation of a blockchain, please see Satoshi Nakamoto’s original paper, [Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf). Aletheia utilises a blockchain to achieve a distributed and tamper proof database of information, storing document metadata, vote topics, vote results and user reputation. Aletheia is a redundant, resilient and decentralised application that is not controlled by any one party; it is administered by the community. This makes the information stored in Aletheia hard to assail, cryptographically protected, redundantly stored, verified by everyone and controlled by no one, locking it into the commons.

Currently, Aletheia is utilising the Ethereum blockchain for pragmatic reasons such as Ethereum’s smart contract functionality, the maturity of the development ecosystem, and Ethereum’s development roadmap. Similarly, if a different blockchain or an entirely different technology presented itself that better aligned with Aletheia’s goals, Aletheia would shift to use this new offering. Until one presents itself the Ethereum blockchain is being used.

### The problems with the prestige system
The often cited reason for the fact that existing open access journals do not grow to rival their paywall counterparts is due to prestige. For academics it is often more beneficial for their careers to publish in a large paywall journal due to the prestige they obtain [5](https://www.theguardian.com/science/2013/dec/09/nobel-winner-boycott-science-journals). Publishing in a prestigious paywall journal will positively influence your research career and possibility for grant funding, allowing you to conduct more research. Journal publishers know all too well that this system of incentives binds researchers to them, as people risk their careers, their income, and future grants if they do not publish in prestigious journals. Since these journals effectively have a monopoly on academic communication, they can largely do what they want. This led to the introduction of paywalls to academic publishing in the first place. Publishing in top tier journals attracts prestige due to the stringent editorial and peer review process, but evidence show retraction rates for peer reviewed work is rising [6](https://theconversation.com/what-lesson-do-rising-retraction-rates-hold-for-peer-review-28823), raising doubts about the substance of this prestige.

There are a number of negative consequences to the prestige system. Human knowledge is concentrated behind paywalls, harming the entire human race by preventing access to scientific knowledge, robbing us of scientific advancements. The power such journals wield is perpetuated by this concentration of knowledge. Academics are incentivised to bury research that has negative findings or just is not deemed "ground breaking", meaning money and time is wasted, along with the fact that humanity's collective knowledge pool is not added to. It produces bad science. The prestige system is a complex socio-economic system perpetuated by journals and researchers themselves by rewarding publication in prestigious journals and punishing a lack thereof. It is self-reinforcing and is very difficult to remove.

### A new reputation ecosystem
Aletheia allows reputation to be accrued by users and uploaded academic papers. Aletheia creates a reputation ecosystem that can be drilled down into the show the number of papers uploaded and their quality, number of citations the paper receives, number of reviews performed and their quality, number of decisions participated in and what decision was made. This information is a comprehensive record of a user's contribution to science, which is more rigorous and scientific than the prestige model of publishing in top tier journals. While initially encouraging submissions to Aletheia, it is hoped this transparent and quantifiable reputation system could come to be seen as a preferred alternative to the prestige system that constricts academia today. Because anyone can participate in Aletheia, this reputation system also offers a pathway for others without specific scientific experience or affiliation to an academic center to engage with academia and have their skills valued and recognised, opening academia and making scientific research more inclusive. This might be anathema for a large portion of academia, but openness and inclusivity are founding principles of open access. Walls and exclusion, while forever tempting, rarely ever gave humanity anything of value.

### A peer to peer journal
Peer to peer file sharing is a method of file sharing where peer to peer software is run on a computer, making that computer a part of a file sharing network. This allows the computer to query other peers also running the same software, and once it has found a peer with the desired file it begins to download a copy [7](https://en.wikipedia.org/wiki/Peer-to-peer). To facilitate the main function of Aletheia, the obtaining of scientific journals, the Aletheia client is a peer to peer file sharing client that allows the submission of academic papers and datasets for sharing through the client. Currently datasets are hard to obtain, often stored in online repositories separate from the papers themselves, if accessible at all. One of Aletheia’s goals is to make data easier to obtain in order to assist with checking the veracity of articles. By downloading and running the Aletheia client you are becoming a peer in the distributed network.

### A community journal
Smart contracts are computer programs designed to execute a predefined action based on inputs. They are typically imagined as legal contracts written as programs [8](https://en.wikipedia.org/wiki/Smart_contract), and they can be used to create a community management framework. Smart contracts can be written to either perform one or more of a predefined set actions, or simply to perform or not perform a predefined action based on number of votes received during a specified time frame, giving Aletheia a means of community decision making. In this way, the community directly administers Aletheia as a DAO through direct democracy, meaning anyone can take part in this open community and that Aletheia has no [key person risk](https://en.wikipedia.org/wiki/Bus_factor). Every smart contract, along with every time it is invoked and the outcome of the execution of the smart contract is stored on Ethereum to provide a fully transparent audit trail. Aletheia is also open source, allowing people to view its source, verify its security and contribute to it if desired. Because everyone has access to the code, the code can be hosted on any website for download, making Aletheia hard to censor.

## Submitting documents to Aletheia
Once a user has installed the Aletheia client on their computer, they can upload academic papers and associated datasets to be shared with the Aletheia community. The user need not be one of the authors. Any paper, so long as it is not under copyright, can be uploaded. To facilitate the search function and allow the client to return papers on particular topics or from particular disciplines, metatdata is also required. This can be entered at time of submission to Aletheia, or it can be added at a later date by the community.

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

For an explanation of the Dublin Core Metadata Element Set please see the [Dublin Core website](http://dublincore.org/documents/dces/). Not all of these terms will be immediately clear to the average user, so they are not mandatory fields. The metadata are initially saved to Ethereum with a note that they have not been vetted. This notation, or block, will be vetted by the community and once done another block will be added stating that the previous block is now vetted. This forms an audit trail such that any tampering with the metadata will be clearly visible.

Should any disagreement arise over the vetted metadata, it will be resolved through a community voting mechanism, the results of which will be again added as a new block to again add to the audit trail. Should part or all of the article be superseded, a vote will be held and another block will be added to Ethereum noting the vote and the vote’s outcome with an amendment outlining the superseded information being added to the document itself and version information to show the document’s progression. The entire life cycle of the article will be clear for anyone to see. Vetting metadata will be incentivised through reputation.

## Acceptance into Aletheia
Before the articles become searchable and downloadable through the client, a community vote must be carried out for the article to be accepted into Aletheia. This is to prevent things other than academic papers and related documents like datasets being uploaded to Aletheia. A vote for the document to be accepted into Aletheia is launched at the time of submission, a deliberately general question that is a binary yes/no vote: "Do the documents represent academic research or not?". All users can see pending votes on documents through their client, can download the documents associated with the vote to assess them and cast their own vote.

### Thresholds
Three thresholds are required to be met for a vote to be carried. First, a reputation threshold will be set and for a vote to pass a number of users that collectively have more than the required reputation must vote yes for the documents to be added to Aletheia. The reputation threshold for the yes vote will be higher than the no vote, deliberately biasing Aletheia to make it harder for non academic content to enter Aletheia. Second, a user number threshold will also need to be met, to ensure a minimum number of users vote on the inclusion of any documents. This ensures it's harder for users who have legitimately amassed reputation to dictate what does or doesn't come into Aletheia. The third and final threshold will be a time, votes will remain active for a set duration allowing enough time for both a yes or a no vote to accrue. If both yes and no votes reach their reputation and user number thresholds within the time frame, the vote defaults to no and fails. All three thresholds, reputation, number of users and time elapsed must be met for a vote to succeed.

### Storage in Aletheia
If a vote passes the respective documents are accepted into Aletheia and will be returned in the client through search results. If the vote fails the documents will be deleted and the user notified by way of their client. Acceptance into Aletheia means a hash of the document and the document metadata are added to Ethereum and the Aletheia client will seed the document for download by other users. The hash can be checked against seeds to prevent tampering with documents and help demonstrate version control for papers. Due to current limitations with the amount of information able to be stored on a blockchain, the article itself is not stored on Ethereum. With advances in blockchain and computing it is hoped that a point can be reached where content could be stored on the blockchain itself, making the storage of articles more secure, at which point this new method would be adopted for Aletheia.

### Voting reputation
Voting will be incentivised through reputation and further reputation will be rewarded for voting with the majority, regardless of if the vote passed or failed or if the majority voted one way and the vote went the other way due to thresholds either being met or not. This means people will not be punished by the vote but they will be rewarded by following the crowd. The posed question, "Do the documents represent academic research or not?" is deliberately broad and the crowd in most instances should pick the correct outcome, therefore deliberately trying to skew votes will be punished. To prevent a malicious actor downloading a number of clients and attempting to vote, only users with a set reputation level can vote. That reputation level can be attained by the solving of a one time captcha and/or any other method of proving a user is a human as the technology around bots continues to develop.

## Peer review
To quote the paper [A multi-disciplinary perspective on emergent and future innovations in peer review](https://github.com/aletheia-foundation/aletheia-whitepaper/blob/master/Submitted-Ver-1.pdf) *"Success for any such development (of a new peer review system) relies on reaching a critical threshold of research community engagement with both the process and the platform, and therefore cannot be achieved without a significant change of incentives in research environments. A major part of this relies on research communities recognising that peer review is not a static or singular process, but a constantly evolving, and ideally improving, mechanism of quality assurance. This could greatly reduce friction to the cultural adoption of new models, and lead to a peer review process fit for a modern scholarly communication system."*

It's acknowledged at the outset of building Aletheia that current academic publishing processes are culturally entrenched and will be hard to supplant. But to highlight the point above, *peer review is not a static or singular process, but a constantly evolving, and ideally improving, mechanism of quality assurance*, an open source platform that anyone can iterate upon is perhaps the best place for a peer review system. As such we do not expect the peer review process in Aletheia to remain static and it is therefore hard to quantify in this paper. What follows is a straightforward approach to peer review but will not definitively cover all Aletheia's final features.

Along with the vetting of metadata, the papers and datasets themselves must be vetted. A number of papers will already have undergone a peer review process or will elect to forego a peer review process, so peer review not a mandatory step for submission. The review, regardless which chosen, remains open indefinitely, and should a paper be uploaded without selecting a peer review option but at a later stage the author/s desire one they only need re-upload the same document and select peer review at time of submission. The unreviewed paper will we retrievable through the client once submitted and approved, effectively existing as a preprint at this stage.

Should the paper receive reviews, as they are performed a hash of the review will be stored as a new block associated with the paper, meaning as and when reviews come in they can also be retrieved through the client. Papers can be re-uploaded once redrafted to incorporate the review notes, again being appended as another document associated with the initial preprint, so papers can progress from preprint to peer reviewed with the paper's reputation score increasing at each step. If the submitter requests the article be peer reviewed they can choose to either have their work peer reviewed by particular users, a short list peer review, or they can open their article up to the entire reviewer pool, an entire pool peer review.

### Short List peer review
In short list review, the submitter will be able to search for users to review their work through their client, either by name or reputation score. The reviewer can see if they have been selected for short list review through their client and can either accept or decline the review. Only selected users can peer review the document. This gives academics the ability to ensure only people inside their field, even inside a specific specialisation in a set field, should they so desire.

### Entire Pool peer review
In an entire pool review any user can review the document. This option acknowledges that people from all walks of life have valued experience and skills and allows people outside a set field to review papers. For example, a data scientist with twenty or more years experience in industry might not be able to comment authoritatively on a geology paper, but they might have valued insights related to the datasets and the way the paper interprets their contents. While an unorthodox approach it's hoped this peer review option will demonstrate it's worth and make academia more accessible to everyone.

### Anonymity
Along with choosing the type of review the submitter will also have the option to have all names of authors hidden to reviewers if they so choose, and reviewers can also choose to hide their names. Papers and reviews can accrue reputation through citations and downloads so the ability to remain anonymous is to mitigate bias based on gender/race/any other criterion. The paper and reviews are only anonymous until at least one round of peer review is completed. Anonymity and preprints is an issue, as under this model authors cannot be seen any anyone until one round of peer review. The alternative is to have the names of authors show when the paper is to be downloaded for general reading but hidden if downloading for peer review. This would effectively be an honour system as there would be no way to tell definitively which reason a user was downloading a paper for and would rely on the user self reporting. Even if it could be determined, a reviewer could simply ask another user to download the paper for reading and discover the authors this way. Currently Aletheia is adopting anonymity until peer review is over to mitigate peer review bias as much as possible.

### Rounds of peer review
The submitter is notified via their client when they receive reviews and to go through a round of review another version of the paper is uploaded that addresses the reviews received. The revised paper needs to go through a vote to confirm that the paper has adequately addressed the reviewers comments. The submitter can write a short statement outlining how the revised paper addresses the reviews and if any reviews where ignored for any reason, such as lack of relevance, which is possible in Entire Pool peer review. Once this vote is carried, the paper's preprint and now peer reviewed versions are connected in Aletheia as the next version of the initial paper, so people can track the evolution of the paper along with review comments. At this point one round of peer review is complete and the paper can continue to go through multiple rounds of peer review if reviews continue to be made. Each round of peer review confers additional reputation on the paper.

## Cryptographic Control
One obvious vulnerability of Aletheia is that an attacker could upload a large number of articles in an attempt to overload the network. The mechanism that has been designed to mitigate such an attack is called a cryptographic control. A control is a cryptographic resource issued to users that allow them to upload documents to the network. It is abundant enough that a normal user would not notice the control, but places an upper limit on how many documents can be uploaded per user in a twenty four hour period. The control will be tied to interaction with the network, downloading articles, participating in votes, peer review etc., along with a natural amount that accrues over time that will decay if not used. The decay prevents an attacker registering 'sleeper' accounts to attack the network at some point in future. The control for Aletheia has been dubbed Veris, derived from the word verisimilitude, meaning the appearance or semblance of truth, likelihood or probability. The amount of Veris a user has will determine how many documents they can be upload to Aletheia.

## The content of Aletheia
_Meanwhile, those who have been locked out are not standing idly by. You have been sneaking through holes and climbing over fences, liberating the information locked up by the publishers and sharing them with your friends. But all of this action goes on in the dark, hidden underground. It’s called stealing or piracy, as if sharing a wealth of knowledge were the moral equivalent of plundering a ship and murdering its crew. But sharing isn’t immoral – it’s a moral imperative. - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_

Aletheia looks to provide a publishing platform for new academic work as well as form a repository for older work. Currently there are simpler models than Aletheia for making scientific articles available to people, such as hosting previously peer reviewed articles regardless of rights or legality and offering them to anyone through their browser, much like a search engine. In effect this is pirating scientific articles. [Sci-Hub](https://sci-hub.bz/) is an example. Aletheia recognises what Sci-Hub does as illegal as it violates the laws of many jurisdictions. However, Sci-Hub shares exactly the same motivations as Aletheia, making scientific knowledge available to everyone, but due to the fact that Sci-Hub and similar projects are illegal, publishers advance the argument that what they do is immoral simply because it is breaking the law.

This is a powerful argument leveraged by publishers. The morality of copyright law, or the morality of profiting from denying people knowledge, profiting from perpetuating ignorance and the damage it does, is never put under scrutiny. Due to their illegal nature, Sci-Hub and others also face operational challenges, like having their websites taken down periodically and having criminal and civil charges being brought against site administrators. At the time of writing, Alexandra Elbakyan, the creator of Sci-Hub, is wanted for extradition to the United States over charges of piracy [9](https://arstechnica.com/wp-content/uploads/2016/02/sci-hub.pdf). Aletheia has been designed to comply with anti-piracy laws to remove the morality argument from paywall journals against open access projects that aren't purely outlets to publish new work. Aletheia is an attempt to advance the argument against paywalls by creating an alternative to paywall journals that cannot be labelled illegal and immoral.

Sci-Hub already exists, Aletheia is not trying to be Sci-Hub. Aletheia is trying to be a missing piece in the open access ecosystem that sits beside Sci-Hub and traditional
 open access publishers.

### Creative Commons Licenses
_Forcing academics to pay money to read the work of their colleagues? Scanning entire libraries but only allowing the folks at Google to read them? Providing scientific articles to those at elite universities in the First World, but not to children in the Global South? It’s outrageous and unacceptable. - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_

Content that has not been published elsewhere that is submitted to Aletheia is offered under a _Creative Commons Attribution-ShareAlike 4.0 International licence_. By publishing through Aletheia you certify that you have permission to publish the submitted content or that the article is already in the public domain. Content that has been published elsewhere and therefore has rights attached to it can still be published through Aletheia as long as it is legal to do so, the content will be offered under those rights. Again, the user certifies as part of the upload that they are not breaching existing rights by doing so. In the event where rights of work are ambiguous, such as orphan works,  Aletheia offers the work under _Creative Commons Attribution-ShareAlike 4.0 International licence_ until such time as the existing rights become clear and to continue hosting the article would breach these rights. It is clear that under the above system it is possible for someone to submit work in violation of existing rights, so Aletheia needs functionality to remove such content.

### Removing non-academic content
A vote to remove anything from Aletheia can be initiated, and the vote will follow the same process as the acceptance vote requiring three thresholds to be met, the question being "Is this non-academic content?". Again the vote will be weighted to the no response in an effort to mitigate attacks designed to remove legitimate content. If the vote passes a secondary check is initiated, users above a set reputation will be able to see through their client all requests to remove content through their client, and they can cast a deciding yes or no vote to remove or keep the contents. If at this second check the volunteer votes no, do not remove, the content remains in Aletheia. If they vote yes to remove the content is deleted from the client. The Ethereum reference will remain but the content itself will be deleted by the client and no longer shared by the network.

### Assessing takedown orders
In a perfect world a system could be built with checks such that it is impossible for someone to upload work to Aletheia illegally. Unfortunately this isn’t a perfect world and Aletheia needs to have a mechanism in place to remove content to avoid running afoul of legal action, or simply to remove content that doesn’t belong in Aletheia. Aletheia takes no responsibility for the actions of users, but will comply with takedown orders if found to be valid. On receiving a takedown order, a notification will be sent to the community through the Aletheia client. A vote will be held on the veracity of the takedown order to weed out vexatious orders. The vote will have the same three thresholds as acceptance of material into Aletheia and will be a similarly broad question "Is this takedown order enforceable by law?" In other words, does the party issuing the order hold the copyright to the claimed material and can they legally enforce the copyright?

### Complying with takedown orders
_“I agree,” many say, “but what can we do? The companies hold the copyrights, they make enormous amounts of money by charging access, and it’s perfectly legal – there’s nothing we can do to stop them.” But there is something we can, something that’s already being done: we can fight back. - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_

If the yes vote wins, that the take down is enforceable by law, a block will be added to Ethereum against the document preventing it from being shared. The document will be searchable by the client but will no longer download through the client. Instead, a document will be created by the Aletheia client and returned instead of the taken down paper. The notice will appear in search results for the original paper and will be downloadable. It will state something yet to be decided upon but in the spirit of the below:

_Article [insert name here] has been removed from Aletheia as the Aletheia community has received a takedown order from [insert name here] and found the order to be valid in its assertion that rights to the work have been violated._

_Scientific knowledge should be free for all though, and [insert name here] just deprived you of knowledge. What’s worse, [insert name here] did this legally. While Aletheia complies with the law, we don’t believe all laws are moral and some should be changed. Certain practices, like paywalls, stunt the growth of humanity simply to line the pockets of a select few. Did you know that [insert name here] posted a profit of [insert value here] in [insert year here]?_

_Laws that benefit very powerful vested interests will only be changed if pressure is bought to bare. Things you can do to help add to this pressure while remaining within the confines of the law:_

_Boycott paywalls of all kinds. Do not give them money, don't publish through them. Hit paywall publishers where it hurts._

_Call or write to your local, state and federal government representatives expressing that [insert name here] is operating in a legal but unethical manner, and the changing of laws that allow these immoral practices to occur legally is an important issue to you and your vote come election time._

_Call or write to your local educational institutions and express that [insert name here] is operating in a legal but unethical manner, and the educational institution should join you in boycotting them. Suggest the educational institution source articles from open access journals and that this decision will be an important factor in deciding where your future tuition fees are invested._

_Pitch news stories to your local media representatives about the legal but immoral practices [insert name here] engage in._

_You may be able to find the article you are looking for on websites such as Sci-Hub, this is simply a fact, much like saying water is wet, and we do not encourage you to find your article there. Piracy is illegal._

A notice like this adequately expresses Aletheia’s position while not breaching the law. In an effort to prevent abuse of legitimate papers not under copyright being removed from Aletheia a vote can be held at any time to make the article downloadable again. If such a vote succeeds, another block would be added to Ethereum indicating the document is again searchable and downloadable.

## The incentivised seeding problem
An often cited issue with peer to peer technology is that few people share content, called seeding, purely for the benefit of the peer to peer network. Some networks will hamper people who don't seed at all, called leeches, that take from the network without giving back, to encourage users to seed. What often happens is that only popular content is seeded, the content that most people have is therefore the content that most people can access. This marginalises less popular content that might have just as much intrinsic worth. There has been a great deal of study around the behavioural economics of peer to peer networks, but the approach Aletheia will take is a simple one. The health of the network is vital for Aletheia's success and all content must be shared equally, therefore Aletheia will enforce seeding. When a user downloads the client they are agreeing to be part of a peer to peer network that will seed academic papers and this will be made explicitly clear. The Aletheia client chooses what content will be seeded, ensuring there will always be content available to all users, that all content will be redundantly stored and all the content will be equally accessible.

## Community
_It’s time to come into the light and, in the grand tradition of civil disobedience, declare our opposition to this private theft of public culture. - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_

Aletheia is the embodiment of software that, while it exists as code, has no function removed from a human context. Aletheia’s skeleton may be code, but it’s heart is the human community. Anyone, by downloading the Aletheia client, can be a member of the community and through the client the user will be able to see all the activities they can take part in as a member of the community.

Below is a basic outline of common community activities:

* Peer review documents – Users are able to see documents pending an Entire Pool peer review. They will be able to upload comments on the document that will go back to the submitter form part of the peer review. It submitters have an issue with any user being able to submit comments, they can either choose a Short List peer review, or no peer review at all
* Localise documents – translate documents into other languages and then upload the document which will be linked to the original, making Aletheia’s content more accessible to a wider audience
* Vet the metadata submitted with articles and datasets – improve the metadata quality to improve search results for papers through the Aletheia client
* Participate in votes – decisions are given over to the global community to vote on
* Audit and contribute to source code – by auditing and contributing to source code users can improve the security of Aletheia and continue its growth

The community exists past the Aletheia client and there may be other ways that the community interacts, such as through the Aletheia Foundation GitHub account, messaging
 services, online forums and in person events. The community will be supported by the Aletheia Foundation, an entity created to support all aspects of Aletheia.

### What reputation will be scored on
The below is a basic list of the different things that will impact the reputation of a user:

* Submitting academic papers
* The quality of the paper
* Receiving citations to published papers
* The inclusion of datasets with papers
* The inclusion of data analysis methodology
* Peer reviewing the papers of others
* The quality of the peer reviews
* Participating in community voting
* Performing code audits
* Contributing to the code base
* Localising academic papers
* Effort will be placed on finding ways to measure contributions from other community members, like though community organising and managing Aletheia's social media presence.

As a general rule of thumb, where an action could infer reputation, but also could be abused, such as performing the action numerous times with no benefit to the Aletheia ecosystem purely for the purpose of appearing to have made a number of contributions and therefore accruing reputation, a check will be put in place. Before reputation can be incurred a vote is launched to assess the users contribution. This vote will have the same three thresholds as other votes. If the community vote passes, the user will be given reputation. If a number of failed votes are registered against the same user that user will incur a reputation penalty.

## Revenue model
The Aletheia application will have a cryptocurrency miner built into it. This will be explicit and it will be explained to users that by downloading the Aletheia application, you are running a cryptocurrency miner. All cryptocurrency mined will go to the Aletheia Foundation and everyone will be able to check the amount of cryptocurrency received by the Foundation. Funds will cover [Ethereum gas costs](https://ethereum.gitbooks.io/frontier-guide/content/costs.html), a tax for using Ethereum, along with paying the wages of any Foundation full time staff. Wages of staff will be publicly available. Remaining funds will be given to members of the community that help maintain Aletheia through fixing bugs and other tasks, and records of community payments will also be publicly available.

## Smart contracts
The mechanism that Aletheia handles votes and other decisions is through smart contracts. These smart contracts can be separated into two categories, Aletheia's governance and management of the Aletheia Foundation.

### Smart contracts for Aletheia's governance
* Acceptance into Aletheia – should the submitted documents be seeded by the client and returned in search results
* Confirmation that a document sufficiently included peer review notes in redrafting for resubmission – after a paper has been accepted into Aletheia, peer review notes have been submitted against the document, the document has been redrafted and resubmitted, a vote will be held to assess the peer review to ensure the redrafted paper adequately addresses all points raised.  If the user's review was included in the redrafting of the paper, a portion of any available funds will be routed to the user as payment if the vote is carried. It is understood that paying for peer review is controversial, the Aletheia community has received arguments for and against from multiple people currently in academia. This is still under active discussion and will be closely monitored to ensure it doesn't detriment the peer review process  
* Confirmation that a code audit was legitimate – a portion of any available funds will be routed to the user as payment if the vote is carried
* Disagreement with acceptance into Aletheia – If something that is not an academic paper or dataset makes it past the previous checks a vote can be held to make it unsearchable by the client and removed from seeding, thereby removing it from circulation through Aletheia
* Vetting localisation – for a translated document to be accepted onto Aletheia it will need to be approved by someone who affirms they also speak this language. A portion of any available funds will be routed to the translator as payment if the vote is carried
* Disagreement with localisation – should a user feel a translated document is of poor quality or completely incorrect, a vote can be launched to remove the document from Aletheia
* Superseded/incorrect information – should an article be found to be partially or wholly factually incorrect, a vote can be held to add a notation to the article stating as such
* Acceptance of legitimacy of a takedown order – If Aletheia receives takedown orders, to ensure the order is legitimate the order will be made available to all users to look at. Assessment of the order is a simple series of questions, does Aletheia host the document the order pertains to and was the order issued by a party that legitimately holds the rights to that document.
* Disagreement with a previously accepted takedown order – if information comes to light that a takedown order was spurious, or if the party who issued the takedown order no longer holds the rights to the document, a vote can be held to make the document downloadable once again
* Maintenance of the platform – users will have the ability to make bug reports through the client. These bugs will be viewable by all users. Users can claim bugs to work on and the user will see the bug report in their client.
* Vote to verify bug was fixed – avoids bugs being simply marked as completed without being addressed, the community will verify code improvements to confirm the bug has been fixed. A portion of any available funds will be routed to the user who fixed the bug as payment on successful completion of the task once the community verifies the bug is indeed fixed
* Development of the platform – as per maintenance of the platform, being feature requests rather than bug reports
* Vote to verify feature is now available – as per vote to verify bug fixed, being a feature request instead of a bug report

### Smart contracts for managing the Aletheia Foundation
The Aletheia Foundation is an entity created to support the Aletheia community and the Aletheia code base. The long term vision is that the Foundation will be run as a DAO, just like Aletheia. Below is the preliminary structure of the contracts that create the Aletheia Foundation DAO.

* Hiring paid staff – users can fill out a form listing all their skills and previous work experience. The form will be accessible by other users and people can endorse one another if they have worked together previously. Based on the quality of the candidate worked out by possessed skills, length of previous work experience and endorsements rated by the reputation of the endorser, a paid position will offered to the best candidate as and when roles become available or workload demands an increase in headcount
* Allocation of internal work – any user who is a paid staff member of the Aletheia Foundation can submit a work request noting down the team the work is required from. the contract will keep a record of the workload for each team. The contract will allocate to members of the team with the best skills/most capacity. This workload allocation prevents the need of positions purely devoted to workload management of direct reports. This type of work is considered internal work, which needs a vote to sign off on completion from Aletheia Foundation employees but not the wider community
* Other requirements of the platform – as per maintenance of the platform, but is a catch all contract for things like legal advice, graphic design etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  

* Payroll – at a regular interval the contract will check how much work has been completed by each staff member, taking into account the difficulty of the work, and a portion of any available funds will be routed to the user as a regular wage.
* Budget – at a regular interval the contract will check how much money is available to the Aletheia entity. It will publish this information to Ethereum along with expenses accrued during that period such as wages of staff and payments to volunteers. At the end of each year the system will publish a projection for the coming year based off data from the last year/s.
* Catch-all contract – smart contracts are meant to facilitate work, not dictate it and sometimes computer code just doesn't cover a real world situation. Any staff member can call a vote on whatever the issue happens to be. If the vote passes its agreed work will be carried out contrary to/outside of the scope of existing contracts until that particular subject is addressed. There is potential for abuse in such a contract, however a large percentage of the workforce would need to collude to use this contract maliciously, being a high bar of difficulty.

## Outlook on blockchain and scientific communication
In the course of completing this white paper differing opinions in the scientific community on blockchain have become apparent, particularly around the peer review process. Some camps espouse a human actioned/blockchain facilitated peer review process as outlined in this paper. Others say that humans should be eliminated from the peer review process and through semantics, making human written text machine readable, a computer should check the facts in a scientific article against other submitted articles, thereby performing a ‘machine review’. Still others say that humans should be removed even from the collection of scientific fact, with large and complex Internet of Things networks generating data that can be fed into a universal 'blockchain of absolute truth'. Any misunderstanding or misrepresentation of these latter two positions is entirely unintended. This paper outlines the first of these three schools of thought, believing that perfection should not become the enemy of good. If Aletheia is successful it will certainly bring projects of the other two camps closer to realisation, so it is hoped that everyone with an interest in blockchain and/or scientific communication can support Aletheia.

_With enough of us, around the world, we’ll not just send a strong message opposing the privatisation of knowledge – we’ll make it a thing of the past. Will you join us? - [Aaron Swartz, Guerilla Open Access Manifesto](https://archive.org/details/GuerillaOpenAccessManifesto)_
