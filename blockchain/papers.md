<h1>Paper summaries</h1>
This page contains links to various papers related to blockchain and cryptocurrencies that I read and found useful. I have added the abstract and a brief summary for each paper.

<h2>Classic papers</h2>
<h3><a href='https://bitcoin.com/bitcoin.pdf'>Bitcoin: A Peer-to-Peer Electronic Cash System.</a> <i>Nakamoto. 2008</i></h3>

<h4>Summary</h4>
<p align="justify">
This paper introduces the concept of implementing a distributed timestamp server by using a public <i>blockchain</i> combined with <i>proof-of-work</i> to prevent double spending. Using this, the paper proposes to build a peer to peer electronic cash system called <i>bitcoin</i>. The paper only gives a general idea about the concepts used in bitcoin and presents them quite informally. Much of the implementation details are skipped and can only be learned by reading the <a href='https://github.com/bitcoin/bitcoin/tree/4405b78d6059e536c36974088a8ed4d9f0f29898'>reference client</a> released in 2009.
</p>

<h4>Abstract</h4>
<blockquote align='justify'>
A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution. Digital signatures provide part of the solution, but the main benefits are lost if a trusted third party is still required to prevent double-spending.  We propose a solution to the double-spending problem using a peer-to-peer network.  The network timestamps transactions by hashing them into an ongoing chain of hash-based proof-of-work, forming a record that cannot be changed without redoing the proof-of-work. The longest chain not only serves as proof of the sequence of events witnessed, but proof that it came from the largest pool of CPU power. As long as a majority of CPU power is controlled by nodes that are not cooperating to attack the network, they'll generate the longest chain and outpace attackers. The network itself requires minimal structure. Messages are broadcast on a best effort basis, and nodes can leave and rejoin the network at will, accepting the longest proof-of-work chain as proof of what happened while they were gone.
</blockquote>

<h2>Literature survey</h2>
<h3><a href='http://www.jbonneau.com/doc/BMCNKF15-IEEESP-bitcoin.pdf'>SoK: Research Perspectives and Challenges for Bitcoin and Cryptocurrencies.</a> <i>Bonneau, et al. SP. 2015 </i></h3>
<h4>Summary</h4>
<p align="justify">
This paper gives a summary of history of research in cryptocurrency systems. It divides the important concepts into 3 categories which together form the core of cryptocurrencies: 1. <i>Transactions &amp; Scripts</i> 2. <i> Consensus and Mining</i> 3. <i>Stability</i>. For each category it explains the basic approach and further reviews various alternatives and improvements.
</p>

<h4>Abstract</h4>
<blockquote align='justify'>
Bitcoin has emerged as the most successful cryptographic currency in history. Within two years of its quiet launch in 2009, Bitcoin grew to comprise billions of dollars of economic value despite only cursory analysis of the system’s design. Since then a growing literature has identified hidden-but-important properties of the system, discovered attacks, proposed promising alternatives, and singled out difficult future challenges. Meanwhile a large and vibrant open-source community has proposed and deployed numerous modifications and extensions. <br/>
We provide the first systematic exposition Bitcoin and the many related cryptocurrencies or ‘altcoins.’ Drawing from a scattered body of knowledge, we identify three key components of Bitcoin’s design that can be decoupled. This enables a more insightful analysis of Bitcoin’s properties and future stability. We map the design space for numerous proposed modifications, providing comparative analyses for alternative consensus mechanisms, currency allocation mechanisms, computational puzzles, and key management tools. We survey anonymity issues in Bitcoin and provide an evaluation framework for analyzing a variety of privacy-enhancing proposals. Finally we provide new insights on what we term disintermediation protocols, which absolve the need for trusted intermediaries in an interesting set of applications. We identify three general disintermediation strategies and provide a detailed comparison.
</blockquote>

<h2>Smart contracts</h2>
<h3><a href='https://www.weusecoins.com/assets/pdf/library/Ethereum_white_paper-a_next_generation_smart_contract_and_decentralized_application_platform-vitalik-buterin.pdf'>Ethereum: A next generation smart contract & decentralized application platform</a>. <i>Buterin. 2014</i></h3>
<h4>Summary</h4>
<p align='justify'>
This white paper introduces the Ethereum protocol. It builds upon the concepts used in bitcoin to provide a general purpose, turing complete scripting language that can be used to build arbitrary <i>smart contracts</i>. It generalizes the bitcoin's block chain ledger by viewing it as a global state with each transaction defining a state transition. It gives details of the language including how it will prevent unbounded computation. It also gives various applications of the protocol including token systems, financial derivatives, identity systems, file storage, decentralized autonomous organizations etc. It gives details about the process of how the Ethereum protocol will be bootstrapped and other practical issues.
</p>

<h2>Proof-of-work</h2>
<h3><a href='Altcoin://web.cs.dal.ca/~abrodsky/7301/readings/DwNa93.pdf'>Pricing via Processing or Combatting Junk Mail</a>. <i>Dwork & Naor. 1992</i></h3>
<h4>Summary</h4>
<p align='justify'>
This paper proposes a system for limiting junk mail by making the sender solve a <i>cryptographic puzzle</i> (e.g. a Fiat-Shamir based scheme). To allow legitimate users to send bulk emails, the paper uses the concept of <i>shortcuts</i> - which can be bought from a trusted party and helps solve the puzzle much quicker.
</p>
<h4>Abstract</h4>
<blockquote align='justify'>
We present a computational technique for combatting junk mail, in particular, and controlling access to a shared resource, in general. The main idea is to require a user to compute a moderately hard, but not intractable, function in order to gain access to the resource, thus preventing frivolous use. To this end we suggest several pricing functions, based on, respectively, extracting square roots modulo a prime, the Fiat-Shamir signature scheme, and the Ong-Schnorr-Shamir (cracked) signature scheme.
</blockquote>

<h3><a href='http://www.hashcash.org/papers/hashcash.pdf'>Hashcash - A Denial of Service Counter-Measure</a>. <i>Back. 2002</i></h3>
<h4>Summary</h4>
<p align='justify'>
Hashcash is a way to counter denial of service attacks by having the client do a proof-of-work. To make a connection, each client must add a nonce value to a starting string such that the hash of the starting string concatenated with the nonce has the given number of zero bits as a prefix. The number of zero bit prefix needed can be varied based on the load. The paper also presents an interactive version of the protocol.
</p>
<h4>Abstract</h4>
<blockquote align='justify'>
Hashcash was originally proposed as a mechanism to throttle systematic abuse of un-metered internet resources such as email, and anonymous remailers in May 1997. Five years on, this paper captures in one place the various applications, improvements suggested and related subsequent publications, and describes initial experience from experiments using hashcash.<br/>
The hashcash CPU cost-function computes a token which can be used as a proof-of-work. Interactive and non-interactive variants of cost-functions can be constructed which can be used in situations where the server can issue a challenge (connection oriented interactive protocol), and where it can not (where the communication is store–and–forward, or packet oriented) respectively.
</blockquote>

<h3><a href='http://fc15.ifca.ai/preproceedings/bitcoin/paper_12.pdf'>Cuckoo Cycle: a memory bound graph-theoretic proof-of-work</a>. <i>Tromp. FC. 2015</i></h3>
<h4>Summary</h4>
<p align='justify'>
This paper proposes a new proof-of-work that needs a lot more memory access compared to cpu cycles. This may prevent ASIC miners from having a huge advantage over normal CPU based miners. The proof-of-work in this case consists of finding a fixed length cycle in a large, random, sparse graph. The difficulty can be adjusted based on hash of the solution as well as size of the graph. To reduce memory access, much more CPU cycle needs to be used.
</p>
<h4>Abstract</h4>
<blockquote align='justify'>
We introduce the first graph-theoretic proof-of-work system, based on finding small cycles or other structures in large random graphs. Such problems are trivially verifiable and arbitrarily scalable, presumably requiring memory linear in graph size to solve efficiently. Our cycle finding algorithm uses one bit per edge, and up to one bit per node. Runtime is linear in graph size and dominated by random access latency, ideal properties for a memory bound proof-of-work. We exhibit two alternative algorithms that allow for a memory-time trade-off (TMTO)—decreased memory usage, by a factor k, coupled with increased runtime, by a factor Ω(k). The constant implied in Ω() gives a notion of memory-hardness, which is shown to be dependent on cycle length, guiding the latter’s choice. Our algorithms are shown to parallelize reasonably well.
</blockquote>
