# Ethereum Zurich 2024

## Friday 5th April

### Fireside Chat Regulation

- Prof. Dr Claudio J. Tessone
- Alexander Brunner

General discussion about regulation of the crypto space in Switzerland and Europe with the new MiCA law. MiCA primarly tries to regulate centrlized entites. It is unclear how they are going to regulate decentralizes organizations because they need to regulate entities. Since a DAO is not an entity there is no quick solution how they are going to regulate. According to FINMA this must first be changed in law before any regulatory clarity can exist.

### Cryptonative Economy Report

- Josef Je

PWN's goal is to give crypto natives the same financial services as traditional banks do. Like loans or morgages. They publish a report that shows how much money people spend on fees related to different fileds. L1 fee revenue in 2022 was about 5.5 billion USD an 80% of those fees came from ethereum. In 2023 the narative in crypto change to liquid staking dirivatives and layer 2 systems. Fee revenue decreased by about 17%. Ethereum transactions where stable during 2023 but layer 2 transactions where and sill are rising.

Report: https://cryptonative.pwn.xyz

### Speculative Denial-of-Service Attacks in Ethereum

- Arthur Gervais

Reverted transactions also cost a fee to prevent DoS attacks. A problem associated with this is censorship. An example of this is Tornado Cash. The contracts where blacklisted by the United States. The DoS here is that a builder (validator, miner, ...) needs to check for blacklisted transactions which fees cannot be accounted for.

Ethereum Censorship: http://censorship.pics

### Future Use Cases Of Digital Identities

- David Bakk
- Luca von Wyttenbach
- Bill Laboon
- Micha Bitterli

Digital identities are basically digital passports where the user can choose which information she wants to share with some party. Use case could be everywhere where one needs to prove that you are a human beeing or some specific properties like age or nation of origion and so on. Other examples are protection mechanisms against fake news or deep fakes.

Website: https://www2.deloitte.com/ch/de.html

### The Case for Native Account Abstraction

- Antoine Sparenberg

Externally Owned Accounts can only be the source fo a transacton. Contract accounts however can contain code but cannot execute a transaction. In 2018 Argent used a relayer (EOA) combined with a contact account so simulate account abstraction capabilities on Ethereum. Since the relayer is centralized this was not the best solution. With ERC-4337 however the relayer could be decentralized. Now the smart account sends a so called user operation to a bundler (decentralized relayer) which then will execute a transaction. Problem with this approach is that DApps would need to implement two UIs and user flows. See https://eip1271.io. Starknet solved this by only supporting Contract Accounts and therefore not giving users or dapps a choice.

Argent: https://www.argent.xyz

### Navigation the Waters of Decentralized Exchanges and On-Chain Spot Trading

- Raphael

Automated Marketmakers make price discovery using Arbitrageurs who are buying or selling assets accoring to the external price information they have access to. The liquidity provision on the other hand get a reward for providing liquidity in the form of a fee they get whenever someone trades tokens on the AAM. Concentrated liquidity AMMs save the liquidity at 0 and infinitly problem. Liquidity providers can set a range where they want to provide liquidity within. However, when the price moves out of those bounds a liquidity provider will not earn any fees anymore and is left with one of both assets. This problem is calles LVR. New AMM designs try to solve this. For example by bringing in pricing oracles or batching transactions together and executing them at a uniform price.

- Arrakis: https://www.arrakis.finance

### Bridging EVM and Non-EVM Assets: A Practical Approach

- Michael Bucher

The Neo blockchain has been around since 2014. It is a non-EVM chain and has multiple language support. Currently non-EVM chains have it harder to get integrated into centralized exchanges or stable coins for example. The upsides are that they can be faster and follow different approaches. Neo-X is a new EVM compatible sidechain that should be using the same native token $GAS as Neo. Therefore one needs to bridge the tokens from Neo to Neo-X. The team at AxLabs researched different approaches to do this and explained how they solved those very specific problems.

Neo: https://neo.org

### Shared Sequencing and Latency Competition as a Noisy Contest

- Akaki Mamageishvili

Ethereum is scaling with rollups fastly. The fact that there are may different rollups creates the problem of fragmented liquidity. With a shared sequencer this can be mitigated. Arbitrageurs can cross chain trade tokens and the shared sequencer will guarantee that one arbitrageur will win the trade. How the winner gets selected will be chosen according to some signal. This signal can either be first come first server or could use some other cost function.

Shared Sequencers: https://www.alchemy.com/best/shared-sequencers

### Threshold Cryptography for Multichain Dapps

- Björn Tackmann

The network of nodes jointly controls a cryptographic key, in a way such tat a misbehaving minority cannot extract any information about it. The threshold for example on a ploynomial of degree d = 3 woud be d + 1 = 4. This is because if you know 3 Points on the polynomial you cannot derive the polynomial from it. But if you know another point you can. This all is in contrast to multi signature where every party has a different key and the one that validates therefore exactly knows who provided the key. This is not given with threshold keys.

ICP Threshold Keys: https://internetcomputer.org/docs/current/developer-docs/smart-contracts/encryption/t-ecdsa

### MULTI-CHAIN GOVERNANCE: ON-CHAIN VOTING WITH ETHEREUM AND INTERNET COMPUTER

- Björn Assmann
- Severin Siffert

Decentralized voting is a core aspect of blockchain governance. Since fees are pretty high lots of this is done off-chain. ICP consists of so called subnets that can run canisters (smart contracts). In the example a simple voting application was built.

Example App: https://vbruu-oqaaa-aaaal-ai5aq-cai.icp0.io
Fork Repo: https://github.com/jbaettig/icp_multi_chain_voting

### Build Dapps at Lightning Speed

- David Dal Busco

Juno is an open-source Blockchain-as-a-Service solution based on ICP that simplifies Web3 development. In the workshop a simple note application was built on ICP using Juno.

Website: https://juno.build
Fork Repo: https://github.com/jbaettig/juno_workshops

## Saturday 6th April

### Building Universal Web3 Apps with React Native

- Thiago brezinski

With react native one can build on iOS, Andorid, web, Windows, macOS, visionOS and many more. Many DApps are web only mostly because of the populairty of browser wallets. The react native quick crypto library can be used to build react native DApps. Good modules to use:

- Expo: A framework to help you develop universal apps with react native.
- React Native Web: A compatibility layer between React DOM and React Native.
- React Navigation: The standard navigation library in React Native.
- Viem: The lightweight interface to Ethereum.
- Wagmi: React hooks wrapper on top of Viem.
- Walletconnect Web3Modal: Cross platform solution to connect to app to hundreds of wallets.

Plattform specific code can be easlily written als shown in the picture below. Metro can handle this more or less automatically.

Example App: https://github.com/junobuild/workshops

PS: React native would be cool for Papyrus!

### Blockchain's ChatGPT Moment: Unlocking new Opportunities for SMES and Enterprises

- Giovanni Vanini

Today the main usage of NFTs and blockchain in general are nieches. The problem with Blockchain "marketing" is that it often focuses on technology but enterprises do not realy care about that. The care more about how the blockchain helps them to be more productive.

### DAO Modularity - The next Unlock

- Antony Leutenegger

Missed most of the talk. Look into Aragon. Might be interesting for Papyrus.

### Breaking the Code: ETHDebug Format for Smart Contract Debugging

- Nebojsa Urosevic

A good debugger is always important. Especially in Web3 where smart contracts manage lots of funds. The team of tenderly showed a demo of their product. You can set brakpoints and go though instruction by instruction and output variables on the command line similar to debuggin in other applications.

### Essential Maths for Zero Knowledge Proofs

- Laurence Kirk

Intorduction to group theory, (finite) fields and complexity theory. Zero knowledge proves are in the interactive proof calss when it comes to complexity theory. A explanatory video can be found in the slides linked below. With SNARKs the proof has always the same size. With STARKs the proof is growing with the transaction size. Zero knowledge proof systems use polynomial commitment schemes to keep the size of the proof small.

-> Best presentation so far. Really liked it. Maybe also a good topic for CS Seminar.

Slides: https://drive.google.com/file/d/1mFTZsjf2hFAfmCo-yFzCwfZcnQlpwLJw/view

### Elliptic Curves

- Özgür Armanc Yigit

Introduction to elliptic curves, finite fields and scalar multiplication.

### On-Chain Undercollaterized Credit: Banking but Worse

- Andreas Fletcher

Overcollateralization is when you must provide a security that has more value than the a loan you want to get. With undercollateralization the privided security can be less than the loan one wants to get. In crypto overall loans are very overcollateralized. An itneressintg thought within the presentation was that stablecoins are in fact already undercolleteralized since they are backed by central bank money which by defintion is undercollateralized.

Wildcat: https://wildcat.finance

### Bridging Traditional Finance and Blockchain

- ROSTYSLAV

Traditional finance on the blockcahin would increase transparency and improve accessibility and inclusion. Tokenization would enable taking loans against the asset behind the token. For example an NFT that represents the owership of a part of an appartment complex. Issues currently are regulatory and compliance issues and also technical problems like getting real world information on chain. I did not really get what their product is doing. Has something to do with restaking.

Website: https://asymetrix.io

### The Swiss DLT Law in Practical Application

- Nicola Plain

Aktionariat brings Stocks on the Blockchain. All legal in Switzerland. The problem with private equity is that it is in general only available to high networth individuals and on averadge you have to hold the share for at least 7.5 years since there is no secondary market. With tokenization this can be changed. Aktionariat uses slightly changed liquidity pools. That also enables companies to allow easily buybacks for example.

-> Might be interesting vor Avantic AG ;)

Website: https://www.aktionariat.com

### Build with a Hardware Device

- Akram el Milligy

On a Ledger one needs to install blockchain specific applications which run in isolation. There are for different connection layers which are explained in the picture below. Akrem then showed a demo on how to integrate leder.

Sample Repo: https://github.com/aelmilligy-ledger/examples-ledger/tree/main/sign-personal-message
Developer Portal: https://developers.ledger.com

### Opportunities in CEDEFI

- Aliya Das Gupta

Sygnum bank is a classic bank but you can also buy and sell crypto. It calls itself a CeDeFi bank since they integrate functionality fo CeFi and DeFi. They also support staking coins and give you a tax statement for that. Another feature is social recovery.

-> They sound interesting. However I would still prefer to own my keys.

Website: https://www.sygnum.com

### Are RWAs the Answer to the DeFi Boom-Bust Cycle?

- Niklas Kunkel

Revenue is generated by yield which is correlated to revenue. The boom-bust cycle is therefore the sharp charp rise and decline by revenue. This is correlated to the bear- and bullcycles of crypto in general. Niklas quickly introduced Maker DAO which creates the DAI stablecoin. They use on- and off-chain assets to back the coin including real world assets. RWAs for Maker are mainly short term us goverment treasury bills. However one must keep in mind that RWA are not crypto native. This makes it important to know the contexts of RWAs.

- Custody: Who holds the off-chain asset? How can it be verified?
- Liquidity: How much liquidity is there if there even is any?
- Counterparty Risk: On must keep in mind that a party could default.
- Yield: The protocol could automatically optimize for yeald and sell RWAs with bad yields for the better ones.

Website: https://chroniclelabs.org

## Sunday 7th April

### Designing a Decentralized Atonomous Organization

- Florian Spychiger

A DAO has five strucural elements wich are in the center of the picture below. For a DAO the following things are important:

- Purpose: Bild a strong community around a shared prupose that creates a sense of connection and solidarity.
- Legislation: The legal structure may affect the organizational design, e.g. the organisazional bodies. However, there is still a lot fo freedom to design teh organizational process.
- Business & Use Case: New thinking of business models with more equil

- Organizational Bodies: Power distribution in a decentralized organization is the holy grail. Just because we are all equal and have the same rights doesn't mean everyone needs to vote on everything.
- Decision-Making: If a few people own a company in the sense of shareholders, and then a lot of people decide what happens with this investment? On person voting or token based voting? The dicision making process should align with the purpose of the DAO.
- Token: They can signal mebmership, decision rights and can be financial assets of a DAO.
- Treasury: What are the asset? The innovative thing about DAOs is that the community vote on what happens with the treasury.
- Communication: Should not be underestimated. Members should have one source of trouth.

-> Quadratic Voting is interesting concept.

Website: https://dawo24.org

### Demystifying Account Abstraction EIPs

- Ivo Georgiev

Account abstraction is valuable since it makes onboarding easier. For example socail recovery oer email based account recovery instead of seed phrases. It also makes it possible to pay gas with other tokens than ETH.

ERC-4337: Bare minimum to make account abstraction realy work. The good thing is that no consensus changes are needed to implement it unlike EIP-2938 which was the OG AA EIP. Another plus is that it standardizes smart account user operations and enables paymasters.
ERC-6492:

-> So many EIPs not so much time.

### Unlocking Ownership: The Path to an Invisible Web3 Though Account Abstraction

- Lukas Schor

Safe provides multi-signature smart contract wallets and social login or passkeys. Recovery could be made by social recovery or a trusted thrid party with banks or centralized exchanges. With keystores one can create many public keys by one private key.

Website: https://app.safe.global/welcome

### Even Faster P256 for On-Chain Passkeys and SGX

- Renaud Dubois

secp256r1/P256 is an elliptic curve. It enables to us passkeys in account abstraction.

-> Good that I took cryptography module in my master. At least i understood some parts of the presentation.

### The Magic of Native Account Abstraction on ZKSync

- Gauthier

Only about 1% of users are actually using AAs at the moment. One problem is that users must have gas to deploy a smart contract wallet. Another point is that they do not like to switch wallets when they already have an EOA. ZyFi enables paymaster transactions on ZKSync. This means a user can pay gas in a token of their choosing or projects could sponser gas for early adoptors or similar.

Website: https://www.zyfi.org

### Bring your own Execution Environment

- zpedro

Wallets are currently not fit for privacy and that is a problem. The proovs of ownership are currently on-chain and therefore public. That means that users need to prove the exection on their own machine. The wallets of the future should be able to do this easily.

Website: https://aztec.network

### Decentralized ID for those that need it the most

- Aleksejs Ivashuk

Who issues your proof of identity and who ownes it? This is a curtial thing since if one has no legal identity one has no rights. Currently the proof of identity is created by the state and is owned by the state which means that the government owns everyone who they have identified. The governments can revoke these and make people stateless. Stateless people cannot participate in daily live since they cannot identify them selfes. For example they cannot open a bank account or similar.

- We carry our ID data with us in form of biometrical information.

Website: https://apatride.eu

### Efficient Light Client for Stateless Verification

- Sogol Malek

One of the biggest problems of ethereum is currently state bloat. This leads to longer block verification times. Currently there are full nodes and light nodes which have different properties when it comes to efficiency and security. Stateless light clients are slowly but surely coming. They do not require the whole state to check if a block is valid. Only a small amount of information is used which is called a witness.

### How can you assess if your Blockchain Scales?

- Filip Rezabek

Problems of increasing block size on ethereum leads to som problems. Validators must process more data and need better hardware to get this done in time. The peer to peer network must also support the increas of blocksize and must have increased throughput. Scaling of the blockchain can be measured by evaluating how good it scales horizontally or vertically. Some challenges that come with this are on-boarding new ecosystems.

GitHub: https://github.com/rezabfil-sec/engine-framework

### DeFi Supervision - Who's Task is it?

- Tim Weingaertner

Short introduction to DeFi followed by a workshop. Currently supervision of DeFi protocols is made by the "community" if they are supervised at all. This is a problem since DeFi comes with many risks als seen in the picture below.

The aim of supervision is transparancy, risk managment, market integrity, financial stability, comuser protection, compliance with laws and the promotion of competition. Promotion of competition is importent when it comes to prevent monopoly.

-> The national regulator should check if the local laws are held by the protocol. The rest should be done my the community.

Paper: https://www.mdpi.com/1911-8074/16/10/454

### Zero Knowledge Proof of Reserves

- Hodlon

In the past there where many central exchanges going down like Mt. Gox or more recently FTX. In both of these cases neither the exchanges nor the customers knew what was happening with the assets of the exchange. Proof of reserves should make transparent if the exchange has all the funds to payout all customers. Proof of reserve could be used for any costodials not only exchanges. To create a proof of reserve one must transparently show all assets and liabilities. Typically a proof of reserve is a snapshot of a specific point in time that is then reviewed by an auditor. This is a problem since not many audit firms touch crypto. Summa tries to cut out the auditor by using zk technology.

Website: https://pse.dev/en/projects/summa
