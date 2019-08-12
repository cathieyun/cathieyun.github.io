---
title: "Splinter: Practical Private Queries on Public Data"
collection: publications
permalink: /publications/2017-03-splinter
excerpt: 'This paper presents Splinter, a system that protects
users’ queries on public datasets while achieving practical
performance for many current web applications.'
date: 2017-03-27
venue: 'Proceedings of the 14th USENIX Symposium on Networked Systems Design and Implementation (NSDI '17), Boston, March'
paperurl: 'https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wang-frank.pdf'
citation: 'Frank Wang, Catherine Yun, Shafi Goldwasser, and Vinod Vaikuntanathan. (2017). &quot;Splinter: Practical Private Queries on Public Data.&quot; In <i>Proceedings of the 14th USENIX Symposium on Networked Systems Design and Implementation (NSDI '17), Boston, March</i>.'
---
Many online services let users query public datasets such as maps, flight prices, or restaurant reviews. Unfortunately, the queries to these services reveal highly sensitive information that can compromise users’ privacy. This paper presents Splinter, a system that protects users’ queries on public data and scales to realistic applications. A user splits her query into multiple parts and sends each part to a different provider that holds a copy of the data. As long as any one of the providers is honest and does not collude with the others, the providers cannot determine the query. Splinter uses and extends a new cryptographic primitive called Function Secret Sharing (FSS) that makes it up to an order of magnitude more efficient than prior systems based on Private Information Retrieval and garbled circuits. We develop protocols extending FSS to new types of queries, such as MAX and TOPK queries. We also provide an optimized implementation of FSS using AES-NI instructions and multicores. Splinter achieves end-to-end latencies below 1.6 seconds for realistic workloads including a Yelp clone, flight search, and map routing.

[Download paper here](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-wang-frank.pdf)

Recommended citation: Frank Wang, Catherine Yun, Shafi Goldwasser, and Vinod Vaikuntanathan. (2017). &quot;Splinter: Practical Private Queries on Public Data&quot; <i>USENIX NSDI 2017</i>