---
cover: >-
  https://images.unsplash.com/photo-1498050108023-c5249f4df085?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwyfHxjb2RlfGVufDB8fHx8MTY0ODc2MTU3OA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Introduction

Currently, distributed ledger technology (DLT) \[**2**,**3**]— especially those based on blockchain ledgers—is a subject of interest because many companies are rushing to take advantage of the perceived benefits of using a time-oriented, tamper-proof ledger of records as a public or intercompany backbone for transactions, data keeping, and process monitoring.

According to the leading provider of market and consumer data Statista ([**https://www.statista.com**](https://www.statista.com), accessed on 15 October 2021), worldwide spending on blockchain solutions will grow from 1.5 billion in 2018 to an estimated 15.9 billion by 2023. In the first quarter of 2021 alone, blockchain startup companies around the world amassed 2.6 billion U.S. dollars in venture-capital funding, more than the whole year of 2020 \[**4**].

Expanding on the idea of a decentralized currency, as implemented in Bitcoin, many of these startups are explicitly building decentralized business models as an alternative to the existing centralized ones. They promote this idea as “cutting out the middleman” \[**5**] thanks to a peer-to-peer network where customers and suppliers make transactions directly, with the goal of decentralized data storage and saving money on transaction fees. In this regard, DLT offers new paradigms on how companies and people can interact and negotiate and new ways in which assets and data are represented and monetized. The benefits and prospects deriving from this received attention—sometimes perhaps a little too optimistically and superficially—for many application domains and related use cases. Some surveys conducted by Statista, which involved hundreds of companies worldwide during the three years 2018–2020, reflect this state of affairs. For example, **Figure 1** presents use cases for blockchain technologies as of 2021. This statistic shows that companies were working on use cases concerning the following four main broad topics: digital currencies/payments, data sharing/reconciliation, identity protection, and asset transfer/traceability, each of which can be in itself declined and adapted to many different application scenarios.

![](file:///C:/Users/Phill/AppData/Local/Temp/ksohtml/wpsCA7C.tmp.png)&#x20;

**Figure 1.** Global organizations’ use cases for blockchain technology as of 2021 (©Statista) \[**6**]. Percentages equal more than 100 percent because respondents were allowed to submit more than one answer.

**Figure 2** instead shows the factors that over this span of years have been perceived as the main obstacles that discourage more significant investments in blockchain technology and platforms. As the outcomes show, only a strict minority of respondents believed there were no barriers. At the same time, significant uncertainties concerned the actual usefulness and viability of this new technology, the risks associated with its adoption, and the lack of adequate regulations and standards.

![](file:///C:/Users/Phill/AppData/Local/Temp/ksohtml/wpsCA8D.tmp.png)&#x20;

**Figure 2.** Perceived barriers for investing in blockchain technology during the three years 2018–2020 (©Statista) \[**7**].

_1.1. Paper Contribution and Organization_

Many of the contributions to the literature in recent years have tried to mitigate the above problems by orienting operators and people potentially interested in developing or using DLT thanks to an examination of existing solutions and their main characteristics in terms of both functionality and performance, referring to (a set of) specific application domains or use cases. In some cases (see **Section 1.2**), these contributions take the form of real _vademecum_, which is a ready but reasoned reference for a conscious choice of the most appropriate platform (often the best compromise among both DLT platforms and traditional systems and architectures) able to satisfy one’s needs.

The purpose of the present work is different: it aims to discuss the evolution of some basic DLT concepts in terms of their scope and implementation, the emerging of new concepts and tools, and which prospects these concepts and tools can have in terms of the effectiveness of the decentralization solution obtained and its cyber-physical security. Overall, this work intends to provide a broad overview of the main concepts, approaches, and technical solutions that have characterized the development of DLT so far. Its main contributions are:

· an in-depth critical discussion of the concept of _decentralization_ and its implementation in current DL systems. Decentralization is the primary goal of any DL system, and we discuss it for system architecture and governance, also considering how the system interacts with the outside world during its operation;

· a reference architecture for DLT, in order to provide an integrated and comprehensive view of the function and role of the various concepts and tools offered by this technology;

· a new classification for consensus protocols based on a five-component framework, aimed at underlining similarities and differences between the protocols recently introduced for DL systems and those introduced since the eighties for more traditional distributed systems. Rather than providing a broad array of blockchain consensus protocols with technical details, we focus on the milestones of research developments in this sector, citing only those protocols that we believe have introduced truly innovative features;

· a review of the most relevant tools and strategies introduced for integrating DL systems with the physical world. This integration is an emerging and exciting research field whose primary goal is to design and develop cyber-physical systems capable of implementing an extended notion of process authentication, which encompasses both digital and physical assets. In this context, we introduce the notion of _authentic data encoding for physical resources_ (AD-ExPR), which results in a constructive scheme for the authentication of a physical resource through alphanumeric data. To the best of our knowledge, some authors in the literature implicitly used but did not explicitly define this scheme.

The remaining part of this survey is organized as follows. **Section 2** discusses the two opposite models of achieving decentralization through DLT, with their significant differences in system governance, ledger management, and business models. **Section 3.4.1** illustrates the core notions and their diverse implementations in major DLT platforms compared to a reference architecture. In particular, this section compares the different types of technical solutions proposed for the ledger structure and the consensus protocol to allow better performance and a more extensive set of possible applications. **Section 4** discusses some emerging concepts and techniques whose scope is to reliably connect DLT networks to the physical context in which they must operate. The idea is to obtain cyber-physical systems capable of implementing an extended notion of process authentication, contemplating all the different agents that contribute to realizing the process, whether digital processes, human operators, or physical devices. Finally, **Section 5** summarises our findings, indicating their implications for theory and practice.