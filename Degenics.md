# degenics

# Decentralized Genetics

### Latest changes to main project always concurred by [CHANGELOG.md](https://github.com/Degenics/degenics-public/blob/main/CHANGELOG.md) via weekly sprint.

### This file provides a more detailed concept document for the Degenics project.

If you found this file somewhere else, organizational repo for the project is at [Degenics](http://github.com/Degenics) and the public-facing website is at [decentralizedgenetics.com](http://decentralizedgenetics.com).

Caveat: *The Following Concept Description is licensed via [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/), to Pandu Sastrowardoyo / [Decentricity](http://github.com/Decentricity)*

# Elevator Pitch 

## Degenics: The Decentralized Genetics Initiative

We are building a decentralized platform for your personal genetics.
Our concept allows synergy between labs of all scales while guaranteeing user anonymity and sovereignty at every step of the genomic data science workflow—
from sample collection, data storage, to report generation.

## Vision

We aim to democratize direct-to-consumer genomics with a privacy-preserving, anonymous-first platform running on a fully decentralized, autonomous infrastructure.

## WHY?

* **To provide an alternative to centralized personal genetic testing services, an alternative where privacy is enforced at infrastructure level, where users control their data from sending to monetization**
* **To empower labs everywhere possible by adding to their revenue streams and optimizing their PCR equipment yield**
* **To provide consumers with a stigma-free, private and anonymous health service, be it for lifestyle or healthcare motives**

# Opportunities

## A Sizable Market

As per the report published by Allied Market Research, the global genetic testing market generated $12.68 billion in 2019, and is projected to reach **$21.26 billion by 2027, growing at a CAGR of 10.1% from 2020 to 2027**.

## An Answers to Several Problems

### **PROBLEM ** : PERSONAL GENOMICS COMPANIES OWN, MONETIZE , OR LEAK USER DATA AND PERSONAL ID.

It is no secret that certain conditions and illnesses come together with social stigma. Requiring physical presence and named documents may prevent their efficient detection and/or prevention. 

Beyond the social aspect, personal genomics company are in possession of their user's ID, personal data and DNA analysis data. Those data, that should belong exclusively to the service's users. [These companies already sell users' genes to pharmacogenetics research with arguable consent.](https://time.com/5349896/23andme-glaxo-smith-kline/)

Personal genomic companies [are already being hacked ](https://www.bloomberg.com/news/articles/2018-06-05/hack-of-dna-website-exposes-data-from-92-million-user-accounts)in certain cases.

**ANSWER**: Degenics uses a blockchain based network together with additional cryptographic measures to ensure that users can remain anonymous , and the sole owners of their data. Reuse and monetization are possible, and entirely up to the users.

### PROBLEM : CUSTOMERS CAN'T NORMALLY CHECK THE EFFICIENCY AND ACCURACY OF THE SEQUANCING AND ITS RESULTS, UNLESS THEY HAVE THEIR OWN LABS AT HOME

While it might be possible to download raw genome sequencings from DNA analysis services, users generally do not have the means and knowledge to independently verify their accuracy. Second opinions require another end-to-end sampling, sending and analysis process, which causes time, money and further data exposure. 

**ANSWER**: Degenics lets users privately keep and re-share sequencing files in order to resubmit it to health specialists on a need-to basis. As a control mechanism, users are also able to select more than one lab to generate those initial results, which contribute to mitigate inconsistencies and isolate bad potential bad actors.

### PROBLEM: PCR DEVICES ARE EXPENSIVE AND NOT ALWAYS READILY AVAILABLE, WHICH DRIVES UP CONSUMER PRICES AND TESTING SERVICE YIELD

Accurate PCR devices represent a real investment for heath related institutions. DIY kits do exist, but their precision level isn't enough to carry a comprehensive range of tests. As a result, waiting time and service prices are kept up. 

**ANSWER** : Degenics can onboard independent laboratories, universities, clinics, hospital and DYI genomics enthusiasts to create a high availability marketplace, where DIY owners see a raise in income, and users can enjoy more affordable prices. 

## A Wide Rage of Extended Uses

### Self Data Monetization

1. Users have the option to sell their non PID genetic data to parties that requires this data for research
2. A system to protect the data and monitor access to the data is required.
3. Purchasers of genetic data will be required to make a payment in fiat or DGNX token in order to access this data.
4. Fiat payment that is received will be used to purchase the DGNX token from crypto markets
5. DGNX tokens will be re-distributed or burned according to the decision of the DAO

### Health, Lifestye and Wellness Products

<u>Genome Risk Analysis</u>

- Disease risk analysis.
  Know what diseases you have contracted or might contract in the future (Including COVID and SARS-Cov2 
- Descent disease risk analysis 
  Know what diseases your children might be prone to by checking your genome against your spouse's

<u>Self Knowledge</u>

- Your metabolism (Dietary consulting  — which foods are best for your health, to prevent disease or reduce weight, exercise, skincare, personalized advice)
- Find Physical and behavioral traits
- Find(and monetize) your rare genes
- Personality and character traits
- "Find Your Super Power"

<u>Ancestry</u>

- Ancestry (Who do you share blood ties with?)
- Heritage (ethnic mix and geographical family migration history)

### MVP Vision

Degenics 1.0 (private deployment March 2021) will provide anonymous, decentralised sample collection, payment, data storage, and report distribution. 
TL;DR: a VPN for your DNA.

### Who we are

Degenics is a group of IT consultants, blockchain developers, and biologists who are passionate about privacy, decentralized technologies, and genomic data science.

* [Pandu Sastrowardoyo](http://github.com/Decentricity) - Initiator
* [Gilang Bhagaskara](http://github.com/gilangbh) - Tech Lead
* Jean-Daniel Gauthier - Product Lead
* Aaron Ting - Marketing Lead
* [Bobby Andika](http://github.com/ybobby) - Dev Lead
* [Muhammad Arif](http://github.com/marcondol) - Back End and Blockchain
* [Aloysius Dedy](http://github.com/aloisius82) - Blockchain and Smart Contracts
* [Kevin Janada](http://github.com/kevinjanada) - UI/UX
* Ibnu Gamal Alhadid - Advisor

# Tech Overview

## Trustless/Fully Decentralized Model

### Anonymous Physical-Digital Bridge

Without having to enter KYC, the user activates the dApp and generates her passphrase. This forms the basis of her private key, and is paired with a sharable public key.

The user takes two samples -- a cheek swab to be practical-- and puts them into a sample bottle each. Each sample bottle is put into its own envelope.

dApp creates an envelope label that the user can either rewrite or print on the sample envelopes. This envelope label contains her public key, no personally identifiable information and no return address, but does contain 2 lab addresses to send samples to.

User sends the two envelopes via her local post office box.

### Decentralized Labs, Sovereign Data

The aforementioned labs analyze the sample and produce datasets (VCF file & analysis).

The platform compares datasets from the  two labs and checks the difference between select points in the data.

If there is more than 10% difference, the user is given the option to send in another sample. Sampling instructions are provided again.

If there is less than 10% difference between two output datasets. both are encrypted with the user's public key and put inside the platform (Blockchain + Decentralized Storage).

User is alerted, and can access her data at any time by decrypting via private key.

## Enterprise/Consortium Model

### Semi-Decentralized  Deployment with "Lab Marketplace"

An alternative deployment model would be the private / consortium deployment where labs are directly selected by the users.

This simplifies the workflow while maintaining the anonymity of the users. The labs get access to a commercial market, and the users still get an anonymous physical-to-digital bridge for their genomic data.

Additionally, after the initial on-ramp, the labs are free to up-sell additional analytics products to the users, without resampling.

# Financials

## Circulating Token Supply

* Year 0 - 2.5mil
* Year 1 - 3.46mil
* Year 2 - 4.1865mil
* Year 3 - 4.913 mil
* Year 4 - 5.6395 mil
* Year 5 - 6.366 mil
* Year 6 - 7.0925 mil
* Year 7 - 7.819 mil
* Year 8 - 8.5455 mil
* Year 9 - 9.272 mil
* Year 10 - 10 mil

## Token Allocation

1. Private Sale (20%)
2. Team Members and Advisors (5%)
3. DAO Allocation (20%)
4. Marketing/Partnerships (10%)
5. Local Support (10%)
6. Client Incentive (10%)
7. Hospitals/ Labs (10%)
8. LP Provision and LP Rewards (10%)
9. Supplies (2.5%)
10. Airdrop and Bounties (2.5%)

## Tech-Related FAQ

### If things are happening anonymously, how does the user/customer pay for the service?

There are two options, the traditional option or the fully decentralized option. We prefer fully decentralized, but this might not be an option in all locales. Traditional payment models may also work better for consortium or private deployments of Degenics.

#### Enterprise/Consortium Model

The traditional option: Consumer funds are held in escrow by a local payment gateway or bank until the lab provides valid data (report and genome) into decentralized storage. The smart contract then triggers fund disbursement into the lab's accounts. Note that this still maintains anonymity of the genomic data, since:

- Payment gateway / bank does have access to consumer KYC, but does not have access to genomic data or reports
- Labs don't have access to consumer KYC, although it does have access to anonymized genomic data.

#### Trustless/Decentralized Payments

All transactions happen via a Blockchain token model. Consumer onboards with their preferred cryptocurrency token, or goes through a fiat-to-crypto bridge (example here) to pay. Smart contracts hold consumer's tokens in escrow until labs provide valid data. The smart contract then triggers fund disbursement into the labs' account

### Why 2 labs?  Is it for the sake of comparing the result?

We designed Degenics with 2 labs per transaction since we want to solve this following global problem with personal genetic testing:

Unlike other categories of services, consumers can't recheck the results of DNA analytics services unless they have access to a lab or PCR device of their own.

This, we feel, places consumers at a disadvantage and may lower the quality of future genetic testing results within the ecosystem.

Thus, we designed the platform with a semi-random, rating-based selection of two labs per transaction to ensure two things:

- All labs, from garage DIYBiolabs to large companies, can join the ecosystem and compete with each other.
- The quality of the results are maintained, even with the consumers being anonymous.

The two labs model is optional (users can elect to just choose one lab to send to), but Degenics believes that the future of a truly decentralized genetic testing ecosystem lies here.

In the long term, this system also allows the ecosystem to grow further -- with smaller labs helping to check the larger labs, and vice versa. The rating system associated with the labs would also provide incentives for the ecosystem to increase in quality.

### Personal genome files are huge. How would you expect to send these files via Blockchain?

You're right -- genome files are quite large. Raw PCR output can be up to 900GB, and even VCF files hover around 10-100MB (for a subset of sequences) or 1GB (for Whole Genome Sequencing).

Here's our strategy in enabling these files to be shared and owned by the user:

* First, we will focus on the VCF files exclusively. In our initial POC, only the smaller VCF files will be included in the "result package" sent to each user, along with the report.

* Second, we will utilize a combination IPFS / torrent platform to act as the decentralized storage mechanism. The "result package" is encrypted off-chain (with the user's public key) and put within this decentralized storage platform.

* Third, the main blockchain platform itself will link to the decentralized storage mechanism through a hash list. This means that the main blockchain platform only contains pointers to the data in decentralized storage, and not the actual genomic files.

In the enterprise/consortium strategy, the IPFS/torrent platform can be replaced with regular public or private cloud solutions.
