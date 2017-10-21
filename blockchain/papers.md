<h1>Paper summaries</h1>
This page contains links to various papers related to blockchain and cryptocurrencies that I read and found useful. I have added the abstract and a brief summary for each paper.

<h2>Classic papers</h2>
<h3><a href='https://bitcoin.com/bitcoin.pdf'>Bitcoin: A Peer-to-Peer Electronic Cash System.</a> <i>Nakamoto 2008</i></h3>

<h4>Summary</h4>
<p align="justify">
This paper introduces the concept of implementing a distributed timestamp server by using a public <i>blockchain</i> combined with <i>proof-of-work</i> to prevent double spending. Using this, the paper proposes to build a peer to peer electronic cash system called <i>bitcoin</i>. The paper only gives a general idea about the concepts used in bitcoin and presents them quite informally. Much of the implementation details are skipped and can only be learned by reading the <a href='https://github.com/bitcoin/bitcoin/tree/4405b78d6059e536c36974088a8ed4d9f0f29898'>reference client</a> released in 2009.
</p>

<h4>Abstract</h4>
<p align='justify'><i>
A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution. Digital signatures provide part of the solution, but the main benefits are lost if a trusted third party is still required to prevent double-spending.  We propose a solution to the double-spending problem using a peer-to-peer network.  The network timestamps transactions by hashing them into an ongoing chain of hash-based proof-of-work, forming a record that cannot be changed without redoing the proof-of-work. The longest chain not only serves as proof of the sequence of events witnessed, but proof that it came from the largest pool of CPU power. As long as a majority of CPU power is controlled by nodes that are not cooperating to attack the network, they'll generate the longest chain and outpace attackers. The network itself requires minimal structure. Messages are broadcast on a best effort basis, and nodes can leave and rejoin the network at will, accepting the longest proof-of-work chain as proof of what happened while they were gone.
</i></p>

<h2>Literature survey</h2>
<h3><a href='http://www.jbonneau.com/doc/BMCNKF15-IEEESP-bitcoin.pdf'>SoK: Research Perspectives and Challenges for Bitcoin and Cryptocurrencies.</a> <i>Bonneau, et al. SP. 2015 </i></h3>
<h4>Summary</h4>
<p align="justify">
This paper gives a summary of history of research in cryptocurrency systems. It divides the important concepts into 3 categories which together form the core of cryptocurrencies: 1. <i>Transactions &amp; Scripts</i> 2. <i> Consensus and Mining</i> 3. <i>Stability</i>. For each category it explains the basic approach and further reviews various alternatives and improvements.
</p>

<h4>Abstract</h4>
<p align="justify"><i>
Bitcoin has emerged as the most successful cryptographic currency in history. Within two years of its quiet launch in 2009, Bitcoin grew to comprise billions of dollars of economic value despite only cursory analysis of the system’s design. Since then a growing literature has identified hidden-but-important properties of the system, discovered attacks, proposed promising alternatives, and singled out difficult future challenges. Meanwhile a large and vibrant open-source community has proposed and deployed numerous modifications and extensions. <br/>
We provide the first systematic exposition Bitcoin and the many related cryptocurrencies or ‘altcoins.’ Drawing from a scattered body of knowledge, we identify three key components of Bitcoin’s design that can be decoupled. This enables a more insightful analysis of Bitcoin’s properties and future stability. We map the design space for numerous proposed modifications, providing comparative analyses for alternative consensus mechanisms, currency allocation mechanisms, computational puzzles, and key management tools. We survey anonymity issues in Bitcoin and provide an evaluation framework for analyzing a variety of privacy-enhancing proposals. Finally we provide new insights on what we term disintermediation protocols, which absolve the need for trusted intermediaries in an interesting set of applications. We identify three general disintermediation strategies and provide a detailed comparison.
</i></p>

<h2>Altcoins</h2>
<h3><a href='https://www.weusecoins.com/assets/pdf/library/Ethereum_white_paper-a_next_generation_smart_contract_and_decentralized_application_platform-vitalik-buterin.pdf'>Ethereum: A next generation smart contract & decentralized application platform</a>. <i>Vitalik Buterin. 2014</i></h3>
<h4>Summary</h4>
<p align='justify'>
This white paper introduces the Ethereum protocol. It builds upon the concepts used in bitcoin to provide a general purpose, turing complete scripting language that can be used to build arbitrary <i>smart contracts</i>. It generalizes the bitcoin's block chain ledger by viewing it as a global state with each transaction defining a state transition. It gives details of the language including how it will prevent unbounded computation. It also gives various applications of the protocol including token systems, financial derivatives, identity systems, file storage, decentralized autonomous organizations etc. It gives details about the process of how the Ethereum protocol will be bootstrapped and other practical issues.
</p>