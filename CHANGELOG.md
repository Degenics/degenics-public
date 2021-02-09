# Changelog
Sprint is **weekly**. Outside of holidays, sprint call is **every first working day of the week.**

## Initializing 2020/12/21 [Unreleased](https://github.com/Degenics)

- Gitlab initialized ([kevinjanada](http://github.com/kevinjanada))
- Google Cloud Platform initialized ([Decentricity](http://github.com/Decentricity))
- Migrated Gitlab to Github (non-technical considerations applied) ([Decentricity](http://github.com/Decentricity))
- Domain acquired, [www.degenics.com](http://degenics.com) ([Decentricity](http://github.com/Decentricity))
- Website go live, [www.degenics.com](http://degenics.com) ([Decentricity](http://github.com/Decentricity))
- IAM granted, accesses provided, roles defined ([Decentricity](http://github.com/Decentricity))
- UI/UX research: Vitagene, 23andme, Ancestry (Team)
- Storage research: IPFS / Torrent / IPFS+Torrent Research for Whole Genome Sequences (VCF files 1GB++) (Team)
- Payment research: [Transak](http://transak.com) Payment Gateway supported by Consensys (Team)

## Prototyping 2020/12/28 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Architectural decisions:**

- IPFS for storage layer, no Torrent required ([marcondol](http://github.com/marcondol) & ([dedy](http://github.com/aloisius82))
- Deploying on Ethereum testnet ([marcondol](http://github.com/marcondol) & ([dedy](http://github.com/aloisius82))
- Keypair derived from Ethereum keypair ([marcondol](http://github.com/marcondol) & ([dedy](http://github.com/aloisius82) & [kevinjanada](https://github.com/kevinjanada))
- Simple initial UI/UX ([kevinjanada](https://github.com/kevinjanada))
- Consortium / Private Deployment ([Decentricity](http://github.com/Decentricity))
- Marketplace ([Decentricity](http://github.com/Decentricity))
- Smart Contract expires if delivery not done within x days (Agent J, contributor)
- Structure: Nation>City>Lab>GenProduct ([ybobby](http://github.com/ybobby))

**Development**

- Workflow:
    ![/media/20201228Workflow.png](https://github.com/Degenics/degenics-public/blob/main/media/20201228Workflow.png) 
    ([ybobby](http://github.com/ybobby),[marcondol](http://github.com/marcondol) & [dedy](http://github.com/aloisius82))
- Encryption using ethereum address. ([kevinjanada](https://github.com/kevinjanada))
- IPFS connected with encryption, upload / download ability implemented. ([marcondol](http://github.com/marcondol)) 
- UX/UI initialized, keypair & mnemonic process initialized, dashboard initialized. ([kevinjanada](https://github.com/kevinjanada)) Demo is at [/media/20201228UIUX.mkv](https://github.com/Degenics/degenics-public/blob/main/media/20201228UIUX.mkv).

**Revision / Expansion Requests**

- Dashboard expansion with product categories, lab selection, city selection, nation selection (See Workflow)
- Research deanonymizing mechanism (if user requests and provides consent, can print nonymized file)
- Research logistics process & sampling mechanism / UX
- UX tweaks (Jean-Daniel Gauthier, contributor)


## Prototyping 2021/1/4 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Development**

- User onboarding flow 60% implemented ([kevinjanada](https://github.com/kevinjanada)), including:
    - Keygen
    - Private key login
    - Import json keystore
    - Mnemonic login
- User onboarding 40% backlog:
    - Explore onboarding with metamask (see **performance notes**)
    - Anti-frustration features & instructions (when keygen, ensure user has written down key, etc)
    - Progress bars
- Userside core experience 50% implemented (Team), including:
    - Nation, city, lab selection
    - Product selection under labs
    - Payment interface
    - Download and decrypt results when done
- Userside core experience 50% backlog:
    - Payment interface (may use Metamask)
    - More product selections with descriptions (marketplace paradigm)
    - Notifications
    - Instruction page for sampling and sending
    - Template to put on printable envelope with code and lab address
    - Separate buttons to only download certain files (REPORT and/or GENOME type file selection)
- IPFS Upload / Download implemented 60%  ([marcondol](http://github.com/marcondol) & [dedy](http://github.com/aloisius82))
- IPFS backlog 40%:
    - Two flows for the files (one button for REPORT filetype, one button for GENOME filetype, with multiple files allowed for each)
- Labside 50% implemented (Team):
    - Lab can already input user code (anonymous)
    - Lab can already upload file encrypted with user public key
- Labside 50% backlog:
    - Notifications
    - Time / deadline warning to revert with results
    - Instructions for labside user
    - Progress bar


**Demo Video**
    [![Demovid](/media/DegenicsAlpha01.png)](https://www.youtube.com/watch?v=qTyi8Zg8W_A&)

**Platform/Performance Notes**
- Team will explore using metamask for a better user experience and performance optimization.
- (Added 2020/01/06) Team will explore using Polkadot

**UX Notes**
- General simplification required for next sprint
- User feedback and anti-frustration features (Jean-Daniel Gauthier, contributor)

(added 2020/01/06) **UX Notes, screenshots of Figma mockup with revisions for next sprint (Jean-Daniel Gauthier, contributor):**
    ![1](/media/DA01.gif)
    Screens: 
    - [1](/media/DA01-5.PNG)
    - [2](/media/DA01-4.PNG) 
    - [3](/media/DA01-3.PNG) 
    - [4](/media/DA01-2.PNG) 
    - [5](/media/DA01-1.PNG)  
    
    
## Prototyping 2021/1/14 [Unreleased](https://github.com/Degenics)
**Demo Video**
    [![Demovid](/media/DegenicsAlpha02.png)](https://drive.google.com/file/d/1TB9RJz_FCDe8vIvvc41j0s1LYC9Oc3Ka/view)
    
    
## Prototyping 2021/1/18 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Development**

- Front End
    - (2021/1/5) Use custom Wallet class for faster encrypt decrypt and wallet generation
    - (2021/1/7) Update login page: update login page design, add confirm password validation, gitignore local contract.json
    - (2021/1/8) Update receipt page design: add DNA sample sending instruction, add helper to format specimen number; Handle and show send payment error message 
    - (2021/1/9) Update request test page: fix the numbering in DNA sample sending instructions, resize selected product icon, set product selection limit, parse               additionalData from lab and services data, show lab address if any
    - (2021/1/12) Update user dashboard & user request test: set max view limit for order history and test result fix order history sorting, disabled unselected product card;  Update style: update style for order history and lab order list; Fix order history sorting at user dashboard
    - (2021/1/13) Deployment changes: Create multi stage docker compose and config nginx
    - (2021/1/14) Move to testnet: fix ethereum tx issue, fix send transaction when register speciment; Change IPFS connection; 
    - (2021/1/15) Fix authentication flow: add route guards to check if logged in, sdd route guards to check user role when app start, move load web3 and contracts to router so to be able to access; Refactor; Connect to web3 and setup contracts before app renders; Fix flow in lab: change upload to result and genome, fix finalize to new method, fix bug crash on lab order list
    - (2021/1/17) Update lab's dashboard: Modified lab's dashboard home datatable to show next actions, add Process Screen to process specimen, Receive -> Wetwork -> Encrypt Upload Files -> Send (Set specimen status to success) workflow
    - (2021/1/18) Create order detail and all result: create page for w all result, create page for order detail, link page to dashboard; Create result: create result parser, create download result, create download genome; Update success & reject flow: show reject alert after rejecting speciment, show success alert after set speciment status to success

- Smart Contract
    - (2021/1/6)  Add timestamp
    - (2021/1/9)  Add dummy services data
    - (2021/1/11) Add escrow reg
    - (2021/1/13) Update skin product to skin care
    
- Demo
    - https://drive.google.com/file/d/1Rk0AZ1qMIUMhtZ2M_BKcpeV_mHnPmFWF/view?usp=sharing
    
    
## Prototyping 2021/1/25 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Development**

- Front End
    - (2021/1/19) Update order detail page: refactor testResult component, add search feature to test result page, fix typos, refactor button component, refactor status chip component, add DegenicsLog contract to Vuex store; Update bug: change search by report, change public key to encrypt, change default rpc; Add breadcrumbs; Refactor page header
    - (2021/1/20) Update refund mechanism: Add refund policy explanation, handle refund if order exceeded max processing time, refactor components 
    - (2021/1/21) Update login mechanism as lab, show wallet balance 
    - (2021/1/22) Update dowload genome page: get genome files in download genome page, handle download genome files, clean up and rename routes and their components
   
- Smart Contract
    - No Updates

- Documentation
    - Testing Document: https://drive.google.com/file/d/1JnhPwm2861wyxrC5lNBQgZshQB90RN75/view?usp=sharing
    
- Demo
    - https://drive.google.com/file/d/11XT5nDsqMuiDcawVk_WVRP545zVYuUs_/view?usp=sharing
    
    
## Prototyping 2021/2/02 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Development**

- Front End
    - (2021/1/26) Add & Refresh Favicon; Bug hotfix (rejection not showing); Add login validation using private key; Fix typos; Display rejection reason in order history table and lab dashboard processing page
    - (2021/1/29) Update Lab Process Rule: Lab can now finalized order by uploading either genome or report, Update contract.json for new network; Update default RPC connection
    - (2021/2/02) Fix order history link
   
- Smart Contract
    - (2021/1/28) Update dummy data DNA with new icon and description
    
- Demo
    - Video: https://drive.google.com/file/d/1QpOIdyyvNO0AwF_Y82XMNSuIgpM4xQGg/view?usp=sharing
    - Created 5 new accounts: https://drive.google.com/file/d/1HzXtPtvCN2cuY41atwvvajova3pVjNjs/view?usp=sharing 
    
    
## Prototyping 2021/2/08 [Unreleased](https://github.com/Degenics)

### Full Changelog

**Development**

- Front End
    - (2021/2/03) Update specimen sending instruction: Create a page for DNA sample collection instructions, refactor Card component, create BulletPoint component, add createHref method to breadcrumbs for dynamic breadcrumb links with parameters; Fixing: change current logo with new logo, edit sending instructions, edit dna sample collection instructions, show product price in request test page, add tooltip to Orders with 'sending' status.
    - (2021/2/04) Hotfix: change product card column size on xl screens; Fixing: show DNA Sample collection requirements, get ether when login.
    - (2021/2/05) Adjust menu card height: add height parameter to MenuCard, set height to 120 to MenuCard at dashboard Home; Truncate Product Description Overflow: new contract, truncate long product description, add tooltip to show product description; Disable Reject button while uploading: watch if file manager is loading, disable send and reject button while file manager is loading.
    - (2021/2/08) Add recaptcha, change 'Buccal Swab' to 'Cotton Bud'.
   
- Smart Contract
    - No Updates
    
- Demo
    - Video: TBA
    

