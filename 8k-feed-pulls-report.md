# 8-K current-feed pulls: three daily snapshots, item tallies, changes and 40 non-routine filings read

Three timed EDGAR current-feed pulls, 198 / 197 / 200 unique 8-K filings, 20/20 spot-verified against source documents per pull, and 40 non-routine filings read in full (108 items).

## Job

- Job: "8-K current-feed pulls: three daily snapshots, item tallies, changes and 40 non-routine filings read"
- Intent: `70c3670d-db36-43e3-a827-18c0a02d9d13` | Escrow: `esc_1f37c3ce3e5e40bdb5cfd452`
- Seller: BOSS NERO (`did:key:z6Mkp8e8LK8VTwhHh1MVhXqU7fMcvPCzDDcm9pbP75B8Adm5`)
- Budget $9.00, winning bid $2.25 (25%), net $2.18
- Awarded 2026-11-16 10:25 UTC; earliest submit 2026-11-18 10:25 UTC; first-delivery deadline 2026-11-20 18:25 UTC
- Deliverables: this report (D1) + `8k-feed-pull1.csv` (D2) + `8k-feed-pull2.csv` (D3) + `8k-feed-pull3.csv` (D4)

## Pulls and platform timeline

Progress notes on the platform record (server time, verified live 2026-11-18):

| Note | Recorded (UTC) | Gap from previous | Rows | SHA-256 of CSV |
|---|---|---|---|---|
| Award received | 2026-11-16 10:27:56 | — | — | — |
| PULL 1 | 2026-11-16 10:37:23 | — | 198 | `3a6ea568ee72b242e44dae52e70701d8b3cecc68b7666e20c71c6ea0b1e37d4a` |
| PULL 2 | 2026-11-17 10:41:13 | 24h 03m 50s | 197 | `b8d472f4d16305a887c648b5818fa06ff8d58b3d813b4785d8bc4806d705fbac` |
| PULL 3 | 2026-11-18 10:42:08 | 24h 00m 55s | 200 | `a4efa96674902edda72032412cd8f1052db8313a2a99813f1191b6e4f98ad19a` |

Each PULL note is at least 24 hours after the previous one, and each carries the row count and the SHA-256 of its CSV. No pull failed and no pull was re-pulled; the Revision 1 cleanup of the company column in the attached CSV copies is declared separately in `CORRECTED PULL k:` notes (see Revision 1 corrections).

| Pull | Pulled (UTC) | Feed updated page 0 | Feed updated page 1 | HTTP Date page 0 | HTTP Date page 1 | Rows | Duplicates skipped |
|---|---|---|---|---|---|---|---|
| PULL 1 | 2026-11-16T10:32:56Z–2026-11-16T10:33:13Z | 2026-11-16T05:32:44-05:00 | 2026-11-16T05:33:03-05:00 | Mon, 16 Nov 2026 10:33:09 GMT | Mon, 16 Nov 2026 10:33:13 GMT | 198 | 2 |
| PULL 2 | 2026-11-17T10:40:43Z–2026-11-17T10:40:49Z | 2026-11-17T05:40:45-05:00 | 2026-11-17T05:40:49-05:00 | Tue, 17 Nov 2026 10:40:45 GMT | Tue, 17 Nov 2026 10:40:49 GMT | 197 | 3 |
| PULL 3 | 2026-11-18T10:41:45Z–2026-11-18T10:41:51Z | 2026-11-18T05:41:48-05:00 | 2026-11-18T05:41:51-05:00 | Wed, 18 Nov 2026 10:41:48 GMT | Wed, 18 Nov 2026 10:41:51 GMT | 200 | 0 |

Source times increase strictly from pull to pull. The feed is rolling: the two pages of a pull already differ by seconds, so each snapshot is judged from its own excerpt (feed `updated` line + CSV row count), as the brief provides.

## Item tallies (recomputed from the final CSVs)

### PULL 1 — 198 unique accessions, 0 with no items

| Item | Count |
|---|---:|
| 1.01 | 26 |
| 1.02 | 4 |
| 1.03 | 1 |
| 2.01 | 1 |
| 2.02 | 48 |
| 2.03 | 17 |
| 2.04 | 1 |
| 3.01 | 11 |
| 3.02 | 9 |
| 3.03 | 7 |
| 4.01 | 1 |
| 4.02 | 3 |
| 5.01 | 1 |
| 5.02 | 45 |
| 5.03 | 8 |
| 5.07 | 11 |
| 5.08 | 1 |
| 7.01 | 29 |
| 8.01 | 50 |
| 9.01 | 132 |

First accession `0001125345-26-000077`, last accession `0001628280-26-073758`.

### PULL 2 — 197 unique accessions, 0 with no items

| Item | Count |
|---|---:|
| 1.01 | 21 |
| 1.02 | 3 |
| 2.01 | 4 |
| 2.02 | 64 |
| 2.03 | 12 |
| 2.05 | 1 |
| 3.01 | 3 |
| 3.02 | 8 |
| 3.03 | 3 |
| 4.01 | 1 |
| 4.02 | 3 |
| 5.02 | 29 |
| 5.03 | 5 |
| 5.07 | 9 |
| 7.01 | 66 |
| 8.01 | 37 |
| 9.01 | 162 |

First accession `0001104659-26-128592`, last accession `0001539497-26-002999`.

### PULL 3 — 200 unique accessions, 0 with no items

| Item | Count |
|---|---:|
| 1.01 | 29 |
| 1.02 | 3 |
| 2.01 | 4 |
| 2.02 | 30 |
| 2.03 | 21 |
| 2.04 | 1 |
| 2.05 | 1 |
| 3.01 | 6 |
| 3.02 | 8 |
| 3.03 | 5 |
| 4.01 | 5 |
| 5.01 | 2 |
| 5.02 | 39 |
| 5.03 | 12 |
| 5.07 | 8 |
| 7.01 | 57 |
| 8.01 | 51 |
| 9.01 | 150 |

First accession `0001104659-26-129167`, last accession `0001901440-26-000037`.

## Review: 40 non-routine filings (from PULL 1, in feed order)

Selection rule: the first 40 unique accessions in PULL 1 feed order whose items include at least one item other than 7.01, 8.01, 9.01. All 40 are complete; parsed item codes match the feed for all 40. One line per item: a summary in our own words of the sentence(s) under that item's heading in the filing document (all 108 summaries rewritten in our own words for Revision 1; the PROOF section below quotes each heading with the complete first sentence(s) verbatim).

| # | Accession | Company | CIK | Form | Document path | Items (one-line summary each) |
|---|---|---|---|---|---|---|
| 1 | `0001213900-26-119916` | Tempest Therapeutics, Inc. | 0001544227 | 8-K | `/Archives/edgar/data/1544227/000121390026119916/ea0312157-8k_tempest.htm` | **2.02** Results of Operations and Financial Condition. — Tempest Therapeutics issued a press release on November 13, 2026 announcing its financial results for the quarter ended September 30, 2026 and other business highlights.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release dated November 13, 2026 (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 2 | `0001171843-26-007431` | BeyondSpring Inc. | 0001677940 | 8-K | `/Archives/edgar/data/1677940/000117184326007431/f8k_111326.htm` | **2.02** Results of Operations and Financial Condition. — BeyondSpring issued a press release announcing its financial results for the quarter ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release dated November 13, 2026 (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 3 | `0001193125-26-461047` | BCP Investment Corp | 0001372807 | 8-K | `/Archives/edgar/data/1372807/000119312526461047/d520705d8k.htm` | **2.02** Results of Operations and Financial Condition. — BCP Investment Corporation furnished a press release announcing its financial results for the fiscal quarter ended September 30, 2026, plus a supplemental investor presentation dated November 12, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the earnings press release (99.1), the investor presentation (99.2), and the cover-page interactive data file (104). |
| 4 | `0001140361-26-043831` | CareTrust REIT, Inc. | 0001590717 | 8-K | `/Archives/edgar/data/1590717/000114036126043831/ny20085288x3_8k.htm` | **1.01** Entry into a Material Definitive Agreement — CareTrust REIT signed forward sale agreements with Bank of America and Morgan Stanley on November 11, 2026 covering 17,000,000 shares of common stock, and additional agreements on November 12 covering a further 2,550,000 shares.<br>**8.01** Other Events — CareTrust and its operating partnership signed the underwriting agreement for the registered offering of the 17,000,000 shares; the underwriters exercised their option for the extra 2,550,000 shares in full, and the forward purchasers borrowed and sold all 19,550,000 shares to the underwriters on November 13, 2026.<br>**9.01** Financial Statements and Exhibits — Lists the exhibits: the underwriting agreement (1.1), the DLA Piper opinion (5.1) and consent (23.1), forward confirmations (10.1-10.4), and the cover-page interactive data file (104). |
| 5 | `0001493152-26-051858` | MANGOCEUTICALS, INC. | 0001938046 | 8-K | `/Archives/edgar/data/1938046/000149315226051858/form8-k.htm` | **3.03** Material Modification to Rights of Security Holders. — Incorporates Item 5.03: the Series B and Series C designation amendments and the new Series D designation took effect November 9, 2026; the Series D stock will rank senior to the common stock for dividends and liquidation, though no Series D shares were issued by the filings themselves.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — Mangoceuticals filed Texas certificates of amendment on November 9, 2026 (board-approved November 4) amending the designations of its Series B and 6% Series C convertible preferred stock - chiefly to approve the new Series D designation and its transactions and waive conflicting Series B/C restrictions - and establishing the Series D preferred stock.<br>**5.07** Submission of Matters to a Vote of Security Holders. — The holder of all 980,000 outstanding Series C shares approved the Series C amendment and the Series D designation by written consent on November 6, 2026, including a proposed Regulation A sale of up to 1,000,000 Series D shares at $10.00 per share; there were no votes against or abstentions.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the Series B amendment (3.1), the Series C amendment (3.2), the 8% Series D certificate of designations (3.3), and the cover-page interactive data file (104). |
| 6 | `0001193125-26-461028` | Western Union CO | 0001365135 | 8-K | `/Archives/edgar/data/1365135/000119312526461028/d152329d8k.htm` | **1.02** Termination of a Material Definitive Agreement. — Western Union's 2024 delayed-draw term loan agreement will terminate when the loan under it is repaid, expected on or about November 17, 2026, with no material early-termination penalties.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — Western Union borrowed the full $800 million committed amount under its January 2026 delayed-draw term loan facility on November 10, 2026 and intends to use the proceeds to repay in full the $800 million outstanding under the 2024 term loan agreement, which matures in December 2027. |
| 7 | `0001193125-26-461027` | 3D SYSTEMS CORP | 0000910638 | 8-K | `/Archives/edgar/data/910638/000119312526461027/d533328d8k.htm` | **1.01** Entry into a Material Definitive Agreement. — 3D Systems exchanged all of its outstanding 5.875% convertible notes due 2030 on November 12, 2026 for $85 million of new 3.30% convertible notes due 2031, $20 million in cash plus accrued interest, and 13,471,138 shares of common stock, under exchange agreements signed November 4 with all of the 2030 noteholders.<br>**1.02** Termination of a Material Definitive Agreement. — After the exchange, 3D Systems had all outstanding 2030 notes cancelled on November 12, 2026, so the 2030 notes indenture was satisfied and discharged and the related guarantees and collateral liens were released.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — Cross-references Item 1.01: the new $85 million of 3.30% convertible notes due 2031 are a direct financial obligation.<br>**3.02** Unregistered Sales of Equity Securities. — Cross-references Item 1.01 for the shares and notes issued in the exchange, and reports 1,464,206 shares issued to J. Wood Capital Advisors LLC on November 12, 2026 as payment for services, with no cash proceeds, under the Section 4(a)(2) exemption.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the 2031 notes indenture (4.1), the form of 3.30% note due 2031 (4.2), and the cover-page interactive data file (104). |
| 8 | `0001140361-26-043829` | Navient Holdings, Inc. | 0002152623 | 8-K | `/Archives/edgar/data/2152623/000114036126043829/ef20085597_8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Navient director Frederick Arnold told the company on November 11, 2026 that he was voluntarily retiring from the board effective immediately; his decision was not the result of any disagreement with the company. |
| 9 | `0001493152-26-051849` | Polomar Health Services, Inc. | 0001265521 | 8-K | `/Archives/edgar/data/1265521/000149315226051849/form8-k.htm` | **1.01** Entry Into a Material Definitive Agreement. — Incorporates Item 2.03: the $450,000 promissory note and loan agreement with Island 40 Group, LLC is the material definitive agreement reported.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation. — Polomar signed a $450,000 promissory note and loan agreement with Island 40 Group, LLC effective November 9, 2026, covering placement commissions owed under their sales director and distribution agreement; its pharmacy subsidiary guarantees the note, which bears interest at 10% through 2026 and then at the WSJ prime rate plus 4%, and matures March 31, 2027.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the promissory note and loan agreement (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 10 | `0001193125-26-461016` | IonQ, Inc. | 0001824920 | 8-K | `/Archives/edgar/data/1824920/000119312526461016/ionq-20261110.htm` | **3.02** Unregistered Sales of Equity Securities. — IonQ filed a prospectus supplement on November 13, 2026 under its Form S-3ASR shelf covering the resale by selling stockholders of up to 34,580,646 shares of common stock.<br>**5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — IonQ appointed Gary Merrill - previously Commvault's chief financial officer - as CFO, Treasurer and principal financial and accounting officer on November 10, 2026, effective his expected start date of December 3, 2026; he succeeds Inder M. Singh, and Niccolo M. de Masi serves as interim principal financial and accounting officer until Merrill starts.<br>**8.01** Other Events. — IonQ announced on November 13, 2026 that Thomas A. Austin, previously Juniper Networks' chief accounting officer, was appointed its Chief Accounting Officer effective November 16, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the Paul, Weiss opinion (5.1) and consent (23.1), the press release (99.1), and the cover-page interactive data file (104). |
| 11 | `0001193125-26-461010` | Dolby Laboratories, Inc. | 0001308547 | 8-K | `/Archives/edgar/data/1308547/000119312526461010/d101237d8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Dolby's compensation committee adopted the 2027 Dolby Executive Bonus Plan on November 10, 2026; CEO Marc Whitten's target bonus is 100% of base salary and his fiscal 2027 bonus will be paid at 100% of target, while other officers' bonuses hinge on non-GAAP operating income, revenue and other goals set by the committee. |
| 12 | `0001640334-26-001797` | Panamera Holdings Corp | 0001620749 | 8-K | `/Archives/edgar/data/1620749/000164033426001797/pnht_8k.htm` | **4.02** Non-Reliance on Previously Issued Financial Statements or a Related Audit Report or Interim Review — Panamera said that, following its October 26, 2026 disclosure of an unreported employment agreement and a resulting unreported lawsuit, it is restating the affected periods through an amendment to its annual report on Form 10-K for the fiscal year ended July 31, 2025, and that its audit committee discussed the matters with its independent registered public accounting firm. |
| 13 | `0001493152-26-051841` | Cingulate Inc. | 0001862150 | 8-K | `/Archives/edgar/data/1862150/000149315226051841/form8-k.htm` | **1.01** Entry into Material Definitive Agreement — Cingulate amended its at-the-market sales agreement on November 13, 2026 to add Maxim Group LLC as a sales agent alongside A.G.P./Alliance Global Partners, under which the company may sell up to $100 million of common stock from time to time.<br>**2.02** Results of Operations and Financial Condition. — Cingulate issued a press release announcing its financial results for the quarter ended September 30, 2026 and providing a regulatory update.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the ATM agreement amendment (Exhibit 10.1), the press release (Exhibit 99.1), and the cover-page interactive data file (Exhibit 104). |
| 14 | `0001493152-26-051839` | Flux Power Holdings, Inc. | 0001083743 | 8-K | `/Archives/edgar/data/1083743/000149315226051839/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — Flux Power's lender, Gibraltar Business Capital, agreed by letter dated November 13, 2026 (effective November 6) to extend the deadline for the company's required $4.0 million equity raise under its loan and security agreement from November 6 to December 4, 2026; all other loan terms are unchanged.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — Cross-references Item 1.01 for the direct-financial-obligation information.<br>**3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — Nasdaq notified Flux Power on November 9, 2026 that its stockholders' deficit of $431,000 puts it below the $2.5 million minimum stockholders' equity required for continued listing on the Nasdaq Capital Market; the company has until December 24, 2026 to submit a plan to regain compliance.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the lender letter agreement (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 15 | `0001104659-26-127233` | Versa Bancorp | 0002100848 | 8-K12B | `/Archives/edgar/data/2100848/000110465926127233/tm2629642d1_8k12b.htm` | **1.01** Entry into a Material Definitive Agreement. — Incorporates the introductory note on the completed reorganization, and adds that on completion Versa Bancorp entered into indemnification agreements with each of its directors and executive officers.<br>**2.01** Completion of Acquisition or Disposition of Assets. — Incorporates the introductory note describing completion of the reorganization under which Versa Bancorp became the parent company of VersaBank.<br>**3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — Incorporates the introductory note for the listing information connected with the reorganization.<br>**3.03** Material Modification to Rights of Security Holders. — Incorporates the introductory note and Item 5.03, and explains that Versa Bancorp is governed by Delaware corporate law rather than the Canadian Bank Act regime that governed VersaBank, with the material differences described in the registration statement.<br>**5.01** Changes in Control of Registrant. — Incorporates the introductory note for the change-of-control information arising from the reorganization.<br>**5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Director Patrick DeLacey resigned from the board on November 9, 2026, not over any disagreement; the board was reduced from eight to seven directors, Scott Verity became audit committee chair, and Barbara Chaffee joined the audit committee.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — Versa Bancorp amended its certificate of incorporation on November 12, 2026 to increase authorized shares to 350,000,000 and to provide indemnification for officers and directors, and adopted new bylaws, in anticipation of the reorganization.<br>**7.01** Regulation FD Disclosure. — Versa Bancorp issued a press release on November 13, 2026 announcing completion of the reorganization.<br>**9.01** Financial Statements and Exhibits. — Attaches VersaBank's audited consolidated financial statements for fiscal 2025 and 2024 and unaudited statements for the nine months ended July 31, 2026 and 2025 as exhibits, and lists the amended charter (3.1), bylaws (3.2), form of indemnification agreement (10.1), incentive plan (10.2), press release (99.1), and cover-page data file (104). |
| 16 | `0001104659-26-127230` | Datavault AI Inc. | 0001682149 | 8-K | `/Archives/edgar/data/1682149/000110465926127230/tm2629197d1_8k.htm` | **3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — Nasdaq told Datavault AI on November 10, 2026 that its common stock is subject to delisting for failing the $1.00 minimum bid price rule, and that trading will be suspended from November 17, 2026 because the stock closed below $0.10 for ten consecutive business days; the company plans to request a hearings-panel review and expects the shares to trade on OTC Markets under DVLT meanwhile.<br>**8.01** Other Events. — Datavault issued a press release on November 13, 2026 announcing the Nasdaq delisting letter and the trading suspension.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 17 | `0001878897-26-000055` | Douglas Elliman Inc. | 0001878897 | 8-K | `/Archives/edgar/data/1878897/000187889726000055/doug-20261113.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers — Douglas Elliman and its Executive Vice President, Treasurer and CFO James B. Kirkland III mutually agreed that he will retire effective November 13, 2026; his separation agreement pays one year of his $650,000 base salary, a $369,253 pro-rated 2026 bonus, a $150,000 retention payment, accelerated vesting of 447,708 restricted shares, and $40,000 for unused vacation. |
| 18 | `0001104659-26-127228` | CHEETAH NET SUPPLY CHAIN SERVICE INC. | 0001951667 | 8-K | `/Archives/edgar/data/1951667/000110465926127228/tm2629774d1_8k.htm` | **2.02** Results of Operations and Financial Condition — Cheetah Net issued a press release announcing its financial results for the third quarter of 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 19 | `0001493152-26-051834` | AIRWA INC. | 0001674440 | 8-K | `/Archives/edgar/data/1674440/000149315226051834/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — AiRWA signed securities purchase agreements on November 9, 2026 to sell 1,800,000 shares of common stock to investors at $0.8332 per share - about $1.5 million gross - in a private placement expected to close around November 17, 2026, with proceeds for working capital and general corporate purposes.<br>**3.02** Unregistered Sales of Equity Securities. — Cross-references Item 1.01 for the unregistered sale of the 1,800,000 shares.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the form of securities purchase agreement (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 20 | `0001437749-26-036953` | AZIO AI HOLDINGS, INC. | 0001563568 | 8-K | `/Archives/edgar/data/1563568/000143774926036953/adom20261113_8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Azio AI stockholders approved the company's 2026 Equity Incentive Plan at the annual meeting on November 13, 2026, so the plan took effect immediately.<br>**5.07** Submission of Matters to a Vote of Security Holders. — At Azio's reconvened annual meeting on November 13, 2026 (adjourned from November 2 for lack of quorum), holders of 54.2% of the shares were represented and proposals 1, 2, 3, 5, 6 and 7 were approved; only proposal 4 - approval of shares issuable on conversion of the Series A preferred stock - was adjourned to December 4, 2026 because Nasdaq has not yet approved the company's listing application. |
| 21 | `0001493152-26-051832` | Where Food Comes From, Inc. | 0001360565 | 8-K | `/Archives/edgar/data/1360565/000149315226051832/form8-k.htm` | **2.02** Results of Operations and Financial Condition Reference — Points readers to the company's November 12, 2026 press release and conference-call transcript for its financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits (d) — Lists the exhibits: the press release (99.1), the conference-call transcript (99.2), and the cover-page interactive data file (104). |
| 22 | `0001104659-26-127223` | Booking Holdings Inc. | 0001075531 | 8-K | `/Archives/edgar/data/1075531/000110465926127223/tm2629703d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — Booking Holdings issued senior notes on November 13, 2026 under its 2017 indenture - €1.25 billion of 3.950% notes due 2029, €800 million of 4.375% notes due 2032, €750 million of 4.750% notes due 2035 and €750 million of 5.000% notes due 2038 - documented through four officers' certificates.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation Under an Off-Balance Sheet Arrangement of the Registrant. — Incorporates Item 1.01: the senior-note issuance creates a direct financial obligation.<br>**8.01** Other Events. — Booking Holdings signed an underwriting agreement on November 9, 2026 with Banco Santander, BNP Paribas, Deutsche Bank, Goldman Sachs and HSBC as underwriters' representatives for the registered public offering of the €3.55 billion of senior notes.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the underwriting agreement (1.1), forms of the senior notes (4.1-4.4), the officers' certificates (4.5-4.8), the agency agreement (4.9), the Cravath opinion (5.1) and consent (23.1), and the cover-page interactive data file (104). |
| 23 | `0001193125-26-460951` | BEASLEY BROADCAST GROUP INC | 0001099160 | 8-K | `/Archives/edgar/data/1099160/000119312526460951/bbgi-20261113.htm` | **2.02** Results of Operations and Financial Condition. — Beasley Broadcast Group issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 24 | `0001213900-26-119857` | Health In Tech, Inc. | 0002019505 | 8-K | `/Archives/edgar/data/2019505/000121390026119857/ea0311991-8k_health.htm` | **2.02** Results of Operations and Financial Condition. — Health In Tech issued a press release on November 12, 2026 announcing its results of operations for the quarter ended September 30, 2026.<br>**7.01** Regulation FD Disclosure. — Repeats the Item 2.02 disclosure - the November 12, 2026 press release with results for the quarter ended September 30, 2026 - under Regulation FD.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 25 | `0000877860-26-000230` | NATIONAL HEALTH INVESTORS INC | 0000877860 | 8-K | `/Archives/edgar/data/877860/000087786026000230/nhi-20261109.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — National Health Investors entered into indemnification agreements on November 9, 2026 with each of its directors and certain officers, including all executive officers, obligating the company to indemnify them to the maximum extent permitted by Maryland law.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the form of indemnification agreement (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 26 | `0001628280-26-073911` | DocGo Inc. | 0001822359 | 8-K | `/Archives/edgar/data/1822359/000162828026073911/dcgo-20261113.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — DocGo and CEO Lee Bienstock signed a transition services and separation agreement on November 13, 2026: with his employment agreement expiring December 31, 2026 and a CEO search under way, he will stay on as CEO through a transition period running January 1 to March 31, 2027 (then serve as senior advisor if a successor starts sooner), for $90,000 per month plus specified equity vesting and his 2026 bonus.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the transition services and separation agreement with Lee Bienstock (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 27 | `0001437749-26-036943` | ACCURAY INC | 0001138723 | 8-K | `/Archives/edgar/data/1138723/000143774926036943/aray20261111_8k.htm` | **3.02** Unregistered Sales of Equity Securities. — Incorporates Item 3.03 on the Series A preferred stock, which was sold in a private placement to accredited investors in reliance on the Section 4(a)(2) exemption.<br>**3.03** Material Modification to Rights of Security Holders. — Accuray closed the sale of 55,000 shares of Series A convertible preferred stock for $55.0 million - $15.0 million in cash plus conversion of $40.0 million of existing investor debt - and filed the certificate of designations on November 12, 2026; the shares were issued November 13, carry an 8% preferential dividend, and rank senior to the common stock.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — Accuray filed two charter amendments on November 6, 2026 - one raising authorized common shares from 200 million to 400 million and one effecting a 1-for-40 reverse stock split - both effective November 9, 2026, when the stock began trading split-adjusted under ARAY with a new CUSIP.<br>**7.01** Regulation FD Disclosure — Accuray disclosed that warrants held by the investors to buy about 27.6 million pre-split shares were automatically cancelled at the financing closing, and that it issued a press release on November 13, 2026 about the share increase, reverse split and preferred stock issuance.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the Series A certificate of designations (3.1), the authorized-share-increase amendment (3.2), the reverse-split amendment (3.3), the press release (99.1), and the cover-page interactive data file (104). |
| 28 | `0001104659-26-127202` | Contango Silver & Gold Inc. | 0001502377 | 8-K | `/Archives/edgar/data/1502377/000110465926127202/tm2629486d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — Contango Silver & Gold signed an at-the-market sales agreement on November 13, 2026 with Cantor Fitzgerald as lead agent and co-agents, under which it may offer and sell up to $75 million of common stock from time to time, paying the agents a commission of up to 3% of gross proceeds.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the sales agreement (1.1), the Cozen O'Connor opinion (5.1) and consent (23.1), and the cover-page interactive data file (104). |
| 29 | `0001213900-26-119843` | SOUNDHOUND AI, INC. | 0001840856 | 8-K | `/Archives/edgar/data/1840856/000121390026119843/ea0312272-8k_sound.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Tyler Moore became SoundHound's principal accounting officer effective November 9, 2026, succeeding CFO John Collins in that role while Collins continues as CFO and principal financial officer; Moore, hired November 2, 2026 as Executive Vice President and Chief Accounting Officer, receives a $345,000 base salary, a bonus target of up to 40% of salary, and 100,000 RSUs vesting monthly over four years.<br>**9.01** Financial Statement and Exhibits. Exhibit Number — Lists the exhibits: the cover-page interactive data file (Exhibit 104) only. |
| 30 | `0001493152-26-051809` | NextBoat Inc. | 0002067767 | 8-K | `/Archives/edgar/data/2067767/000149315226051809/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — NextBoat's subsidiary Off The Hook Yacht Sales NC signed a seven-year triple-net lease (guaranteed by NextBoat) with Hadley Harbor Group on November 4, 2026 for 22 boat slips at Cape Fear Marina in Wilmington, North Carolina, at $8,950 per month rising 3% a year; the landlord is controlled by director Zebulon Z. Hadley IV and bought the slips from chairman Jason Ruegg's entity, a related-party deal approved by the disinterested audit-committee members.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — Cross-references Item 1.01: the guaranteed marina-slip lease is a direct financial obligation.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the marina lease, including NextBoat's guaranty (Exhibit 10.1), and the cover-page interactive data file (Exhibit 104). |
| 31 | `0001493152-26-051811` | Co-Diagnostics, Inc. | 0001692415 | 8-K | `/Archives/edgar/data/1692415/000149315226051811/form8-k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — At a court-ordered special meeting on November 13, 2026, Co-Diagnostics shareholders approved Amendment No. 1 to the company's 2025 Equity Incentive Plan, adding 2,000,000 shares to the plan reserve for a maximum of 2,223,333 shares (the same cap applies to incentive stock options).<br>**5.07** Submission of Matters to a Vote of Security Holders — Co-Diagnostics' special meeting on November 13, 2026 elected Dwight Egan, Eugene Durenard, Richard Serbin, James Nelson and Edward Murphy as directors for one-year terms and adopted the proposals to enlarge the equity-plan reserve, approve executive compensation on an advisory basis, and ratify Tanner LLC as independent auditor for 2026, among the matters voted on.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: Amendment No. 1 to the 2025 Equity Incentive Plan (Exhibit 10.1) and the cover-page interactive data file (Exhibit 104). |
| 32 | `0001493152-26-051810` | Beyond Air, Inc. | 0001641631 | 8-K | `/Archives/edgar/data/1641631/000149315226051810/form8-k.htm` | **2.02** Results of Operations and Financial Condition. — Beyond Air issued a press release on November 11, 2026 announcing its financial results for the fiscal quarter ended September 30, 2026 and recent corporate developments.<br>**7.01** Regulation FD Disclosure. — Incorporates the Item 2.02 information - the November 11, 2026 results press release - under Regulation FD.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 33 | `0001493152-26-051808` | Q/C TECHNOLOGIES, INC. | 0001321834 | 8-K | `/Archives/edgar/data/1321834/000149315226051808/form8-k.htm` | **3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — Nasdaq notified Q/C Technologies on November 6, 2026 that, with its closing bid price below $1.00 for the 30 consecutive business days from September 25 to November 5, 2026, it no longer meets the minimum bid price rule; the company has a 180-day compliance period, until May 5, 2027, to regain compliance and is evaluating options including a possible reverse stock split. |
| 34 | `0001213900-26-119839` | BRC Group Holdings, Inc. | 0001464790 | 8-K | `/Archives/edgar/data/1464790/000121390026119839/ea0312286-8k_brcgroup.htm` | **5.02** (b) Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — BRC Group will eliminate the Chief Accounting Officer role effective November 16, 2026 because it does not consider the separate role necessary; Howard Weitzman will step down as Chief Accounting Officer, remain with the company as Head of Corporate Tax, and cease to be an executive officer and Section 16 officer. |
| 35 | `0001493152-26-051806` | Evofem Biosciences, Inc. | 0001618835 | 8-K | `/Archives/edgar/data/1618835/000149315226051806/form8-k.htm` | **2.02** Results of Operations and Financial Condition. — Evofem issued a press release announcing its financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 36 | `0001193125-26-460888` | Seritage Growth Properties | 0001628063 | 8-K | `/Archives/edgar/data/1628063/000119312526460888/srg-20261113.htm` | **2.02** Results of Operations and Financial Condition. — Seritage Growth Properties issued a press release regarding its financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 37 | `0001193125-26-460887` | CERENOME, INC. | 0001095981 | 8-K | `/Archives/edgar/data/1095981/000119312526460887/cnsy-20261113.htm` | **2.02** Results of Operations and Financial Condition. — Cerenome reported its financial results for the third quarter ended September 30, 2026, together with other recent corporate updates, in a press release.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release announcing financial results dated November 13, 2026 (Exhibit 99.1) and the cover-page interactive data file (Exhibit 104). |
| 38 | `0001193125-26-460879` | Apollo Global Management, Inc. | 0001858681 | 8-K | `/Archives/edgar/data/1858681/000119312526460879/d143669d8k.htm` | **1.01** Entry into a Material Definitive Agreement. — Apollo Global Management issued $600 million of 7.550% fixed-rate resettable junior subordinated notes due 2056 on November 13, 2026 in an underwritten public offering; interest is fixed until the first reset date of December 15, 2036 and thereafter floats at the five-year U.S. Treasury rate plus 2.672%, and the proceeds are earmarked for general corporate purposes including funding the announced investment in Mubadala Capital.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — Cross-references Item 1.01: the $600 million junior subordinated notes are a direct financial obligation.<br>**8.01** Other Events. — Cross-references Item 1.01 and adds the underwriting agreement dated November 9, 2026 with J.P. Morgan, BofA Securities, Morgan Stanley and Wells Fargo as representatives, and the Paul, Weiss opinion on the validity of the notes and guarantees.<br>**9.01** Financial Statements and Exhibits. — Incorporates the exhibits into the registration statement and lists them: the underwriting agreement (1.1), the indenture (4.1), the form of note (4.2), the Paul, Weiss opinion (5.1) and consent (23.1), and the cover-page interactive data file (104). |
| 39 | `0001628280-26-073897` | American Strategic Investment Co. | 0001595527 | 8-K | `/Archives/edgar/data/1595527/000162828026073897/nycr-20261113.htm` | **2.02** Results of Operations and Financial Condition. — American Strategic Investment issued a press release on November 13, 2026 announcing its results of operations for the quarter ended September 30, 2026 and supplemental financial information for the same quarter.<br>**7.01** Regulation FD Disclosure. — Repeats the Item 2.02 disclosure - the November 13, 2026 press release and supplemental information - under Regulation FD.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the press release (99.1), the supplemental information for the quarter ended September 30, 2026 (99.2), and the cover-page interactive data file (104). |
| 40 | `0001104659-26-127163` | QUALCOMM INC/DE | 0000804328 | 8-K | `/Archives/edgar/data/804328/000110465926127163/tm2629667d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — QUALCOMM sold senior notes on November 12, 2026 under its 2015 indenture through an officers' certificate: $750 million of 5.000% notes due 2028, $750 million of 5.150% notes due 2029, $1.0 billion of 5.350% notes due 2031, $750 million of 5.600% notes due 2033, and $750 million of 5.800% notes due 2036.<br>**8.01** Other Events. — QUALCOMM signed an underwriting agreement on November 9, 2026 with BNP Paribas, BofA Securities, Deutsche Bank, J.P. Morgan and Morgan Stanley, as representatives of the underwriters, for the registered public offering of the notes under its Form S-3 shelf registration statement.<br>**9.01** Financial Statements and Exhibits. — Lists the exhibits: the underwriting agreement (1.1), the 2015 indenture (4.1), the officers' certificate (4.2), forms of the series of notes (4.3-4.7), the Sidley Austin opinion (5.1), and the cover-page interactive data file (104). |

Revision 1 note: no summary above is a verbatim copy, a fragment cut at an abbreviation, or a truncated capture; the three summaries that were cut at the old 900-character capture cap in the first submission (Booking Holdings 1.01 and 9.01, QUALCOMM 1.01) are rewritten like all the others, and their PROOF excerpts below are complete.

## PROOF — feed requests

Every request: host `www.sec.gov`, endpoint `/cgi-bin/browse-edgar`, parameters `action=getcurrent`, `type=8-K`, `owner=include`, `count=100`, `output=atom`, `start=0` or `start=100`. User-Agent: `BOSS-NERO research/1.0 (contact: fadliar010817@gmail.com)`. Each page below quotes its raw `<updated>` line verbatim and its first and last entries; the attached CSVs contain every entry.

### PULL 1

Page `start=0` — requested 2026-11-16T10:32:56Z, responded 2026-11-16T10:33:08Z, HTTP 200, Date header `Mon, 16 Nov 2026 10:33:09 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-16T05:32:44-05:00</updated>`

First entry: `8-K - MACROGENICS INC (0001125345) (Filer)` — updated `2026-11-13T17:28:39-05:00` — <https://www.sec.gov/Archives/edgar/data/1125345/000112534526000077/0001125345-26-000077-index.htm>

Last entry: `8-K/A - NIQ Global Intelligence plc (0002054696) (Filer)` — updated `2026-11-13T16:29:35-05:00` — <https://www.sec.gov/Archives/edgar/data/2054696/000205469626000030/0002054696-26-000030-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - MACROGENICS INC (0001125345) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1125345/000112534526000077/0001125345-26-000077-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-13 &lt;b&gt;AccNo:&lt;/b&gt; 0001125345-26-000077 &lt;b&gt;Size:&lt;/b&gt; 6 MB
&lt;br&gt;Item 7.01: Regulation FD Disclosure
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-13T17:28:39-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001125345-26-000077</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K/A - NIQ Global Intelligence plc (0002054696) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/2054696/000205469626000030/0002054696-26-000030-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-13 &lt;b&gt;AccNo:&lt;/b&gt; 0002054696-26-000030 &lt;b&gt;Size:&lt;/b&gt; 4 MB
&lt;br&gt;Item 2.02: Results of Operations and Financial Condition
</summary>
<updated>2026-11-13T16:29:35-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K/A"/>
<id>urn:tag:sec.gov,2008:accession-number=0002054696-26-000030</id>
</entry>
```

Page `start=100` — requested 2026-11-16T10:33:09Z, responded 2026-11-16T10:33:12Z, HTTP 200, Date header `Mon, 16 Nov 2026 10:33:13 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-16T05:33:03-05:00</updated>`

First entry: `8-K - PharmaCyte Biotech, Inc. (0001157075) (Filer)` — updated `2026-11-13T16:28:19-05:00` — <https://www.sec.gov/Archives/edgar/data/1157075/000168316826008705/0001683168-26-008705-index.htm>

Last entry: `8-K - AAON, INC. (0000824142) (Filer)` — updated `2026-11-13T15:16:30-05:00` — <https://www.sec.gov/Archives/edgar/data/824142/000162828026073758/0001628280-26-073758-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - PharmaCyte Biotech, Inc. (0001157075) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1157075/000168316826008705/0001683168-26-008705-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-13 &lt;b&gt;AccNo:&lt;/b&gt; 0001683168-26-008705 &lt;b&gt;Size:&lt;/b&gt; 219 KB
&lt;br&gt;Item 3.03: Material Modifications to Rights of Security Holders
&lt;br&gt;Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
&lt;br&gt;Item 8.01: Other Events
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-13T16:28:19-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001683168-26-008705</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - AAON, INC. (0000824142) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/824142/000162828026073758/0001628280-26-073758-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-13 &lt;b&gt;AccNo:&lt;/b&gt; 0001628280-26-073758 &lt;b&gt;Size:&lt;/b&gt; 2 MB
&lt;br&gt;Item 1.01: Entry into a Material Definitive Agreement
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-13T15:16:30-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001628280-26-073758</id>
</entry>
```

### PULL 2

Page `start=0` — requested 2026-11-17T10:40:43Z, responded 2026-11-17T10:40:45Z, HTTP 200, Date header `Tue, 17 Nov 2026 10:40:45 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-17T05:40:45-05:00</updated>`

First entry: `8-K - Envela Corp (0000701719) (Filer)` — updated `2026-11-16T17:31:11-05:00` — <https://www.sec.gov/Archives/edgar/data/701719/000110465926128592/0001104659-26-128592-index.htm>

Last entry: `8-K - BLUE DOLPHIN ENERGY CO (0000793306) (Filer)` — updated `2026-11-16T16:18:18-05:00` — <https://www.sec.gov/Archives/edgar/data/793306/000143774926037179/0001437749-26-037179-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - Envela Corp (0000701719) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/701719/000110465926128592/0001104659-26-128592-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-16 &lt;b&gt;AccNo:&lt;/b&gt; 0001104659-26-128592 &lt;b&gt;Size:&lt;/b&gt; 481 KB
&lt;br&gt;Item 2.02: Results of Operations and Financial Condition
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-16T17:31:11-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001104659-26-128592</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - BLUE DOLPHIN ENERGY CO (0000793306) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/793306/000143774926037179/0001437749-26-037179-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-16 &lt;b&gt;AccNo:&lt;/b&gt; 0001437749-26-037179 &lt;b&gt;Size:&lt;/b&gt; 328 KB
&lt;br&gt;Item 2.02: Results of Operations and Financial Condition
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-16T16:18:18-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001437749-26-037179</id>
</entry>
```

Page `start=100` — requested 2026-11-17T10:40:45Z, responded 2026-11-17T10:40:49Z, HTTP 200, Date header `Tue, 17 Nov 2026 10:40:49 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-17T05:40:49-05:00</updated>`

First entry: `8-K - NEIGHBORHOOD INTELLIGENCE, INC. (0001130713) (Filer)` — updated `2026-11-16T16:18:08-05:00` — <https://www.sec.gov/Archives/edgar/data/1130713/000114036126044210/0001140361-26-044210-index.htm>

Last entry: `8-K - BBCMS Mortgage Trust 2026-5C43 (0002153909) (Filer)` — updated `2026-11-16T13:40:29-05:00` — <https://www.sec.gov/Archives/edgar/data/2153909/000153949726002999/0001539497-26-002999-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - NEIGHBORHOOD INTELLIGENCE, INC. (0001130713) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1130713/000114036126044210/0001140361-26-044210-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-16 &lt;b&gt;AccNo:&lt;/b&gt; 0001140361-26-044210 &lt;b&gt;Size:&lt;/b&gt; 162 KB
&lt;br&gt;Item 8.01: Other Events
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-16T16:18:08-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001140361-26-044210</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - BBCMS Mortgage Trust 2026-5C43 (0002153909) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/2153909/000153949726002999/0001539497-26-002999-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-16 &lt;b&gt;AccNo:&lt;/b&gt; 0001539497-26-002999 &lt;b&gt;Size:&lt;/b&gt; 5 MB
&lt;br&gt;Item 1.01: Entry into a Material Definitive Agreement
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-16T13:40:29-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001539497-26-002999</id>
</entry>
```

### PULL 3

Page `start=0` — requested 2026-11-18T10:41:45Z, responded 2026-11-18T10:41:47Z, HTTP 200, Date header `Wed, 18 Nov 2026 10:41:48 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-18T05:41:48-05:00</updated>`

First entry: `8-K - GridAI Technologies Corp. (0001604191) (Filer)` — updated `2026-11-17T17:29:47-05:00` — <https://www.sec.gov/Archives/edgar/data/1604191/000110465926129167/0001104659-26-129167-index.htm>

Last entry: `8-K - NEPHROS INC (0001196298) (Filer)` — updated `2026-11-17T16:05:37-05:00` — <https://www.sec.gov/Archives/edgar/data/1196298/000149315226052831/0001493152-26-052831-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - GridAI Technologies Corp. (0001604191) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1604191/000110465926129167/0001104659-26-129167-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-17 &lt;b&gt;AccNo:&lt;/b&gt; 0001104659-26-129167 &lt;b&gt;Size:&lt;/b&gt; 905 KB
&lt;br&gt;Item 1.01: Entry into a Material Definitive Agreement
&lt;br&gt;Item 2.01: Completion of Acquisition or Disposition of Assets
&lt;br&gt;Item 3.02: Unregistered Sales of Equity Securities
&lt;br&gt;Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
&lt;br&gt;Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
&lt;br&gt;Item 7.01: Regulation FD Disclosure
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-17T17:29:47-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001104659-26-129167</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - NEPHROS INC (0001196298) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1196298/000149315226052831/0001493152-26-052831-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-17 &lt;b&gt;AccNo:&lt;/b&gt; 0001493152-26-052831 &lt;b&gt;Size:&lt;/b&gt; 190 KB
&lt;br&gt;Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
</summary>
<updated>2026-11-17T16:05:37-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001493152-26-052831</id>
</entry>
```

Page `start=100` — requested 2026-11-18T10:41:48Z, responded 2026-11-18T10:41:50Z, HTTP 200, Date header `Wed, 18 Nov 2026 10:41:51 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-18T05:41:51-05:00</updated>`

First entry: `8-K - IMPACT BIOMEDICAL INC. (0001834105) (Filer)` — updated `2026-11-17T16:05:36-05:00` — <https://www.sec.gov/Archives/edgar/data/1834105/000149315226052822/0001493152-26-052822-index.htm>

Last entry: `8-K - UL Solutions Inc. (0001901440) (Filer)` — updated `2026-11-17T07:03:35-05:00` — <https://www.sec.gov/Archives/edgar/data/1901440/000190144026000037/0001901440-26-000037-index.htm>

Raw first `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - IMPACT BIOMEDICAL INC. (0001834105) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1834105/000149315226052822/0001493152-26-052822-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-17 &lt;b&gt;AccNo:&lt;/b&gt; 0001493152-26-052822 &lt;b&gt;Size:&lt;/b&gt; 226 KB
&lt;br&gt;Item 5.07: Submission of Matters to a Vote of Security Holders
</summary>
<updated>2026-11-17T16:05:36-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001493152-26-052822</id>
</entry>
```

Raw last `<entry>` element, exactly as the saved feed response returned it (Revision 1):

```xml
<entry>
<title>8-K - UL Solutions Inc. (0001901440) (Filer)</title>
<link rel="alternate" type="text/html" href="https://www.sec.gov/Archives/edgar/data/1901440/000190144026000037/0001901440-26-000037-index.htm"/>
<summary type="html">
 &lt;b&gt;Filed:&lt;/b&gt; 2026-11-17 &lt;b&gt;AccNo:&lt;/b&gt; 0001901440-26-000037 &lt;b&gt;Size:&lt;/b&gt; 245 KB
&lt;br&gt;Item 7.01: Regulation FD Disclosure
&lt;br&gt;Item 8.01: Other Events
&lt;br&gt;Item 9.01: Financial Statements and Exhibits
</summary>
<updated>2026-11-17T07:03:35-05:00</updated>
<category scheme="https://www.sec.gov/" label="form type" term="8-K"/>
<id>urn:tag:sec.gov,2008:accession-number=0001901440-26-000037</id>
</entry>
```

## PROOF — reviewed filings

Per filing: its two requests with the UTC time each was actually fetched (recorded by the review tool at fetch time), the Documents table from its EDGAR index page (verbatim rows), then each item heading with the first sentence(s) under it. A quote is the heading as printed, an em dash, then the first sentence(s) verbatim and complete; exhibit-list items quote the complete exhibit list (Revision 1: the excerpts that were fragmented at abbreviations or cut at 900 characters in the first submission were replaced with complete first sentences). Revision 2: where a summary states facts beyond the first sentence(s), the excerpt also quotes verbatim the further sentence(s) or exhibit-list lines those facts come from, so each summary can be read from the sentence(s) excerpted under its heading. Revision 3: the same rule was re-applied to all 108 summaries with a stricter check; the six items the evaluator named in round 3 now quote the further sentence(s) their summaries state, and the few summaries that stated a total or a count no filing sentence states had that total or count removed (see Revision 3 corrections). Index and document URLs resolve live (all 40 index pages re-opened with HTTP 200 when re-checked 2026-11-18).

### 1. Tempest Therapeutics, Inc. — `0001213900-26-119916`

CIK 0001544227, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/0001213900-26-119916-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/ea0312157-8k_tempest.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/0001213900-26-119916-index.htm> requested 2026-11-16T11:11:40Z, responded 2026-11-16T11:11:42Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/ea0312157-8k_tempest.htm> requested 2026-11-16T11:11:42Z, responded 2026-11-16T11:11:43Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312157-8k_tempest.htm iXBRL | 8-K | 34053 |
| 2 | PRESS RELEASE DATED NOVEMBER 13, 2026 | ea031215701ex99-1.htm | EX-99.1 | 66662 |
| 3 | GRAPHIC | ea031215701_ex99-1img1.jpg | GRAPHIC | 13928 |
|  | Complete submission text file | 0001213900-26-119916.txt |  | 339838 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Tempest Therapeutics, Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026 and other business highlights.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 99.1 Press release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 2. BeyondSpring Inc. — `0001171843-26-007431`

CIK 0001677940, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/0001171843-26-007431-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/f8k_111326.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/0001171843-26-007431-index.htm> requested 2026-11-16T11:11:44Z, responded 2026-11-16T11:11:45Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/f8k_111326.htm> requested 2026-11-16T11:11:46Z, responded 2026-11-16T11:11:46Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | f8k_111326.htm iXBRL | 8-K | 15737 |
| 2 | PRESS RELEASE | exh_991.htm | EX-99.1 | 92889 |
|  | Complete submission text file | 0001171843-26-007431.txt |  | 313879 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, BeyondSpring Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Exhibit 99.1 Press release, dated November 13, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 3. BCP Investment Corp — `0001193125-26-461047`

CIK 0001372807, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/0001193125-26-461047-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/d520705d8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/0001193125-26-461047-index.htm> requested 2026-11-16T11:11:47Z, responded 2026-11-16T11:11:47Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/d520705d8k.htm> requested 2026-11-16T11:11:48Z, responded 2026-11-16T11:11:48Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d520705d8k.htm iXBRL | 8-K | 26427 |
| 2 | EX-99.1 | d520705dex991.htm | EX-99.1 | 226031 |
| 3 | EX-99.2 | d520705dex992.htm | EX-99.2 | 52300 |
| 7 | GRAPHIC | g520705ex99_2p10g1.jpg | GRAPHIC | 280451 |
| 8 | GRAPHIC | g520705ex99_2p11g1.jpg | GRAPHIC | 336442 |
| 9 | GRAPHIC | g520705ex99_2p12g1.jpg | GRAPHIC | 266788 |
| 10 | GRAPHIC | g520705ex99_2p13g1.jpg | GRAPHIC | 252375 |
| 11 | GRAPHIC | g520705ex99_2p14g1.jpg | GRAPHIC | 157658 |
| 12 | GRAPHIC | g520705ex99_2p15g1.jpg | GRAPHIC | 331804 |
| 13 | GRAPHIC | g520705ex99_2p16g1.jpg | GRAPHIC | 361215 |
| 14 | GRAPHIC | g520705ex99_2p17g1.jpg | GRAPHIC | 280287 |
| 15 | GRAPHIC | g520705ex99_2p18g1.jpg | GRAPHIC | 189636 |
| 16 | GRAPHIC | g520705ex99_2p19g1.jpg | GRAPHIC | 146729 |
| 17 | GRAPHIC | g520705ex99_2p1g1.jpg | GRAPHIC | 73371 |
| 18 | GRAPHIC | g520705ex99_2p2g1.jpg | GRAPHIC | 476897 |
| 19 | GRAPHIC | g520705ex99_2p3g1.jpg | GRAPHIC | 289176 |
| 20 | GRAPHIC | g520705ex99_2p4g1.jpg | GRAPHIC | 528470 |
| 21 | GRAPHIC | g520705ex99_2p5g1.jpg | GRAPHIC | 421003 |
| 22 | GRAPHIC | g520705ex99_2p6g1.jpg | GRAPHIC | 388937 |
| 23 | GRAPHIC | g520705ex99_2p7g1.jpg | GRAPHIC | 199182 |
| 24 | GRAPHIC | g520705ex99_2p8g1.jpg | GRAPHIC | 358424 |
| 25 | GRAPHIC | g520705ex99_2p9g1.jpg | GRAPHIC | 297953 |
| 26 | GRAPHIC | g520705g91v13.jpg | GRAPHIC | 6574 |
|  | Complete submission text file | 0001193125-26-461047.txt |  | 8242390 |

- Item 2.02 Results of Operations and Financial Condition. — On November 11, 2026, BCP Investment Corporation (the “Company”) issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026. A copy of the press release is being furnished as Exhibit 99.1 to this Current Report on Form 8-K and is incorporated herein by reference. Additionally, on November 12, 2026, the Company made available on its website, https://www.bcpinvestmentcorporation.com/home, a supplemental investor presentation with respect to the earnings release. A copy of the investor presentation is being furnished as Exhibit 99.2 to this Current Report on Form 8-K and is incorporated herein by reference.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits: Exhibit Number Description 99.1 Press Release, dated November 11, 2026 99.2 Investor Presentation, dated November 12, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL Document)

### 4. CareTrust REIT, Inc. — `0001140361-26-043831`

CIK 0001590717, form 8-K, feed items 1.01, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/0001140361-26-043831-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/ny20085288x3_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/0001140361-26-043831-index.htm> requested 2026-11-16T11:11:49Z, responded 2026-11-16T11:11:50Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/ny20085288x3_8k.htm> requested 2026-11-16T11:11:50Z, responded 2026-11-16T11:11:51Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | ny20085288x3_8k.htm iXBRL | 8-K | 40888 |
| 2 | EXHIBIT 1.1 | ny20085288x3_ex1-1.htm | EX-1.1 | 288465 |
| 3 | EXHIBIT 5.1 | ny20085288x3_ex5-1.htm | EX-5.1 | 34329 |
| 4 | EXHIBIT 10.1 | ny20085288x3_ex10-1.htm | EX-10.1 | 248706 |
| 5 | EXHIBIT 10.2 | ny20085288x3_ex10-2.htm | EX-10.2 | 250717 |
| 6 | EXHIBIT 10.3 | ny20085288x3_ex10-3.htm | EX-10.3 | 248558 |
| 7 | EXHIBIT 10.4 | ny20085288x3_ex10-4.htm | EX-10.4 | 250396 |
| 11 |  | ny20085288x3_ex5-1img01.jpg | GRAPHIC | 12006 |
|  | Complete submission text file | 0001140361-26-043831.txt |  | 1772611 |

- Item 1.01 Entry into a Material Definitive Agreement — On November 11, 2026, CareTrust REIT, Inc. (the “Company”) entered into separate forward sale agreements (the “Initial Forward Sale Agreements”) with each of Bank of America, N.A. and Morgan Stanley & Co. LLC (the “Forward Purchasers”), relating to an aggregate of 17,000,000 shares of the Company’s common stock, par value $0.01 per share (“Common Stock”). On November 12, 2026, the Company entered into separate forward sale agreements (the “Additional Forward Sale Agreements” and, collectively with the Initial Forward Sale Agreements, the “Forward Sale Agreements”) with each of the Forward Purchasers, relating to an aggregate of 2,550,000 shares of Common Stock.
- Item 8.01 Other Events — On November 11, 2026, the Company and the Partnership entered into the Underwriting Agreement with the Underwriters, the Forward Purchasers and the Forward Sellers, relating to the registered public offering and sale of 17,000,000 shares of Common Stock (the “Offering”). In addition, the Underwriters were granted a 30-day option to purchase from time to time up to an additional 2,550,000 shares of Common Stock upon the same terms. On November 12, 2026, the Underwriters exercised in full their option to purchase the additional 2,550,000 shares of Common Stock pursuant to the Underwriting Agreement. On the terms and subject to the conditions set forth in the Underwriting Agreement, the Forward Purchasers (or their respective affiliates) borrowed an aggregate of 19,550,000 shares of Common Stock from third parties and sold them to the Underwriters on November 13, 2026.
- Item 9.01 Financial Statements and Exhibits — (d) Exhibits. Exhibit No. Description 1.1 Underwriting Agreement, dated November 11, 2026, by and among CareTrust REIT, Inc., CTR Partnership, L.P., BofA Securities, Inc. and Morgan Stanley & Co. LLC, as representatives of the several Underwriters and as Forward Sellers, and Bank of America, N.A. and Morgan Stanley & Co. LLC, as Forward Purchasers. 5.1 Opinion of DLA Piper LLP (US). 10.1 Forward Confirmation, dated November 11, 2026, between CareTrust REIT, Inc. and Morgan Stanley & Co. LLC. 10.2 Forward Confirmation, dated November 11, 2026, between CareTrust REIT, Inc. and Bank of America, N.A. 10.3 Forward Confirmation, dated November 12, 2026, between CareTrust REIT, Inc. and Morgan Stanley & Co. LLC. 10.4 Forward Confirmation, dated November 12, 2026, between CareTrust REIT, Inc. and Bank of America, N.A. 23.1 Consent of DLA Piper LLP (US) (included in Exhibit 5.1). 104 Cover Page Interactive Data File (embedded within the inline XBRL document).

### 5. MANGOCEUTICALS, INC. — `0001493152-26-051858`

CIK 0001938046, form 8-K, feed items 3.03, 5.03, 5.07, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/0001493152-26-051858-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/0001493152-26-051858-index.htm> requested 2026-11-16T11:11:51Z, responded 2026-11-16T11:11:52Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/form8-k.htm> requested 2026-11-16T11:11:52Z, responded 2026-11-16T11:11:53Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 75576 |
|  | Complete submission text file | 0001493152-26-051858.txt |  | 251805 |

- Item 3.03 Material Modification to Rights of Security Holders. — As described in Item 5.03, which is incorporated by reference into this Item 3.03, Mangoceuticals, Inc. (the “Company”) amended its Series B and Series C preferred stock designations effective November 9, 2026, and established its Series D Preferred Stock effective November 9, 2026. Upon issuance, the Series D Preferred Stock will rank senior to the Company’s registered common stock, par value $0.0001 per share (the “Common Stock”), with respect to dividends and distributions upon liquidation, dissolution or winding up. The charter filings did not themselves result in the issuance of any Series D Preferred Stock.
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — On November 9, 2026, the Company filed with the Texas Secretary of State a certificate of amendment to each of the previously filed certificates of designations governing its Series B Convertible Preferred Stock (the “Series B Preferred Stock”) and its 6% Series C Convertible Cumulative Preferred Stock (the “Series C Preferred Stock”), as amended. The Board of Directors approved the Amendments on November 4, 2026. The Series B Amendment adds a new Section 13, approving the Series D Designation (defined below) and the transactions implementing it, recognizing the Series D Preferred Stock’s senior dividend and liquidation ranking, and excluding the Series D Preferred Stock from the definition of Junior Securities under the Series B designation. For those transactions, the amendment waives conflicting restrictions, including the variable rate transaction restriction in the Series B Preferred Stock designation and applicable repurchase restrictions, as well as conflicting adjustment, participation and notice rights and resulting defaults and remedies. The Series C Amendment adds a new Section 17, approving the Series D Designation and the transactions implementing it, treating the Series D Preferred Stock as Senior Shares under the Series C Preferred Stock designation, and waiving conflicting restrictions, adjustment and participation rights, notice requirements and resulting defaults and remedies for those transactions. On November 9, 2026, the Board of Directors approved the designation of the Series D Preferred Stock and on November 9, 2026, the Company filed with the Texas Secretary of State its Certificate of Designations (the “Series D Designation”) establishing 1,000,000 shares of 8% Series D Convertible Cumulative Preferred Stock, par value $0.0001 per share (the “Series D Preferred Stock”).
- Item 5.07 Submission of Matters to a Vote of Security Holders. — On November 6, 2026, the holder of all 980,000 outstanding shares of Series C Preferred Stock, acting by written consent in lieu of a meeting, approved the Series C Amendment and the Series D Designation and the transactions contemplated thereby, including the proposed sale of up to 1,000,000 shares of Series D Preferred Stock at $10.00 per share pursuant to Regulation A. The consenting holder represented 100% of the outstanding Series C shares and voting power entitled to act on the matters submitted. All 980,000 shares consented to each matter; there were no votes against, abstentions or broker non-votes.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 3.1 Certificate of Amendment to Mangoceuticals, Inc.’s Certificate of Designations of Series B Convertible Preferred Stock, filed with the Secretary of State of Texas on November 9, 2026 (incorporated by reference to Exhibit 2.11 to the Company’s Offering Statement on Form 1-A filed November 12, 2026). 3.2 Certificate of Amendment to Mangoceuticals, Inc.’s Certificate of Designations of 6% Series C Convertible Cumulative Preferred Stock, filed with the Secretary of State of Texas on November 9, 2026 (incorporated by reference to Exhibit 2.12 to the Company’s Offering Statement on Form 1-A filed November 12, 2026). 3.3 Certificate of Designations of Mangoceuticals, Inc.’s 8% Series D Convertible Cumulative Preferred Stock, filed with the Secretary of State of Texas on November 9, 2026 (incorporated by reference to Exhibit 2.13 to the Company’s Offering Statement on Form 1-A filed November 12, 2026). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 6. Western Union CO — `0001193125-26-461028`

CIK 0001365135, form 8-K, feed items 1.02, 2.03. Index: <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/0001193125-26-461028-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/d152329d8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/0001193125-26-461028-index.htm> requested 2026-11-16T11:11:54Z, responded 2026-11-16T11:11:54Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/d152329d8k.htm> requested 2026-11-16T11:11:55Z, responded 2026-11-16T11:11:55Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d152329d8k.htm iXBRL | 8-K | 27002 |
|  | Complete submission text file | 0001193125-26-461028.txt |  | 138593 |

- Item 1.02 Termination of a Material Definitive Agreement. — As previously reported by The Western Union Company (the “Company”), in the Current Report on Form 8-K filed with the Securities and Exchange Commission (the “SEC”) on June 28, 2024, the Company entered into a delayed draw term loan credit agreement, dated as of June 25, 2024, with the lenders party thereto and Bank of America, N.A., as administrative agent (the “2024 Term Loan Agreement”). The 2024 Term Loan Agreement will terminate upon the repayment described in Item 2.03 below, which the Company expects to occur on or about November 17, 2026. The Company will not incur any material early termination penalties in connection with such repayment and termination.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — As previously reported by the Company, in the Current Report on Form 8-K filed with the SEC on January 9, 2026 (the “Closing Date 8-K”), the Company entered into a delayed draw term loan credit agreement, dated as of January 9, 2026 (as amended by the First Amendment thereto, dated as of June 17, 2026, the “Term Loan Agreement”), with the lenders party thereto and Bank of America, N.A., as administrative agent. On November 10, 2026, the Company borrowed an $800,000,000 term loan (the “Term Loan”) under the Term Loan Agreement which represents a borrowing of the full committed amount thereunder, reducing commitments under the facility to zero. The Company intends to use the proceeds of the Term Loan to repay in full the $800,000,000 aggregate principal amount of term loan outstanding under the 2024 Term Loan Agreement, which term loan is scheduled to mature in December 2027.

### 7. 3D SYSTEMS CORP — `0001193125-26-461027`

CIK 0000910638, form 8-K, feed items 1.01, 1.02, 2.03, 3.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/0001193125-26-461027-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/d533328d8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/0001193125-26-461027-index.htm> requested 2026-11-16T11:11:56Z, responded 2026-11-16T11:11:57Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/d533328d8k.htm> requested 2026-11-16T11:11:57Z, responded 2026-11-16T11:11:58Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d533328d8k.htm iXBRL | 8-K | 37183 |
| 2 | EX-4.1 | d533328dex41.htm | EX-4.1 | 659074 |
| 6 | GRAPHIC | g533328dsp73a.jpg | GRAPHIC | 3187 |
| 7 | GRAPHIC | g533328dsp73b.jpg | GRAPHIC | 4257 |
| 8 | GRAPHIC | g533328dsp74.jpg | GRAPHIC | 4334 |
| 9 | GRAPHIC | g533328dsp75.jpg | GRAPHIC | 4508 |
| 10 | GRAPHIC | g533328dsp77.jpg | GRAPHIC | 3781 |
| 11 | GRAPHIC | g533328dsp78.jpg | GRAPHIC | 4476 |
|  | Complete submission text file | 0001193125-26-461027.txt |  | 988844 |

- Item 1.01 Entry into a Material Definitive Agreement. — As previously disclosed, on November 4, 2026, 3D Systems Corporation (the “Company”) entered into separate, privately negotiated agreements (the “Exchange Agreements”) with all of the holders (the “Transaction Participants”) of the Company’s currently outstanding 5.875% Convertible Senior Secured Notes due 2030 (the “2030 Notes”). On November 12, 2026, the Company entered into an indenture (the “2031 Notes Indenture”) with U.S. Bank Trust Company, National Association, as trustee, pursuant to which the Company issued $85,000,000 aggregate principal amount of its 3.30% Convertible Senior Notes due 2031 (the “2031 Notes”) to the Transaction Participants in exchange for all of their outstanding 2030 Notes. Pursuant to the Exchange Agreements, the Company also paid the Transaction Participants additional consideration consisting of (i) an aggregate of $20,000,000 in cash (plus accrued and unpaid interest on the 2030 Notes exchanged to, but excluding, November 12, 2026) and (ii) an aggregate of 13,471,138 shares (the “Shares”) of the Company’s common stock, par value $0.001 per share (the “Common Stock”).
- Item 1.02 Termination of a Material Definitive Agreement. — On November 12, 2026, following the exchange of all of the outstanding 2030 Notes pursuant to the Exchange Agreements, the Company delivered to Wilmington Savings Fund Society, FSB, as trustee and collateral agent (“WSFS”), an order for the cancellation of all of the outstanding 2030 Notes issued under the indenture, dated as of June 23, 2025 (as supplemented, the “2030 Notes Indenture”), among the Company, the guarantors party thereto and WSFS. As a result of the cancellation, the 2030 Notes Indenture was satisfied and discharged in accordance with its terms, and the guarantees of the 2030 Notes and all liens on the collateral securing the 2030 Notes were released.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the 2031 Notes Indenture and the 2031 Notes is incorporated herein by reference.
- Item 3.02 Unregistered Sales of Equity Securities. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the issuance of the Shares and the 2031 Notes is incorporated herein by reference. On November 12, 2026, the Company issued 1,464,206 shares (the “JWCA Shares”) of Common Stock to J. Wood Capital Advisors LLC (“JWCA”) for services rendered in connection with the transactions contemplated by the Exchange Agreements. The Company did not receive any cash proceeds from the issuance of the JWCA Shares. The JWCA Shares were issued pursuant to an exemption provided by Section 4(a)(2) of the Securities Act.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. 4.1 Indenture, dated as of November 12, 2026, between 3D Systems Corporation and U.S. Bank Trust Company, National Association, as trustee 4.2 Form of 3.30% Convertible Senior Notes due 2031 (included in Exhibit 4.1) 104 Cover Page Interactive Data File (embedded as Inline XBRL document)

### 8. Navient Holdings, Inc. — `0001140361-26-043829`

CIK 0002152623, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/0001140361-26-043829-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/ef20085597_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/0001140361-26-043829-index.htm> requested 2026-11-16T11:11:58Z, responded 2026-11-16T11:11:59Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/ef20085597_8k.htm> requested 2026-11-16T11:11:59Z, responded 2026-11-16T11:12:00Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | ef20085597_8k.htm iXBRL | 8-K | 28917 |
|  | Complete submission text file | 0001140361-26-043829.txt |  | 154717 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 11, 2026, Frederick Arnold, a member of the Board of Directors (the “Board”) of Navient Holdings, Inc. (the “Company”), informed the Company that he was voluntarily retiring from the Board effective immediately. Mr. Arnold’s decision to retire from the Board is not the result of any disagreement with the Company.

### 9. Polomar Health Services, Inc. — `0001493152-26-051849`

CIK 0001265521, form 8-K, feed items 1.01, 2.03, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/0001493152-26-051849-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/0001493152-26-051849-index.htm> requested 2026-11-16T11:12:00Z, responded 2026-11-16T11:12:01Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/form8-k.htm> requested 2026-11-16T11:12:01Z, responded 2026-11-16T11:12:02Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 31282 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 46251 |
|  | Complete submission text file | 0001493152-26-051849.txt |  | 252832 |

- Item 1.01 Entry Into a Material Definitive Agreement. — The information set forth under Item 2.03 of this Current Report on Form 8-K is incorporated by reference into this Item 1.01.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation. — Effective November 9, 2026, Polomar Health Services, Inc. (the “Company”) executed a Promissory Note and Loan Agreement (the “Note”) in favor of Island 40 Group, LLC (“I4G” or the “Lender”) in the principal amount of $450,000 reflecting the amount of commissions due and owing to I4G for services provided to the Company by I4G pursuant to the terms of a certain Sales Director and Distribution Agreement in effect between the Company and I4G. Polomar Specialty Pharmacy, LLC, a wholly owned subsidiary of the Company (the “Guarantor”), is also a party to the Note as a guarantor of the Note and accepts all obligations of the Company thereunder. The Note bears interest at an initial rate of 10% per annum, simple interest through December 31, 2026, and thereafter at a rate equal to the prime interest rate as published on the first day of each month in the Wall Street Journal – Money Rates plus 4%. The Note shall mature and be payable in full on March 31, 2027.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 10.1 Promissory Note and Loan Agreement Effective November 9, 2026, between Island 40 Group. LLC and Polomar Health Services, Inc. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. POLOMAR HEALTH SERVICES, INC. Date: November 13, 2026 By: /s/ Terrence M. Tierney Name: Terrence M. Tierney Title: Interim Chief Executive Officer

### 10. IonQ, Inc. — `0001193125-26-461016`

CIK 0001824920, form 8-K, feed items 3.02, 5.02, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/0001193125-26-461016-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/ionq-20261110.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/0001193125-26-461016-index.htm> requested 2026-11-16T11:12:03Z, responded 2026-11-16T11:12:04Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/ionq-20261110.htm> requested 2026-11-16T11:12:04Z, responded 2026-11-16T11:12:05Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | ionq-20261110.htm iXBRL | 8-K | 57111 |
| 2 | EX-5.1 | ionq-ex5_1.htm | EX-5.1 | 24184 |
| 3 | EX-99.1 | ionq-ex99_1.htm | EX-99.1 | 26100 |
| 4 | GRAPHIC | img1365411_0.jpg | GRAPHIC | 15584 |
|  | Complete submission text file | 0001193125-26-461016.txt |  | 245055 |

- Item 3.02 Unregistered Sales of Equity Securities. — On November 13, 2026, IonQ, Inc. (the “Company”) filed with the Securities and Exchange Commission (the “SEC”) a prospectus supplement to the prospectus included in the Company’s Registration Statement on Form S-3ASR filed with the SEC on February 26, 2025 (File No. 333-285279) (the “Registration Statement”), covering the resale by certain selling stockholders of an aggregate of 34,580,646 shares of Company common stock, par value $0.0001 per share.
- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Also on November 13, 2026, the Company announced that, on November 10, 2026, the Company appointed Gary Merrill as Chief Financial Officer, Treasurer, principal financial officer and principal accounting officer of the Company, to be effective upon his first day of employment, which is expected to be December 3, 2026 (the “Start Date”). Mr. Merrill succeeds Inder M. Singh, who held these roles until November 10, 2026. Niccolo M. de Masi will serve as the Company’s interim principal financial officer and principal accounting officer until the Start Date. Mr. Merrill, age 51, is joining the Company after having served as Chief Financial Officer of Commvault Systems, Inc. (“Commvault”), a publicly-traded provider of cyber resiliency solutions, from April 2026 until the present, before which he served in various other roles at Commvault, including as Chief Commercial Officer from August 2024 to April 2026, Chief Financial Officer from April 2022 to August 2024, Chief Business Operations Officer from 2019 to 2022 and Chief Accounting Officer from 2012 to 2019.
- Item 8.01 Other Events. — Also on November 13, 2026, the Company announced that, effective on November 16, 2026, Thomas A. Austin had been appointed as Chief Accounting Officer of the Company. Mr. Austin is joining the Company after having served as Chief Accounting Officer for Juniper Networks, a multinational networking corporation owned by the Hewlett Packard Enterprise Company.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 5.1 Opinion of Paul, Weiss, Rifkind, Wharton & Garrison LLP. 23.1 Consent of Paul, Weiss, Rifkind, Wharton & Garrison LLP (included in Exhibit 5.1). 99.1 Press Release, dated November 13, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 11. Dolby Laboratories, Inc. — `0001193125-26-461010`

CIK 0001308547, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/0001193125-26-461010-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/d101237d8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/0001193125-26-461010-index.htm> requested 2026-11-16T11:12:06Z, responded 2026-11-16T11:12:07Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/d101237d8k.htm> requested 2026-11-16T11:12:07Z, responded 2026-11-16T11:12:08Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d101237d8k.htm iXBRL | 8-K | 30850 |
|  | Complete submission text file | 0001193125-26-461010.txt |  | 143851 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 10, 2026, the Compensation Committee (the “Committee”) of the Board of Directors of Dolby Laboratories, Inc. (the “Company”) adopted an executive cash bonus plan for fiscal 2027, titled the 2027 Dolby Executive Bonus Plan (the “2027 Executive Plan”). In accordance with the employment agreement dated July 10, 2026, between the Company, Dolby Laboratories, Inc., a California corporation, and Marc Whitten, the Company’s President and Chief Executive Officer, Mr. Whitten is eligible for an annual target bonus equal to 100% of his base salary, and his fiscal 2027 bonus will be paid at 100% of target. The actual bonuses for all other participating named executive officers will be determined by multiplying base salary by the applicable target bonus percentage, and then adjusting such target bonus amount based on (i) the extent to which the non-GAAP operating income, revenue and/or other goals are achieved, and (ii) such other criteria as the Committee, with input from the Chief Executive Officer, in the Committee’s sole and absolute discretion, determines are appropriate to calculate and determine such final bonus amount for any such executive officer.

### 12. Panamera Holdings Corp — `0001640334-26-001797`

CIK 0001620749, form 8-K, feed items 4.02. Index: <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/0001640334-26-001797-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/pnht_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/0001640334-26-001797-index.htm> requested 2026-11-16T11:12:09Z, responded 2026-11-16T11:12:10Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/pnht_8k.htm> requested 2026-11-16T11:12:10Z, responded 2026-11-16T11:12:11Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | pnht_8k.htm iXBRL | 8-K | 20200 |
|  | Complete submission text file | 0001640334-26-001797.txt |  | 124344 |

- Item 4.02 Non-Reliance on Previously Issued Financial Statements or a Related Audit Report or Interim Review — Pursuant to the 8K filed on October 26,2026 regarding an unreported employment agreement and resulting unreported lawsuit that caused the reporting to be affected by Item 4.02 Non-Reliance on Previously Issue Financial Statements or a Related Audit Report or Interim Review. Due to his the Company is in the process of restating the Non-Reliance Periods in an amendment to its previously filed periodic report, in its Annual Report on Form 10-K for the fiscal year ended July 31, 2025, and will file the related 10-K as soon as practicable. The Audit Committee discussed the matters disclosed in this Item 4.02 with the Company's independent registered public accounting firm.

### 13. Cingulate Inc. — `0001493152-26-051841`

CIK 0001862150, form 8-K, feed items 1.01, 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/0001493152-26-051841-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/0001493152-26-051841-index.htm> requested 2026-11-16T11:12:12Z, responded 2026-11-16T11:12:13Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/form8-k.htm> requested 2026-11-16T11:12:13Z, responded 2026-11-16T11:12:14Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 44022 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 32083 |
| 3 | EX-99.1 | ex99-1.htm | EX-99.1 | 41506 |
|  | Complete submission text file | 0001493152-26-051841.txt |  | 341695 |

- Item 1.01 Entry into Material Definitive Agreement — As previously disclosed, on March 24, 2026, Cingulate Inc. (the “Company”) entered into an ATM Sales Agreement, or the ATM Agreement, with A.G.P./Alliance Global Partners (“A.G.P.”) as sales agent (the “Agent”), pursuant to which the Company may offer and sell, our common stock, par value $0.0001 per share, or common stock, having an aggregate offering price of up to $100,000,000, from time to time, through the Agent. On November 13, 2026, the Company entered into Amendment No. 2 to the ATM Agreement (the “Amendment”) with A.G.P. and Maxim Group LLC (“Maxim”) solely to add Maxim Group LLC as an Agent under the ATM Agreement.
- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Cingulate Inc. issued a press release announcing its financial results for the quarter ended September 30, 2026 and providing a regulatory update.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Amendment No. 1 to ATM Agreement, by and among the Company, A.G.P. and Maxim, dated November 13, 2026 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 14. Flux Power Holdings, Inc. — `0001493152-26-051839`

CIK 0001083743, form 8-K, feed items 1.01, 2.03, 3.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/0001493152-26-051839-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/0001493152-26-051839-index.htm> requested 2026-11-16T11:12:15Z, responded 2026-11-16T11:12:16Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/form8-k.htm> requested 2026-11-16T11:12:16Z, responded 2026-11-16T11:12:17Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 49859 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 16812 |
| 3 | GRAPHIC | ex10-1_001.jpg | GRAPHIC | 20951 |
| 4 | GRAPHIC | ex10-1_002.jpg | GRAPHIC | 22454 |
|  | Complete submission text file | 0001493152-26-051839.txt |  | 296501 |

- Item 1.01 Entry into a Material Definitive Agreement. — As previously disclosed, on September 17, 2026 (the “Effective Date”), Flux Power Holdings, Inc. (the “Registrant”) and Flux Power, Inc., a wholly-owned subsidiary of the Registrant (“Flux” and together with the Registrant, the “Company”), entered into Amendment No. 7 to the Loan and Security Agreement (as amended, the “Loan and Security Agreement”) with Gibraltar Business Capital, LLC (“GBC”), pursuant to which the Company is required to, among other things, complete a sale of equity interests resulting in net proceeds of not less than $4.0 million (the “Equity Raise Requirement”) within 50 days of the Effective Date (the “Initial Equity Raise Deadline”), or such later date as may be agreed to in writing by GBC in GBC’s sole discretion. On November 13, 2026, the Company entered into a letter agreement with GBC, effective as of November 6, 2026 (the “Letter Agreement”), pursuant to which GBC agreed to extend the Initial Equity Raise Deadline from November 6, 2026 to December 4, 2026 (the “Extended Equity Raise Deadline”). All other terms and conditions of the Loan and Security Agreement remain unchanged and in full force and effect.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information required by Item 2.03 contained in Item 1.01 of this Current Report on Form 8-K is incorporated herein by reference.
- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 9, 2026, the Company received a notice (the “Notice”) from The NASDAQ Stock Market LLC (“Nasdaq”) notifying the Company that based on its stockholders’ deficit of ($431,000) as reported in its Form 10-Q for the fiscal quarter ended September 30, 2026, the Company is no longer in compliance with Nasdaq Listing Rule 5550(b)(1), which requires the Company to maintain a minimum of $2,500,000 in stockholders’ equity for continued listing on The Nasdaq Capital Market (the “Stockholders’ Equity Requirement”). Pursuant to the Notice, the Company has 45 calendar days from the date of the Notice, or until December 24, 2026, to submit a plan to regain compliance, and the Company intends to submit such a plan during this period.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Exhibit Description 10.1 Letter Agreement, dated November 13, 2026. 104 Cover Page Interactive Data File (formatted as Inline XBRL).

### 15. Versa Bancorp — `0001104659-26-127233`

CIK 0002100848, form 8-K12B, feed items 1.01, 2.01, 3.01, 3.03, 5.01, 5.02, 5.03, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/0001104659-26-127233-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/tm2629642d1_8k12b.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/0001104659-26-127233-index.htm> requested 2026-11-16T11:12:18Z, responded 2026-11-16T11:12:19Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/tm2629642d1_8k12b.htm> requested 2026-11-16T11:12:19Z, responded 2026-11-16T11:12:20Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K12B | tm2629642d1_8k12b.htm iXBRL | 8-K12B | 53973 |
| 2 | EXHIBIT 3.1 | tm2629642d1_ex3-1.htm | EX-3.1 | 32422 |
| 3 | EXHIBIT 3.2 | tm2629642d1_ex3-2.htm | EX-3.2 | 140770 |
| 4 | EXHIBIT 10.1 | tm2629642d1_ex10-1.htm | EX-10.1 | 98934 |
| 5 | EXHIBIT 10.2 | tm2629642d1_ex10-2.htm | EX-10.2 | 248030 |
| 6 | EXHIBIT 99.1 | tm2629642d1_ex99-1.htm | EX-99.1 | 17183 |
| 7 | EXHIBIT 99.3 | tm2629642d1_ex99-3.htm | EX-99.3 | 1182303 |
| 11 | GRAPHIC | exhibit99-1x001.jpg | GRAPHIC | 8112 |
| 12 | GRAPHIC | exhibit99-1x002.jpg | GRAPHIC | 6816 |
| 13 | GRAPHIC | tm2629642d1_ex10-2img001.jpg | GRAPHIC | 7095 |
|  | Complete submission text file | 0001104659-26-127233.txt |  | 2167049 |

- Item 1.01 Entry into a Material Definitive Agreement. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 1.01 by reference. Indemnification Agreements Upon the completion of the Reorganization, Versa Bancorp entered into indemnification agreements (each, an “Indemnification Agreement”) with each of its executive officers and directors.
- Item 2.01 Completion of Acquisition or Disposition of Assets. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 2.01 by reference.
- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 3.01 by reference.
- Item 3.03 Material Modification to Rights of Security Holders. — The information set forth in the Introductory Note and Item 5.03 of this Current Report on Form 8-K is incorporated into this Item 3.03 by reference. VersaBank is governed by Canadian law as a chartered bank under the Bank Act (Canada) (the “Bank Act”). Versa Bancorp, which as a result of the Reorganization became the parent company of VersaBank, is governed by the Delaware General Corporation Law (“DGCL”). The Bank Act differs in some material respects from the laws generally applicable to corporations and their shareholders under the DGCL. Information regarding these differences is included in the section titled “The Reorganization Proposal—Bank Regulatory Approvals—Change in Governing Law” in the Registration Statement and is incorporated herein by reference.
- Item 5.01 Changes in Control of Registrant. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 5.01 by reference.
- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, the Board received notice from Patrick DeLacey of his resignation from the Board. The decision of Mr. DeLacey to resign was not the result of any disagreement with Versa Bancorp on any matter relating to Versa Bancorp’s operations, policies or practices. Effective upon Mr. DeLacey’s resignation, the Board has reduced its size from eight (8) directors to seven (7) directors, Scott Verity has been appointed as chair of the Audit Committee, and Barbara Chaffee has been appointed as a member of the Audit Committee.
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — In anticipation of the completion of the Reorganization, on November 12, 2026, Versa Bancorp filed a certificate of amendment with the Secretary of State of the State of Delaware amending its certificate of incorporation, as amended (the “Amended Certificate of Incorporation”) to (i) increase the authorized number of Versa Bancorp Shares to 350,000,000 and (ii) provide for indemnification of Versa Bancorp’s officers and directors, and authorize indemnification of such employees and agents as Versa Bancorp determines to be appropriate, to the fullest extent permitted by Delaware law and other applicable law. Effective upon the filing of the certificate of amendment, Versa Bancorp also adopted its bylaws (the “Bylaws”).
- Item 7.01 Regulation FD Disclosure. — On November 13, 2026, Versa Bancorp issued a press release announcing the completion of the Reorganization.
- Item 9.01 Financial Statements and Exhibits. — (a) Financial statements of businesses or funds acquired. The audited consolidated financial statements of VersaBank as of and for the years ended October 31, 2025 and 2024, and the related notes thereto, are attached hereto as Exhibit 99.2 and incorporated herein by reference. The unaudited consolidated financial statements of VersaBank as of and for the nine months ended July 31, 2026 and 2025, and the related notes thereto, are attached hereto as Exhibit 99.3 and incorporated herein by reference. (d) Exhibits. Exhibit No. Description 3.1 Amended Certificate of Incorporation of Versa Bancorp 3.2 Bylaws of Versa Bancorp 10.1 Form of Indemnification Agreement of Versa Bancorp 10.2 Omnibus Long-Term Incentive Plan 99.1 Press Release, dated November 13, 2026 99.2 Audited consolidated financial statements of VersaBank as of and for the years ended October 31, 2025 and 2024, and the related notes thereto (incorporated by reference to Amendment No. 2 to Versa Bancorp’s Registration Statement on Form S-4, filed on July 29, 2026) 99.3 Unaudited consolidated financial statements of VersaBank as of and for the nine months ended July 31, 2026 and 2025, and the related notes thereto 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 16. Datavault AI Inc. — `0001104659-26-127230`

CIK 0001682149, form 8-K, feed items 3.01, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/0001104659-26-127230-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/tm2629197d1_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/0001104659-26-127230-index.htm> requested 2026-11-16T11:12:21Z, responded 2026-11-16T11:12:22Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/tm2629197d1_8k.htm> requested 2026-11-16T11:12:22Z, responded 2026-11-16T11:12:23Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629197d1_8k.htm iXBRL | 8-K | 30339 |
| 2 | EXHIBIT 99.1 | tm2629197d1_ex99-1.htm | EX-99.1 | 6891 |
|  | Complete submission text file | 0001104659-26-127230.txt |  | 207504 |

- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 10, 2026, Datavault AI Inc., a Delaware corporation (the “Company”), received a letter (the “Letter”) from the Listing Qualifications department of The Nasdaq Stock Market LLC (“Nasdaq”) notifying the Company that the Company’s common stock, par value $0.0001 per share (“Common Stock”), was subject to delisting from Nasdaq due to the Company’s non-compliance with the $1.00 bid price requirement set forth in Nasdaq Listing Rule 5550(a)(2) (the “Bid Price Rule”), unless the Company timely requests a hearing before the Nasdaq Hearings Panel (the “Panel”), which the Company intends to do. The Company was also notified that, due to a closing bid price of less than $0.10 per share for ten consecutive business days, Nasdaq will suspend trading in the Company’s securities on Nasdaq effective with the open of the market on November 17, 2026 in accordance with Nasdaq Listing Rule 5810(c)(3)(A)(iii). While trading is suspended on Nasdaq, the Company’s Common Stock should be eligible to trade on the OTC Markets system under its existing symbol “DVLT,” also effective with the open of business on November 17, 2026.
- Item 8.01 Other Events. — On November 13, 2026, the Company issued a press release (the “Press Release”) announcing receipt of the Letter and the Nasdaq trading suspension, as required under Nasdaq Listing Rule 5810(c)(3)(A)(iii).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release, dated November 13, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 17. Douglas Elliman Inc. — `0001878897-26-000055`

CIK 0001878897, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/0001878897-26-000055-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/doug-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/0001878897-26-000055-index.htm> requested 2026-11-16T11:12:24Z, responded 2026-11-16T11:12:24Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/doug-20261113.htm> requested 2026-11-16T11:12:25Z, responded 2026-11-16T11:12:25Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | doug-20261113.htm iXBRL | 8-K | 39227 |
|  | Complete submission text file | 0001878897-26-000055.txt |  | 154928 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers — On November 13, 2026, Douglas Elliman Inc. (the “Company”) and James B. Kirkland III mutually agreed that Mr. Kirkland will retire (the “Kirkland Retirement”) from his position as Executive Vice President, Treasurer and Chief Financial Officer, effective November 13, 2026, pursuant to a Separation Agreement and General Release (the “Kirkland Separation Agreement”). The Kirkland Separation Agreement provides for a release of certain claims by Mr. Kirkland, if any, in exchange for (i) severance pay equal to one year of his annualized base salary of $650,000.00, (ii) a pro-rated bonus amount for 2026 in the amount of $369,253, (iii) a retention payment in the amount of $150,000.00, (iv) accelerated vesting of 447,708 restricted shares underlying certain restricted stock grants (with the remainder of unvested shares being forfeited), (v) payment of $40,000 in unused vacation and (vi) eligibility for continuation coverage under the Company’s group health plan pursuant to the Consolidated Omnibus Budget Reconciliation Act and continued copayment of premiums at the same level as if Mr. Kirkland were an active employee of the Company.

### 18. CHEETAH NET SUPPLY CHAIN SERVICE INC. — `0001104659-26-127228`

CIK 0001951667, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/0001104659-26-127228-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/tm2629774d1_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/0001104659-26-127228-index.htm> requested 2026-11-16T11:12:26Z, responded 2026-11-16T11:12:26Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/tm2629774d1_8k.htm> requested 2026-11-16T11:12:27Z, responded 2026-11-16T11:12:27Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629774d1_8k.htm iXBRL | 8-K | 25433 |
| 2 | EXHIBIT 99.1 | tm2629774d1_ex99-1.htm | EX-99.1 | 128512 |
| 6 | GRAPHIC | tm2629774d1_ex99-1img001.jpg | GRAPHIC | 21370 |
| 7 | GRAPHIC | tm2629774d1_ex99-1img002.jpg | GRAPHIC | 32855 |
|  | Complete submission text file | 0001104659-26-127228.txt |  | 409082 |

- Item 2.02 Results of Operations and Financial Condition — On November 13, 2026, Cheetah Net Supply Chain Service Inc. issued a press release announcing its financial results for the third quarter of 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 99.1 The Press Release 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 19. AIRWA INC. — `0001493152-26-051834`

CIK 0001674440, form 8-K, feed items 1.01, 3.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/0001493152-26-051834-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/0001493152-26-051834-index.htm> requested 2026-11-16T11:12:28Z, responded 2026-11-16T11:12:28Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/form8-k.htm> requested 2026-11-16T11:12:29Z, responded 2026-11-16T11:12:29Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 42427 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 230734 |
|  | Complete submission text file | 0001493152-26-051834.txt |  | 480566 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 9, 2026, AiRWA Inc. (the “Company”) entered into securities purchase agreements (the “Purchase Agreement”) with certain investors, pursuant to which the Company agreed to sell to the investors an aggregate of 1,800,000 shares of common stock of the Company, par value $0.001 per share (the “Common Stock”), at a purchase price of $0.8332 per share of Common Stock, which was the closing price of the Common Stock on the preceding trading day (the “Transaction”). The Transaction is expected to close on or about November 17, 2026, and the gross proceeds are expected to be approximately $1.5 million. The Company intends to use the net proceeds from the Transaction for working capital and other general corporate purposes.
- Item 3.02 Unregistered Sales of Equity Securities. — The information provided in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 3.02.
- Item 9.01 Financial Statements and Exhibits. — The following exhibits are furnished with this Form 8-K: Exhibit No. Description 10.1 Form of Securities Purchase Agreement 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 20. AZIO AI HOLDINGS, INC. — `0001437749-26-036953`

CIK 0001563568, form 8-K, feed items 5.02, 5.07. Index: <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/0001437749-26-036953-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/adom20261113_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/0001437749-26-036953-index.htm> requested 2026-11-16T11:12:30Z, responded 2026-11-16T11:12:30Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/adom20261113_8k.htm> requested 2026-11-16T11:12:31Z, responded 2026-11-16T11:12:31Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | adom20261113_8k.htm iXBRL | 8-K | 65848 |
|  | Complete submission text file | 0001437749-26-036953.txt |  | 200777 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, at the 2026 Annual Meeting of Stockholders (the “Annual Meeting”) of Azio AI Holdings, Inc., a Delaware corporation (the “Company”), the Company’s stockholders approved the Azio AI Holdings, Inc. 2026 Equity Incentive Plan (the “2026 Plan”), which the Board of Directors of the Company (the “Board”) previously approved on July 2, 2026, subject to stockholder approval.
- Item 5.07 Submission of Matters to a Vote of Security Holders. — On November 13, 2026, the Company reconvened and held the Annual Meeting, which was originally convened on November 2, 2026, and adjourned to November 13, 2026, due to a lack of quorum. Holders of 9,401,687.72 shares of Common Stock (representing 54.2% of the shares of Common Stock outstanding on the Record Date) were present virtually or represented by proxy at the Annual Meeting on November 13, 2026, constituting a quorum. As described in further detail below, each of Proposals 1, 2, 3, 5, 6 and 7 was approved by the Company’s stockholders. In accordance with the approval of Proposal 7, the Annual Meeting was adjourned with respect to only Proposal 4, which concerns the approval, in accordance with Listing Rules 5635(a) and 5635(b) of The Nasdaq Stock Market LLC (“Nasdaq”), of the issuance of shares of Common Stock upon conversion of the Company’s Series A Non-Voting Convertible Preferred Stock (the “Conversion Proposal”), because the Company’s initial listing application required by Nasdaq Listing Rule 5110(a) has not yet been approved. The polls on the Conversion Proposal were not closed at the Annual Meeting, and the Annual Meeting will be reconvened only with respect to the Conversion Proposal on December 4, 2026, at 9:00 a.m., Pacific Time (the “Adjourned Annual Meeting”), as a virtual meeting at HTTPS://EDGE.MEDIA-SERVER.COM/MMC/GO/AZIO2026AGM.

### 21. Where Food Comes From, Inc. — `0001493152-26-051832`

CIK 0001360565, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/0001493152-26-051832-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/0001493152-26-051832-index.htm> requested 2026-11-16T11:12:32Z, responded 2026-11-16T11:12:33Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/form8-k.htm> requested 2026-11-16T11:12:33Z, responded 2026-11-16T11:12:34Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 41856 |
| 2 | EX-99.1 | ex99-1.htm | EX-99.1 | 89647 |
| 3 | EX-99.2 | ex99-2.htm | EX-99.2 | 17649 |
|  | Complete submission text file | 0001493152-26-051832.txt |  | 329533 |

- Item 2.02 Results of Operations and Financial Condition Reference — Reference is made to the Where Food Comes From, Inc. (the “Company”) press release on November 12, 2026 and conference call transcript, attached hereto as Exhibits 99.1 and 99.2, respectively, and incorporated by reference herein (including, without limitation, the information set forth in the cautionary statement contained in the press release and conference call transcript), relating to the Company’s financial results for the three and nine months ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits (d) — Exhibits Exhibit No. Description 99.1 Press Release issued and dated November 12, 2026 99.2 Transcript for November 12, 2026 conference call 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 22. Booking Holdings Inc. — `0001104659-26-127223`

CIK 0001075531, form 8-K, feed items 1.01, 2.03, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/0001104659-26-127223-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/tm2629703d1_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/0001104659-26-127223-index.htm> requested 2026-11-16T11:12:34Z, responded 2026-11-16T11:12:35Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/tm2629703d1_8k.htm> requested 2026-11-16T11:12:36Z, responded 2026-11-16T11:12:36Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629703d1_8k.htm iXBRL | 8-K | 94716 |
| 2 | EXHIBIT 1.1 | tm2629703d1_ex1-1.htm | EX-1.1 | 277372 |
| 3 | EXHIBIT 4.1 | tm2629703d1_ex4-1.htm | EX-4.1 | 59108 |
| 4 | EXHIBIT 4.2 | tm2629703d1_ex4-2.htm | EX-4.2 | 59109 |
| 5 | EXHIBIT 4.3 | tm2629703d1_ex4-3.htm | EX-4.3 | 59698 |
| 6 | EXHIBIT 4.4 | tm2629703d1_ex4-4.htm | EX-4.4 | 59494 |
| 7 | EXHIBIT 4.5 | tm2629703d1_ex4-5.htm | EX-4.5 | 46642 |
| 8 | EXHIBIT 4.6 | tm2629703d1_ex4-6.htm | EX-4.6 | 46331 |
| 9 | EXHIBIT 4.7 | tm2629703d1_ex4-7.htm | EX-4.7 | 45471 |
| 10 | EXHIBIT 4.8 | tm2629703d1_ex4-8.htm | EX-4.8 | 45952 |
| 11 | EXHIBIT 4.9 | tm2629703d1_ex4-9.htm | EX-4.9 | 460042 |
| 12 | EXHIBIT 5.1 | tm2629703d1_ex5-1.htm | EX-5.1 | 12186 |
| 17 | GRAPHIC | tm2629703d1_ex5-1img001.jpg | GRAPHIC | 16465 |
| 18 | GRAPHIC | tm2629703d1_ex5-1img002.jpg | GRAPHIC | 68972 |
|  | Complete submission text file | 0001104659-26-127223.txt |  | 1979998 |

- Item 1.01 Entry into a Material Definitive Agreement. — Senior Notes On November 13, 2026, Booking Holdings Inc. (the “Company”) executed four Officers’ Certificates (the “Officers’ Certificates”), in accordance with Sections 2.02 and 10.04 of the Indenture dated August 8, 2017 (the “Base Indenture” and, together with the Officers’ Certificates, the “Indenture”) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the “Trustee”) and registrar, in connection with the sale of €1,250,000,000 aggregate principal amount of the Company’s 3.950% Senior Notes due 2029 (the “2029 Notes”), €800,000,000 aggregate principal amount of the Company’s 4.375% Senior Notes due 2032 (the “2032 Notes”), €750,000,000 aggregate principal amount of the Company’s 4.750% Senior Notes due 2035 (the “2035 Notes”), and €750,000,000 aggregate principal amount of the Company’s 5.000% Senior Notes due 2038 (the “2038 Notes” and, together with the 2029 Notes, the 2032 Notes, and the 2035 Notes, the “Senior Notes”).
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation Under an Off-Balance Sheet Arrangement of the Registrant. — The information set forth under Item 1.01 of this Current Report on Form 8-K is incorporated by reference.
- Item 8.01 Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the “Underwriting Agreement”) with Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto (the “Underwriters”), pursuant to which the Company agreed to issue and sell to the Underwriters €3,550,000,000 aggregate principal amount of Senior Notes in a registered public offering (the “Offering”).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit Description 1.1* Underwriting Agreement, dated November 9, 2026, among Booking Holdings Inc., Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto. 4.1 Form of 3.950% Senior Note due 2029. 4.2 Form of 4.375% Senior Note due 2032. 4.3 Form of 4.750% Senior Note due 2035. 4.4 Form of 5.000% Senior Note due 2038. 4.5* Officers’ Certificate, dated November 13, 2026, with respect to the 3.950% Senior Note due 2029 issued pursuant to the Base Indenture. 4.6* Officers’ Certificate, dated November 13, 2026, with respect to the 4.375% Senior Note due 2032 issued pursuant to the Base Indenture. 4.7* Officers’ Certificate, dated November 13, 2026, with respect to the 4.750% Senior Note due 2035 issued pursuant to the Base Indenture. 4.8* Officers’ Certificate, dated November 13, 2026, with respect to the 5.000% Senior Note due 2038 issued pursuant to the Base Indenture. 4.9 Agency Agreement, dated as of November 13, 2026, by and between Booking Holdings Inc., as issuer, U.S. Bank Europe DAC, UK Branch, as paying agent, and U.S. Bank Trust Company, National Association, as transfer agent, registrar and trustee. 5.1 Opinion of Cravath, Swaine & Moore LLP, relating to the Senior Notes. 23.1 Consent of Cravath, Swaine & Moore LLP (included as part of Exhibit 5.1 to this Current Report). 104 Cover Page Interactive Data File - the cover page interactive data file does not appear in the Interactive Data File because its XBRL tags are embedded within the Inline XBRL document. *Schedules or similar attachments have been omitted pursuant to Item 601(a)(5) of Regulation S-K. The Company hereby undertakes to furnish copies of any of the omitted schedules or similar attachments upon request by the Securities and Exchange Commission.

### 23. BEASLEY BROADCAST GROUP INC — `0001193125-26-460951`

CIK 0001099160, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/0001193125-26-460951-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/bbgi-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/0001193125-26-460951-index.htm> requested 2026-11-16T11:12:37Z, responded 2026-11-16T11:12:37Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/bbgi-20261113.htm> requested 2026-11-16T11:12:38Z, responded 2026-11-16T11:12:38Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | bbgi-20261113.htm iXBRL | 8-K | 47755 |
| 2 | EX-99.1 | bbgi-ex99_1.htm | EX-99.1 | 716682 |
| 3 | GRAPHIC | img101118723_0.jpg | GRAPHIC | 27602 |
|  | Complete submission text file | 0001193125-26-460951.txt |  | 934901 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Beasley Broadcast Group, Inc. issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — Exhibit Number Description 99.1 Press Release dated November 13, 2026 issued by Beasley Broadcast Group, Inc. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 24. Health In Tech, Inc. — `0001213900-26-119857`

CIK 0002019505, form 8-K, feed items 2.02, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/2019505/000121390026119857/0001213900-26-119857-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2019505/000121390026119857/ea0311991-8k_health.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/2019505/000121390026119857/0001213900-26-119857-index.htm> requested 2026-11-16T11:12:39Z, responded 2026-11-16T11:12:39Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/2019505/000121390026119857/ea0311991-8k_health.htm> requested 2026-11-16T11:12:40Z, responded 2026-11-16T11:12:41Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0311991-8k_health.htm iXBRL | 8-K | 29918 |
| 2 | PRESS RELEASE DATED NOVEMBER 12, 2026 | ea031199101ex99-1.htm | EX-99.1 | 166493 |
|  | Complete submission text file | 0001213900-26-119857.txt |  | 385445 |

- Item 2.02 Results of Operations and Financial Condition. — On November 12, 2026, Health In Tech, Inc., a Nevada corporation (the “Company”) issued a press release announcing its results of operations for the quarter ended September 30, 2026, attached hereto as Exhibit 99.1.
- Item 7.01 Regulation FD Disclosure. — As disclosed in Item 2.02 above, on November 12, 2026, the Company issued a press release announcing its results of operations for the quarter ended September 30, 2026, attached hereto as Exhibit 99.1.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits: Exhibit No. Description 99.1 Press release dated November 12, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) 1

### 25. NATIONAL HEALTH INVESTORS INC — `0000877860-26-000230`

CIK 0000877860, form 8-K, feed items 5.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/877860/000087786026000230/0000877860-26-000230-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/877860/000087786026000230/nhi-20261109.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/877860/000087786026000230/0000877860-26-000230-index.htm> requested 2026-11-16T11:12:41Z, responded 2026-11-16T11:12:42Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/877860/000087786026000230/nhi-20261109.htm> requested 2026-11-16T11:12:42Z, responded 2026-11-16T11:12:43Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | nhi-20261109.htm iXBRL | 8-K | 28266 |
| 2 | EX-10.1 | exhibit101to8-k502.htm | EX-10.1 | 84730 |
|  | Complete submission text file | 0000877860-26-000230.txt |  | 249449 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, National Health Investors, Inc. (the “Company”) entered into an Indemnification Agreement (each, an “Indemnification Agreement”) with each of the Company’s directors and certain of the Company’s officers, including each of the Company’s executive officers. Each of the Indemnification Agreements obligates the Company to indemnify the directors and officers to the maximum extent permitted by Maryland law.
- Item 9.01 Financial Statements and Exhibits. — Exhibit Index Number Exhibit 10.1 Form of Indemnification Agreement 104 Cover Page Interactive Data File (formatted as inline XBRL and contained in Exhibit 101). ..

### 26. DocGo Inc. — `0001628280-26-073911`

CIK 0001822359, form 8-K, feed items 5.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/0001628280-26-073911-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/dcgo-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/0001628280-26-073911-index.htm> requested 2026-11-16T11:12:43Z, responded 2026-11-16T11:12:44Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/dcgo-20261113.htm> requested 2026-11-16T11:12:45Z, responded 2026-11-16T11:12:45Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | dcgo-20261113.htm iXBRL | 8-K | 33541 |
| 2 | EX-10.1 | ceotransitionservicessepar.htm | EX-10.1 | 121390 |
|  | Complete submission text file | 0001628280-26-073911.txt |  | 299936 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — As previously announced, DocGo Inc. (the “Company”) is conducting a search for a new Chief Executive Officer as the employment agreement of the Company’s current CEO, Lee Bienstock, expires December 31, 2026. On November 13, 2026, the Company and Mr. Bienstock entered into a Transition Services and Separation Agreement (the “Transition Agreement”), pursuant to which Mr. Bienstock will continue to serve as the Company’s Chief Executive Officer (“CEO”) and provide assistance in transitioning the role from January 1, 2027 through March 31, 2027, or such later date as may mutually be agreed by the parties (the “Transition Period”). If a successor CEO commences employment prior to March 31, 2027 (the “Separation Date”), Mr. Bienstock will continue to serve as a senior advisor to the board and the successor CEO through the Separation Date. As consideration for his continued service during the Transition Period and subject to the terms of the Transition Agreement, Mr. Bienstock is entitled to the following: (i) a salary of $90,000 per month, (ii) vesting in one-sixth of his outstanding equity awards that would otherwise vest in 2027 on each of January 31, February 28, and March 31, 2027, and if the Transition Agreement is extended, on each month end thereafter during the extension period, (iii) remaining eligible to participate in the Company’s employee benefit programs, and (iv) in accordance with the severance benefits of his current employment agreement, an annual bonus with respect to 2026 performance no later than March 15, 2027, determined and payable in accordance with the Company’s previously adopted bonus metrics.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Transition Services and Separation Agreement, dated November 13, 2026, by and between the Company and Lee Bienstock 104 Cover Page Interactive Data File (formatted as Inline XBRL).

### 27. ACCURAY INC — `0001437749-26-036943`

CIK 0001138723, form 8-K, feed items 3.02, 3.03, 5.03, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/0001437749-26-036943-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/aray20261111_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/0001437749-26-036943-index.htm> requested 2026-11-16T11:12:46Z, responded 2026-11-16T11:12:46Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/aray20261111_8k.htm> requested 2026-11-16T11:12:47Z, responded 2026-11-16T11:12:47Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | aray20261111_8k.htm iXBRL | 8-K | 52165 |
| 2 | EXHIBIT 3.1 | ex_1043813.htm | EX-3.1 | 149332 |
| 3 | EXHIBIT 3.2 | ex_1043814.htm | EX-3.2 | 13073 |
| 4 | EXHIBIT 3.3 | ex_1043815.htm | EX-3.3 | 13483 |
| 5 | EXHIBIT 99.1 | ex_1043816.htm | EX-99.1 | 15707 |
|  | Complete submission text file | 0001437749-26-036943.txt |  | 421462 |

- Item 3.02 Unregistered Sales of Equity Securities. — The information related to the issuance of the Series A Preferred Stock (as defined below) contained in Item 3.03 of this Current Report on Form 8-K is incorporated herein by reference.
- Item 3.03 Material Modification to Rights of Security Holders. — As previously disclosed, the Company entered into that certain Securities Purchase Agreement, dated as of July 29, 2026 (as amended to date, the “Purchase Agreement”) with certain existing investors of the Company party thereto (the “Investors”), pursuant to which the Company agreed to sell, and the Investors agreed to purchase, an aggregate of 55,000 shares of the Company’s Series A Convertible Preferred Stock, par value $0.001 per share (the “Series A Preferred Stock”), for an aggregate purchase price of $55.0 million, or $1,000 per share, comprised of $15.0 million in cash and the conversion of $40.0 million of existing indebtedness held by the Investors. On November 12, 2026, the Company filed the Certificate of Designations, Preferences and Rights of Series A Convertible Preferred Stock (the “Certificate of Designations”) with the Secretary of State of the State of Delaware to establish the preferences, limitations and relative rights of the Series A Preferred Stock. The shares of Series A Preferred Stock were issued on November 13, 2026 in connection with the closing of the transactions contemplated by the Purchase Agreement. The Series A Preferred Stock ranks senior to the Company’s common stock, par value $0.001 per share (the “Common Stock”) with respect to dividend rights and rights on the distribution of assets on any voluntary or involuntary liquidation, dissolution or winding up of the affairs of the Company. Preferential dividends accrue on the Series A Preferred Stock at a rate of 8% per annum on the then-current stated value of each share (initially $1,000 per share) and compound quarterly to the extent not paid (the “Accruing Dividends”).
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — As previously disclosed, on November 4, 2026, the Company announced that its board of directors had selected a 1-for-40 ratio for the previously approved reverse stock split of the Common Stock. On November 6, 2026, the Company filed two certificates of amendment to the Company’s Amended and Restated Certificate of Incorporation with the Secretary of State of the State of Delaware to (i) increase the number of authorized shares of Common Stock of the Company from 200,000,000 to 400,000,000 (which resulted in an increase in the total number of authorized shares of the Company’s capital stock from 205,000,000 to 405,000,000) (the “Authorized Shares Increase Amendment”), and (ii) effect a reverse stock split (the “Reverse Stock Split”) of the issued and outstanding Common Stock, at a ratio of 1-for-40, and a corresponding decrease to the authorized number of shares of Common Stock (and, as a result, a reduction in the total authorized shares) (the “Reverse Stock Split Amendment”), as described in the Company’s definitive proxy statement filed with the Securities and Exchange Commission on August 24, 2026 and the Company’s amendment to the definitive proxy statement filed with the Securities and Exchange Commission on September 18, 2026, and each as approved by the Company’s stockholders at the Special Meeting of Stockholders held on October 6, 2026. The Authorized Shares Increase Amendment became effective as of November 9, 2026 at 12:01 a.m., Eastern Time. The Reverse Stock Split Amendment became effective as of November 9, 2026 at 12:02 a.m., Eastern Time (the “Effective Time”). Beginning on November 9, 2026, the Common Stock began trading on The Nasdaq Capital Market on a split-adjusted basis under the existing symbol ARAY, with the new CUSIP number 004397 303.
- Item 7.01 Regulation FD Disclosure — Canceled Warrants In connection with the closing of the Purchase Agreement, certain outstanding warrants were automatically canceled and extinguished (the “Canceled Warrants”). The Canceled Warrants previously provided the holders thereof the right to purchase, prior to giving effect to the Reverse Stock Split, an aggregate of approximately 27.6 million shares of Common Stock held by the Investors, consisting of (i) warrants exercisable for an aggregate of approximately 17.2 million shares of Common Stock at $1.68 per share on and after December 7, 2025 until June 6, 2032, (ii) warrants exercisable for an aggregate of approximately 3.1 million shares of Common Stock at $1.50 per share on and after June 16, 2026 until December 15, 2032, (iii) warrants exercisable for an aggregate of approximately 2.2 million shares of Common Stock at $1.25 per share on and after June 16, 2026 until December 15, 2032, (iv) warrants exercisable for an aggregate of approximately 3.0 million shares of Common Stock at $1.50 per share on and after November 19, 2026 until May 18, 2033, and (v) warrants exercisable for an aggregate of approximately 2.1 million shares of Common Stock at $1.25 per share on an after November 19, 2026 until May 18, 2033. Press Release On November 13, 2026, the Company issued a press release announcing the Authorized Shares Increase Amendment, the Reverse Stock Split Amendment, and the issuance of the Series A Preferred Stock.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 3.1 Certificate of Designations, Preferences and Rights of Series A Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective November 12, 2026 3.2 Certificate of Amendment to the Amended and Restated Certificate of Incorporation of Accuray Incorporated, increasing the number of authorized shares of Common Stock 3.3 Certificate of Amendment to the Amended and Restated Certificate of Incorporation of Accuray Incorporated, effecting the Reverse Stock Split 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 28. Contango Silver & Gold Inc. — `0001104659-26-127202`

CIK 0001502377, form 8-K, feed items 1.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/0001104659-26-127202-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/tm2629486d1_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/0001104659-26-127202-index.htm> requested 2026-11-16T11:12:48Z, responded 2026-11-16T11:12:49Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/tm2629486d1_8k.htm> requested 2026-11-16T11:12:49Z, responded 2026-11-16T11:12:50Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629486d1_8k.htm iXBRL | 8-K | 30927 |
| 2 | EXHIBIT 1.1 | tm2629486d1_ex1-1.htm | EX-1.1 | 337096 |
| 3 | EXHIBIT 5.1 | tm2629486d1_ex5-1.htm | EX-5.1 | 9222 |
| 7 | GRAPHIC | tm2629486d1_ex5-1img001.jpg | GRAPHIC | 2564 |
|  | Complete submission text file | 0001104659-26-127202.txt |  | 626541 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 13, 2026, Contango Silver & Gold Inc. (the “Company”) entered into a Controlled Equity OfferingSM Sales Agreement (the “Sales Agreement”) with Cantor Fitzgerald & Co. (the “Lead Agent”) and ATB Capital Markets USA Inc., BTIG, LLC, Canaccord Genuity LLC, Haywood Securities Inc., National Bank Financial Inc., Freedom Capital Markets, Maxim Group LLC, and Research Capital USA Inc. (the “Co-Agents” and, collectively with the Lead Agent, the “Agents”) , pursuant to which the Company may offer and sell from time to time shares of the Company’s common stock, par value $0.01 per share (the “Shares”), having an aggregate offering price of up to $75,000,000 through the Agents. The Company will pay the Agents a commission of up to 3.00% of the gross proceeds from each sale of Shares made through the Agents pursuant to the Sales Agreement.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description of Exhibit 1.1 Controlled Equity OfferingSM Sales Agreement, dated November 13, 2026, by and between Contango Silver & Gold Inc. and Cantor Fitzgerald & Co., ATB Capital Markets USA Inc., BTIG, LLC, Canaccord Genuity LLC, Haywood Securities Inc., National Bank Financial Inc., Freedom Capital Markets, Maxim Group LLC, and Research Capital USA Inc. 5.1 Opinion of Cozen O’Connor. 23.1 Consent of Cozen O’Connor (contained in Exhibit 5.1). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 29. SOUNDHOUND AI, INC. — `0001213900-26-119843`

CIK 0001840856, form 8-K, feed items 5.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/0001213900-26-119843-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/ea0312272-8k_sound.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/0001213900-26-119843-index.htm> requested 2026-11-16T11:12:50Z, responded 2026-11-16T11:12:51Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/ea0312272-8k_sound.htm> requested 2026-11-16T11:12:51Z, responded 2026-11-16T11:12:52Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312272-8k_sound.htm iXBRL | 8-K | 32861 |
|  | Complete submission text file | 0001213900-26-119843.txt |  | 243559 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Effective November 9, 2026, Tyler Moore assumed the role of principal accounting officer of SoundHound AI, Inc. (the “Company”). Mr. Tyler was previously hired as Executive Vice President, Chief Accounting Officer of the Company on November 2, 2026, pursuant to an offer letter dated October 26, 2026 (the “Offer Letter”). Mr. Moore succeeds John Collins, the Company’s Chief Financial Officer, who had served as principal accounting officer in addition to his role as Chief Financial Officer. Mr. Collins will continue to serve as the Company’s Chief Financial Officer and principal financial officer. Compensatory Arrangements Pursuant to the Offer Letter, Mr. Moore will receive an annual base salary of $345,000. He is eligible for an annual bonus under the Company’s discretionary executive bonus plan, with a target of up to 40% of base salary. In addition, Mr. Moore received a grant of 100,000 restricted stock units (“RSUs”) which vest in equal monthly installments over four years from his start date, subject to his continued service, and also received 50,000 performance stock units (“PSUs”) that will vest upon completion of certain performance criteria.
- Item 9.01 Financial Statement and Exhibits. Exhibit Number — Description 104 Cover Page Interactive Data File (formatted as inline XBRL)

### 30. NextBoat Inc. — `0001493152-26-051809`

CIK 0002067767, form 8-K, feed items 1.01, 2.03, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/0001493152-26-051809-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/0001493152-26-051809-index.htm> requested 2026-11-16T11:12:52Z, responded 2026-11-16T11:12:53Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/form8-k.htm> requested 2026-11-16T11:12:54Z, responded 2026-11-16T11:12:54Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 42917 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 83884 |
|  | Complete submission text file | 0001493152-26-051809.txt |  | 313128 |

- Item 1.01 Entry into a Material Definitive Agreement. — Lease of Cape Fear Marina Boat Slips On November 4, 2026, Off The Hook Yacht Sales NC, LLC, (“OTH NC”), a North Carolina limited liability company and a wholly owned subsidiary of NextBoat Inc. (the “Company”), entered into a triple-net lease (the “Lease”) with Hadley Harbor Group LLC (the “Landlord”) for 22 boat slips at Cape Fear Marina in Wilmington, North Carolina. In connection with the Lease, the Company guaranteed the obligations of OTH NC pursuant to Section 36 of the Lease (the “Guaranty”). The Lease has a term of seven years commencing on November 4, 2026, and does not provide OTH NC with an option to renew. Initial base rent is $8,950 per month ($107,400 per year), increasing by 3% annually. As a triple-net lease, OTH NC is responsible for association dues, property taxes, insurance, utilities and maintenance relating to the slips. The Landlord is controlled by Zebulon Z. Hadley IV, a director of the Company, through the Zebulon Z. Hadley IV Revocable Trust. The Landlord acquired the slips subject to the Lease from OTH Realty, LLC, an entity wholly owned by Jason Ruegg, the Chairman of the Board of Directors of the Company (the “Board”) and the Company’s principal stockholder, and from Mr. Ruegg individually, for an aggregate purchase price of $1,400,000. As a result, each of Mr. Hadley and Mr. Ruegg has a direct or indirect financial interest in the Lease. Aggregate base rent payable over the seven-year term of the Lease is approximately $822,948, exclusive of triple-net charges. The Lease is a related person transaction under Item 404 of Regulation S-K. On October 15, 2026, the disinterested members of the Audit Committee of the Board, with Mr. Hadley abstaining, reviewed the Lease and the Guaranty on the terms of the draft presented to them, determined that they were fair to, and in the best interests of, the Company and its stockholders, and recommended their approval by the disinterested members of the Board.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth in Item 1.01 of this Current Report on Form 8-K is incorporated by reference into this Item 2.03.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit Number Exhibits 10.1* Lease, dated November 4, 2026, by and between Off The Hook Yacht Sales NC, LLC and Hadley Harbor Group LLC, including the guaranty by NextBoat Inc. set forth in Section 36 thereof. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). * Certain schedules and exhibits have been omitted pursuant to Item 601(a)(5) of Regulation S-K, and certain personal information has been excluded pursuant to Item 601(a)(6) of Regulation S-K. The Company agrees to furnish supplementally a copy of any omitted schedule or exhibit to the Securities and Exchange Commission upon request.

### 31. Co-Diagnostics, Inc. — `0001493152-26-051811`

CIK 0001692415, form 8-K, feed items 5.02, 5.07, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/0001493152-26-051811-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/0001493152-26-051811-index.htm> requested 2026-11-16T11:12:55Z, responded 2026-11-16T11:12:55Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/form8-k.htm> requested 2026-11-16T11:12:56Z, responded 2026-11-16T11:12:56Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 75533 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 16678 |
|  | Complete submission text file | 0001493152-26-051811.txt |  | 264278 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, Co-Diagnostics, Inc. (the “Company”) held a court-ordered special meeting of shareholders (the “Special Meeting”). At the Special Meeting, the Company’s shareholders approved Amendment No. 1 (the “Plan Amendment”) to the Co-Diagnostics, Inc. 2025 Equity Incentive Plan (the “Plan”). The Plan Amendment increases the number of shares of the Company’s common stock, par value $0.001 per share (“Common Stock”), authorized for issuance under the Plan by 2,000,000 shares. As amended, the Plan provides that, subject to adjustment as provided in the Plan, the maximum number of shares of Common Stock that may be issued or transferred under awards granted under the Plan is 2,223,333 shares. The Plan Amendment also sets the maximum number of shares of Common Stock that may be issued on the exercise of incentive stock options granted under the Plan at 2,223,333 shares, subject to adjustment as provided in the Plan.
- Item 5.07 Submission of Matters to a Vote of Security Holders — On November 13, 2026, the Company held a Special Meeting of shareholders at which the following matters were voted on: Proposal No. 1: Election of Directors. The Company’s shareholders elected for a one-year term each of the persons nominated for election as a director. The following table sets forth the vote of the shareholders at the meeting with respect to the election of directors: Nominee Votes For Votes Withheld Broker Non-votes Dwight Egan 1,280,609 314,073 2,092,364 Eugene Durenard 1,461,469 133,213 2,092,364 Richard Serbin 1,461,461 133,221 2,092,364 James Nelson 1,459,292 135,390 2,092,364 Edward Murphy 1,447,019 147,663 2,092,364 There were no abstentions with respect to the election of directors. Proposal No. 2: A proposal to approve an increase in the number of shares of common stock authorized for issuance under the Company’s Co-Diagnostics, Inc. 2025 Equity Incentive Plan, as described in the Proxy Statement. This proposal was adopted. For Against Abstain Broker Non-votes 1,017,401 571,209 6,072 2,092,364 Proposal No. 3: A proposal to adopt, on an advisory basis, a non-binding resolution approving the compensation of the Company’s named executive officers, as described in the Proxy Statement under “Executive Compensation.” This proposal was adopted. For Against Abstain Broker Non-votes 1,099,440 486,505 8,737 2,092,364 Proposal No. 4: A proposal to ratify the Audit Committee’s appointment of Tanner LLC as the Company’s independent registered public accounting firm for the year ending December 31, 2026. This proposal was ratified.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 10.1# Amendment No. 1 to the Co-Diagnostics, Inc. 2025 Equity Incentive Plan 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) # Indicates a management contract or compensatory plan or arrangement.

### 32. Beyond Air, Inc. — `0001493152-26-051810`

CIK 0001641631, form 8-K, feed items 2.02, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/0001493152-26-051810-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/0001493152-26-051810-index.htm> requested 2026-11-16T11:12:57Z, responded 2026-11-16T11:12:58Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/form8-k.htm> requested 2026-11-16T11:12:58Z, responded 2026-11-16T11:12:59Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 39740 |
| 2 | EX-99.1 | ex99-1.htm | EX-99.1 | 101589 |
|  | Complete submission text file | 0001493152-26-051810.txt |  | 320242 |

- Item 2.02 Results of Operations and Financial Condition. — On November 11, 2026, Beyond Air, Inc. (the “Company”) issued a press release announcing financial results for its fiscal quarter ended September 30, 2026, and certain recent corporate developments.
- Item 7.01 Regulation FD Disclosure. — The information under Item 2.02 above is incorporated herein by reference.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit No. Description 99.1 Press Release from Beyond Air, Inc., dated as of November 11, 2026. 104 Cover Page Interactive Data File (embedded within the inline XBRL document).

### 33. Q/C TECHNOLOGIES, INC. — `0001493152-26-051808`

CIK 0001321834, form 8-K, feed items 3.01. Index: <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/0001493152-26-051808-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/0001493152-26-051808-index.htm> requested 2026-11-16T11:12:59Z, responded 2026-11-16T11:13:00Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/form8-k.htm> requested 2026-11-16T11:13:00Z, responded 2026-11-16T11:13:01Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 36100 |
|  | Complete submission text file | 0001493152-26-051808.txt |  | 201574 |

- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 6, 2026, Q/C Technologies, Inc. (the “Company”) received a letter from the Listing Qualifications staff of The Nasdaq Stock Market (“Nasdaq”) notifying the Company that, based on the closing bid price of the Company’s common stock for the last 30 consecutive business days from September 25, 2026 to November 5, 2026, the Company no longer meets the continued listing requirement of Nasdaq under Nasdaq Listing Rule 5550(a)(2) to maintain a minimum bid price of $1.00 per share. Nasdaq has provided the Company with a 180 calendar day compliance period, or until May 5, 2027, in which to regain compliance with Nasdaq’s continued listing requirement. In the event that the Company does not regain compliance in the compliance period, the Company may be eligible for an additional 180 calendar days, should the Company meet the continued listing requirement for market value of publicly held shares and all other initial listing standards for The Nasdaq Capital Market, with the exception of the bid price requirement, and is able to provide written notice of its intention to cure the deficiency during the second compliance period, by effecting a reverse stock split, if necessary. The Company is currently evaluating options to regain compliance and intends to timely regain compliance with Nasdaq’s continued listing requirement.

### 34. BRC Group Holdings, Inc. — `0001213900-26-119839`

CIK 0001464790, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/0001213900-26-119839-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/ea0312286-8k_brcgroup.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/0001213900-26-119839-index.htm> requested 2026-11-16T11:13:01Z, responded 2026-11-16T11:13:02Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/ea0312286-8k_brcgroup.htm> requested 2026-11-16T11:13:03Z, responded 2026-11-16T11:13:03Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312286-8k_brcgroup.htm iXBRL | 8-K | 36147 |
|  | Complete submission text file | 0001213900-26-119839.txt |  | 269607 |

- Item 5.02 (b) Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Effective November 16, 2026, BRC Group Holdings, Inc. (the “Company”) will eliminate the Chief Accounting Officer role as the Company does not believe this separate role is necessary for operations. As a result, Mr. Howard Weitzman will no longer serve as Chief Accounting Officer. Mr. Weitzman will remain with the Company as the Head of Corporate Tax. In his new role, Mr. Weitzman will no longer be a Section 16 or executive officer.

### 35. Evofem Biosciences, Inc. — `0001493152-26-051806`

CIK 0001618835, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/0001493152-26-051806-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/form8-k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/0001493152-26-051806-index.htm> requested 2026-11-16T11:13:04Z, responded 2026-11-16T11:13:05Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/form8-k.htm> requested 2026-11-16T11:13:05Z, responded 2026-11-16T11:13:06Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 39864 |
| 2 | EX-99.1 | ex99-1.htm | EX-99.1 | 66205 |
| 3 | GRAPHIC | ex99-1_001.jpg | GRAPHIC | 14300 |
|  | Complete submission text file | 0001493152-26-051806.txt |  | 296023 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Evofem Biosciences, Inc. (the “Company”) issued a press release announcing its financial results for the three and nine months ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

### 36. Seritage Growth Properties — `0001193125-26-460888`

CIK 0001628063, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1628063/000119312526460888/0001193125-26-460888-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1628063/000119312526460888/srg-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1628063/000119312526460888/0001193125-26-460888-index.htm> requested 2026-11-16T11:13:07Z, responded 2026-11-16T11:13:08Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1628063/000119312526460888/srg-20261113.htm> requested 2026-11-16T11:13:08Z, responded 2026-11-16T11:13:09Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | srg-20261113.htm iXBRL | 8-K | 52534 |
| 2 | EX-99.1 | srg-ex99_1.htm | EX-99.1 | 454474 |
| 3 | GRAPHIC | img42621_0.jpg | GRAPHIC | 8154 |
|  | Complete submission text file | 0001193125-26-460888.txt |  | 676522 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13 2026, the Company issued a press release regarding its financial results for the three and nine months ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within Inline XBRL document)

### 37. CERENOME, INC. — `0001193125-26-460887`

CIK 0001095981, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/0001193125-26-460887-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/cnsy-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/0001193125-26-460887-index.htm> requested 2026-11-16T11:13:10Z, responded 2026-11-16T11:13:10Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/cnsy-20261113.htm> requested 2026-11-16T11:13:11Z, responded 2026-11-16T11:13:12Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | cnsy-20261113.htm iXBRL | 8-K | 52522 |
| 2 | EX-99.1 | cnsy-ex99_1.htm | EX-99.1 | 531409 |
|  | Complete submission text file | 0001193125-26-460887.txt |  | 722095 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Cerenome, Inc. (the “Company”) reported financial results for the third quarter ended September 30, 2026 and other recent corporate updates.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. Exhibit Number Description 99.1 Press Release Announcing Financial Results, dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 38. Apollo Global Management, Inc. — `0001193125-26-460879`

CIK 0001858681, form 8-K, feed items 1.01, 2.03, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/0001193125-26-460879-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/d143669d8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/0001193125-26-460879-index.htm> requested 2026-11-16T11:13:12Z, responded 2026-11-16T11:13:13Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/d143669d8k.htm> requested 2026-11-16T11:13:14Z, responded 2026-11-16T11:13:15Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d143669d8k.htm iXBRL | 8-K | 33954 |
| 2 | EX-1.1 | d143669dex11.htm | EX-1.1 | 184116 |
| 3 | EX-4.1 | d143669dex41.htm | EX-4.1 | 537287 |
| 4 | EX-5.1 | d143669dex51.htm | EX-5.1 | 17167 |
| 9 | GRAPHIC | g143669dsp39.jpg | GRAPHIC | 6101 |
|  | Complete submission text file | 0001193125-26-460879.txt |  | 1094528 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 13, 2026, Apollo Global Management, Inc. (the “Company”) issued $600,000,000 aggregate principal amount of its 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056 (the “Notes”), pursuant to a previously announced underwritten public offering (the “Offering”). The Notes will bear interest at a fixed rate of 7.550% per year until December 15, 2036 (the “First Reset Date”). On and after the First Reset Date, the interest rate on the Notes for each Reset Period (as defined in the Indenture) will be equal to the Five-Year U.S. Treasury Rate (as defined in the Indenture) as of the most recent Reset Interest Determination Date (as defined in the Indenture) plus a spread of 2.672%. The Company intends to use the net proceeds from the Offering for general corporate purposes, including to fund the previously announced investment in Mubadala Capital Asset Management.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 2.03.
- Item 8.01 Other Events. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 8.01. Underwriting Agreement In connection with the issuance and sale of the Notes, the Company entered into an underwriting agreement, dated November 9, 2026 (the “Underwriting Agreement”), with J.P. Morgan Securities LLC, BofA Securities, Inc., Morgan Stanley & Co. LLC and Wells Fargo Securities, LLC, as representatives of the several underwriters named therein, relating to the Notes. The Underwriting Agreement is filed as Exhibit 1.1 hereto and is incorporated by reference herein. Opinion of Counsel The opinion of Paul, Weiss, Rifkind, Wharton & Garrison LLP, relating to the validity of the Notes and the related guarantees, is filed as Exhibit 5.1 hereto and is incorporated by reference into the Registration Statement.
- Item 9.01 Financial Statements and Exhibits. — The exhibits to this Current Report on Form 8-K (except Exhibit 104) are hereby incorporated by reference into the Registration Statement. (d) Exhibits. Exhibit No. Description 1.1 Underwriting Agreement, dated as of November 9, 2026, among Apollo Global Management, Inc. and J.P. Morgan Securities LLC, BofA Securities, Inc., Morgan Stanley & Co. LLC and Wells Fargo Securities, LLC, as representatives of the underwriters named therein, relating to the 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056. 4.1 Indenture, dated as of November 13, 2026, among Apollo Global Management, Inc., the guarantors named therein and U.S. Bank Trust Company, National Association, as trustee. 4.2 Form of 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056 (included in Exhibit 4.1). 5.1 Opinion of Paul, Weiss, Rifkind, Wharton & Garrison LLP with respect to the 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056. 23.1 Consent of Paul, Weiss, Rifkind, Wharton & Garrison LLP (included in Exhibit 5.1) 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 39. American Strategic Investment Co. — `0001628280-26-073897`

CIK 0001595527, form 8-K, feed items 2.02, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/0001628280-26-073897-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/nycr-20261113.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/0001628280-26-073897-index.htm> requested 2026-11-16T11:13:15Z, responded 2026-11-16T11:13:16Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/nycr-20261113.htm> requested 2026-11-16T11:13:16Z, responded 2026-11-16T11:13:17Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | nycr-20261113.htm iXBRL | 8-K | 34540 |
| 2 | EX-99.1 | ex991-asicearningsrelease9.htm | EX-99.1 | 156786 |
| 3 | EX-99.2 | ex992-asicsupplementalinfo.htm | EX-99.2 | 384300 |
| 8 |  | picture1.jpg | GRAPHIC | 103415 |
|  | Complete submission text file | 0001628280-26-073897.txt |  | 921896 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, American Strategic Investment Co. (the “Company”) issued a press release announcing its results of operations for the quarter ended September 30, 2026, and supplemental financial information for the quarter ended September 30, 2026, attached hereto as Exhibits 99.1 and 99.2, respectively.
- Item 7.01 Regulation FD Disclosure. — As disclosed in Item 2.02 above, on November 13, 2026, the Company issued a press release announcing its results of operations for the quarter ended September 30, 2026, and supplemental financial information for the quarter ended September 30, 2026, attached hereto as Exhibits 99.1 and 99.2, respectively.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release dated November 13, 2026 99.2 Supplemental information for the quarter ended September 30, 2026 104 Cover Page Interactive Data File - the cover page XBRL tags are embedded within the Inline XBRL document

### 40. QUALCOMM INC/DE — `0001104659-26-127163`

CIK 0000804328, form 8-K, feed items 1.01, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/804328/000110465926127163/0001104659-26-127163-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/804328/000110465926127163/tm2629667d1_8k.htm>.

Requests (UTC, recorded at fetch time): index page <https://www.sec.gov/Archives/edgar/data/804328/000110465926127163/0001104659-26-127163-index.htm> requested 2026-11-16T11:13:18Z, responded 2026-11-16T11:13:19Z, HTTP 200; document <https://www.sec.gov/Archives/edgar/data/804328/000110465926127163/tm2629667d1_8k.htm> requested 2026-11-16T11:13:19Z, responded 2026-11-16T11:13:20Z, HTTP 200.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629667d1_8k.htm iXBRL | 8-K | 36308 |
| 2 | EXHIBIT 1.1 | tm2629667d1_ex1-1.htm | EX-1.1 | 214570 |
| 3 | EXHIBIT 4.2 | tm2629667d1_ex4-2.htm | EX-4.2 | 45157 |
| 4 | EXHIBIT 4.3 | tm2629667d1_ex4-3.htm | EX-4.3 | 36504 |
| 5 | EXHIBIT 4.4 | tm2629667d1_ex4-4.htm | EX-4.4 | 36708 |
| 6 | EXHIBIT 4.5 | tm2629667d1_ex4-5.htm | EX-4.5 | 36796 |
| 7 | EXHIBIT 4.6 | tm2629667d1_ex4-6.htm | EX-4.6 | 35867 |
| 8 | EXHIBIT 4.7 | tm2629667d1_ex4-7.htm | EX-4.7 | 36779 |
| 9 | EXHIBIT 5.1 | tm2629667d1_ex5-1.htm | EX-5.1 | 12420 |
| 13 | GRAPHIC | tm2629667d1_ex5-1img01.jpg | GRAPHIC | 2186 |
|  | Complete submission text file | 0001104659-26-127163.txt |  | 765460 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 12, 2026, QUALCOMM Incorporated (the Company) executed an Officers’ Certificate (the Officers’ Certificate), in accordance with Sections 2.02, 2.03, 10.04 and 10.05 of the Indenture dated May 20, 2015 (the Base Indenture and, together with the Officers’ Certificate, the Indenture) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the Trustee), in connection with the sale of $750,000,000 in aggregate principal amount of the Company’s 5.000% Notes due 2028 (the 2028 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.150% Notes due 2029 (the 2029 Notes), $1,000,000,000 in aggregate principal amount of the Company’s 5.350% Notes due 2031 (the 2031 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.600% Notes due 2033 (the 2033 Notes) and $750,000,000 in aggregate principal amount of the Company’s 5.800% Notes due 2036 (the 2036 Notes and, together with the 2028 Notes, the 2029 Notes, the 2031 Notes and the 2033 Notes, the Notes).
- Item 8.01 Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the Underwriting Agreement) with BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P. Morgan Securities LLC and Morgan Stanley & Co. LLC, on behalf of the several Underwriters listed in Schedule I thereto (the Underwriters), pursuant to which the Company agreed to issue and sell the Notes to the Underwriters in a registered public offering (the Offering). The Offering was pursuant to the Company’s shelf registration statement on Form S-3 (Registration File No. 333-283035), filed with the SEC on November 6, 2024.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No Description 1.1 Underwriting Agreement, dated November 9, 2026, among QUALCOMM Incorporated, BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P. Morgan Securities LLC and Morgan Stanley & Co. LLC 4.1 Indenture, dated May 20, 2015, between QUALCOMM Incorporated and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (incorporated herein by reference to Exhibit 4.1 to QUALCOMM Incorporated’s Current Report on Form 8-K filed with the SEC on May 21, 2015) 4.2 Officers’ Certificate, dated November 12, 2026 for the 2028 Notes, the 2029 Notes, the 2031 Notes, the 2033 Notes and the 2036 Notes 4.3 Form of 2028 Notes 4.4 Form of 2029 Notes 4.5 Form of 2031 Notes 4.6 Form of 2033 Notes 4.7 Form of 2036 Notes 5.1 Opinion of Sidley Austin LLP, relating to the Notes (including the consent required with respect thereto) 104 Cover Page Interactive Data File, formatted in Inline XBRL and included as Exhibit

## Changes

### PULL 2 vs PULL 1

- Earlier (PULL 1): 198 rows; later (PULL 2): 197 rows.
- New: 197; gone: 198; changed: 0.
- Check: later = earlier + new − gone → 197 = 198 + 197 − 198 (True).

New accessions (in later pull only):

- `0000017843-26-000052`
- `0000025232-26-000082`
- `0000048465-26-000065`
- `0000067716-26-000089`
- `0000074208-26-000090`
- `0000076605-26-000113`
- `0000080420-26-000139`
- `0000106535-26-000015`
- `0000350852-26-000079`
- `0000715072-26-000092`
- `0000716634-26-000042`
- `0000776901-26-000174`
- `0000795266-26-000080`
- `0000911147-26-000055`
- `0000912593-26-000286`
- `0000926617-26-000058`
- `0000950142-26-003058`
- `0000950157-26-001261`
- `0001053507-26-000167`
- `0001062993-26-006086`
- `0001072613-26-000900`
- `0001079973-26-001517`
- `0001079973-26-001525`
- `0001087294-26-000086`
- `0001087294-26-000087`
- `0001096906-26-001785`
- `0001096906-26-001789`
- `0001099219-26-000064`
- `0001104659-26-128139`
- `0001104659-26-128140`
- `0001104659-26-128161`
- `0001104659-26-128251`
- `0001104659-26-128260`
- `0001104659-26-128272`
- `0001104659-26-128282`
- `0001104659-26-128300`
- `0001104659-26-128328`
- `0001104659-26-128336`
- `0001104659-26-128338`
- `0001104659-26-128350`
- `0001104659-26-128377`
- `0001104659-26-128406`
- `0001104659-26-128450`
- `0001104659-26-128453`
- `0001104659-26-128485`
- `0001104659-26-128533`
- `0001104659-26-128553`
- `0001104659-26-128565`
- `0001104659-26-128573`
- `0001104659-26-128592`
- `0001140361-26-044139`
- `0001140361-26-044210`
- `0001140361-26-044219`
- `0001185185-26-005466`
- `0001193125-26-463071`
- `0001193125-26-463356`
- `0001193125-26-463384`
- `0001193125-26-463400`
- `0001193125-26-463409`
- `0001193125-26-463442`
- `0001193125-26-463444`
- `0001193125-26-463447`
- `0001193125-26-463453`
- `0001193125-26-463456`
- `0001193125-26-463461`
- `0001193125-26-463483`
- `0001193125-26-463495`
- `0001193125-26-463506`
- `0001193125-26-463508`
- `0001193125-26-463553`
- `0001193125-26-463554`
- `0001193125-26-463558`
- `0001193125-26-463559`
- `0001193125-26-463573`
- `0001193125-26-463583`
- `0001193125-26-463591`
- `0001193125-26-463597`
- `0001193125-26-463626`
- `0001193125-26-463696`
- `0001193125-26-463704`
- `0001193125-26-463733`
- `0001193125-26-463741`
- `0001193125-26-463781`
- `0001193125-26-463865`
- `0001193125-26-463901`
- `0001213900-26-120471`
- `0001213900-26-120540`
- `0001213900-26-120603`
- `0001213900-26-120608`
- `0001213900-26-120624`
- `0001213900-26-120625`
- `0001213900-26-120720`
- `0001213900-26-120724`
- `0001213900-26-120734`
- `0001213900-26-120737`
- `0001213900-26-120793`
- `0001213900-26-120816`
- `0001213900-26-120828`
- `0001214659-26-014423`
- `0001214659-26-014450`
- `0001298675-26-000052`
- `0001298946-26-000052`
- `0001306830-26-000136`
- `0001437749-26-037155`
- `0001437749-26-037158`
- `0001437749-26-037162`
- `0001437749-26-037166`
- `0001437749-26-037172`
- `0001437749-26-037175`
- `0001437749-26-037176`
- `0001437749-26-037179`
- `0001437749-26-037194`
- `0001437749-26-037201`
- `0001437749-26-037204`
- `0001437749-26-037257`
- `0001437958-26-000086`
- `0001472375-26-000229`
- `0001493152-26-052288`
- `0001493152-26-052291`
- `0001493152-26-052323`
- `0001493152-26-052331`
- `0001493152-26-052332`
- `0001493152-26-052334`
- `0001493152-26-052349`
- `0001493152-26-052352`
- `0001493152-26-052377`
- `0001493152-26-052409`
- `0001493152-26-052414`
- `0001493152-26-052431`
- `0001493152-26-052451`
- `0001493152-26-052458`
- `0001493152-26-052460`
- `0001493152-26-052461`
- `0001493152-26-052466`
- `0001493152-26-052467`
- `0001493152-26-052468`
- `0001493152-26-052471`
- `0001493152-26-052478`
- `0001493152-26-052519`
- `0001493152-26-052548`
- `0001493152-26-052554`
- `0001493152-26-052559`
- `0001493152-26-052599`
- `0001500435-26-000075`
- `0001516912-26-000070`
- `0001539497-26-002999`
- `0001539497-26-003003`
- `0001600033-26-000052`
- `0001603978-26-000116`
- `0001628280-26-074089`
- `0001628280-26-074161`
- `0001628280-26-074168`
- `0001628280-26-074169`
- `0001628280-26-074184`
- `0001628280-26-074187`
- `0001628280-26-074189`
- `0001628280-26-074196`
- `0001628280-26-074199`
- `0001628280-26-074200`
- `0001628280-26-074209`
- `0001628280-26-074211`
- `0001628280-26-074213`
- `0001628280-26-074216`
- `0001628280-26-074241`
- `0001628280-26-074246`
- `0001628280-26-074264`
- `0001628280-26-074279`
- `0001628280-26-074280`
- `0001649749-26-000071`
- `0001654954-26-009844`
- `0001654954-26-009852`
- `0001654954-26-009854`
- `0001664710-26-000072`
- `0001682852-26-000208`
- `0001683168-26-008827`
- `0001683168-26-008851`
- `0001683168-26-008860`
- `0001683168-26-008861`
- `0001687229-26-000059`
- `0001718939-26-000071`
- `0001747079-26-000106`
- `0001753926-26-002153`
- `0001758766-26-000092`
- `0001758766-26-000094`
- `0001775734-26-000038`
- `0001784254-26-000054`
- `0001794783-26-000110`
- `0001801170-26-000306`
- `0001801661-26-000128`
- `0001805526-26-000177`
- `0001829126-26-012518`
- `0001835268-26-000045`
- `0001837607-26-000087`
- `0001941536-26-000038`
- `0001999371-26-025521`
- `0002015845-26-000065`
- `0002048951-26-000039`

Gone accessions (in earlier pull only):

- `0000004127-26-000058`
- `0000012659-26-000042`
- `0000353184-26-000107`
- `0000353184-26-000108`
- `0000728391-26-000053`
- `0000730464-26-000066`
- `0000763744-26-000125`
- `0000776901-26-000171`
- `0000811830-26-000057`
- `0000877860-26-000230`
- `0000879169-26-000068`
- `0000887343-26-000194`
- `0000908255-26-000075`
- `0000908255-26-000076`
- `0000913144-26-000105`
- `0001006837-26-000135`
- `0001072613-26-000891`
- `0001077428-26-000082`
- `0001079973-26-001496`
- `0001104659-26-126975`
- `0001104659-26-127041`
- `0001104659-26-127048`
- `0001104659-26-127049`
- `0001104659-26-127060`
- `0001104659-26-127061`
- `0001104659-26-127068`
- `0001104659-26-127076`
- `0001104659-26-127089`
- `0001104659-26-127094`
- `0001104659-26-127097`
- `0001104659-26-127104`
- `0001104659-26-127106`
- `0001104659-26-127108`
- `0001104659-26-127122`
- `0001104659-26-127131`
- `0001104659-26-127163`
- `0001104659-26-127202`
- `0001104659-26-127223`
- `0001104659-26-127228`
- `0001104659-26-127230`
- `0001104659-26-127233`
- `0001125345-26-000077`
- `0001140361-26-043754`
- `0001140361-26-043763`
- `0001140361-26-043782`
- `0001140361-26-043788`
- `0001140361-26-043791`
- `0001140361-26-043829`
- `0001140361-26-043831`
- `0001140361-26-043833`
- `0001171843-26-007431`
- `0001174947-26-000991`
- `0001185185-26-005387`
- `0001193125-26-460457`
- `0001193125-26-460588`
- `0001193125-26-460589`
- `0001193125-26-460597`
- `0001193125-26-460599`
- `0001193125-26-460610`
- `0001193125-26-460649`
- `0001193125-26-460653`
- `0001193125-26-460684`
- `0001193125-26-460685`
- `0001193125-26-460692`
- `0001193125-26-460698`
- `0001193125-26-460709`
- `0001193125-26-460713`
- `0001193125-26-460717`
- `0001193125-26-460732`
- `0001193125-26-460736`
- `0001193125-26-460741`
- `0001193125-26-460775`
- `0001193125-26-460798`
- `0001193125-26-460807`
- `0001193125-26-460809`
- `0001193125-26-460816`
- `0001193125-26-460843`
- `0001193125-26-460855`
- `0001193125-26-460864`
- `0001193125-26-460865`
- `0001193125-26-460879`
- `0001193125-26-460887`
- `0001193125-26-460888`
- `0001193125-26-460948`
- `0001193125-26-460951`
- `0001193125-26-461010`
- `0001193125-26-461016`
- `0001193125-26-461027`
- `0001193125-26-461028`
- `0001193125-26-461047`
- `0001213900-26-119657`
- `0001213900-26-119674`
- `0001213900-26-119681`
- `0001213900-26-119686`
- `0001213900-26-119706`
- `0001213900-26-119727`
- `0001213900-26-119734`
- `0001213900-26-119736`
- `0001213900-26-119783`
- `0001213900-26-119785`
- `0001213900-26-119809`
- `0001213900-26-119837`
- `0001213900-26-119839`
- `0001213900-26-119843`
- `0001213900-26-119857`
- `0001213900-26-119862`
- `0001213900-26-119864`
- `0001213900-26-119916`
- `0001224608-26-000084`
- `0001299709-26-000089`
- `0001339970-26-000088`
- `0001428205-26-000132`
- `0001437071-26-000089`
- `0001437749-26-036859`
- `0001437749-26-036861`
- `0001437749-26-036869`
- `0001437749-26-036885`
- `0001437749-26-036897`
- `0001437749-26-036911`
- `0001437749-26-036913`
- `0001437749-26-036914`
- `0001437749-26-036916`
- `0001437749-26-036917`
- `0001437749-26-036919`
- `0001437749-26-036920`
- `0001437749-26-036921`
- `0001437749-26-036924`
- `0001437749-26-036943`
- `0001437749-26-036953`
- `0001448431-26-000022`
- `0001477932-26-006933`
- `0001493152-26-051681`
- `0001493152-26-051691`
- `0001493152-26-051693`
- `0001493152-26-051707`
- `0001493152-26-051708`
- `0001493152-26-051711`
- `0001493152-26-051712`
- `0001493152-26-051725`
- `0001493152-26-051734`
- `0001493152-26-051735`
- `0001493152-26-051746`
- `0001493152-26-051747`
- `0001493152-26-051749`
- `0001493152-26-051750`
- `0001493152-26-051752`
- `0001493152-26-051760`
- `0001493152-26-051780`
- `0001493152-26-051806`
- `0001493152-26-051808`
- `0001493152-26-051809`
- `0001493152-26-051810`
- `0001493152-26-051811`
- `0001493152-26-051832`
- `0001493152-26-051834`
- `0001493152-26-051839`
- `0001493152-26-051841`
- `0001493152-26-051849`
- `0001493152-26-051858`
- `0001524472-26-000152`
- `0001539497-26-002960`
- `0001539497-26-002963`
- `0001571123-26-000151`
- `0001601485-26-000070`
- `0001628280-26-073758`
- `0001628280-26-073816`
- `0001628280-26-073824`
- `0001628280-26-073840`
- `0001628280-26-073844`
- `0001628280-26-073856`
- `0001628280-26-073860`
- `0001628280-26-073863`
- `0001628280-26-073867`
- `0001628280-26-073875`
- `0001628280-26-073897`
- `0001628280-26-073911`
- `0001640334-26-001797`
- `0001654954-26-009781`
- `0001682852-26-000205`
- `0001683168-26-008705`
- `0001720580-26-000069`
- `0001734342-26-000093`
- `0001753926-26-002133`
- `0001756761-26-000162`
- `0001760965-26-000088`
- `0001819438-26-000091`
- `0001829126-26-012399`
- `0001829126-26-012409`
- `0001829126-26-012414`
- `0001836875-26-000095`
- `0001878897-26-000055`
- `0001914496-26-000169`
- `0001976927-26-000092`
- `0002007919-26-000057`
- `0002054696-26-000030`
- `0002065708-26-000012`
- `0002089271-26-000035`
- `0002105965-26-000046`

Changed accessions: none — no accession appears in both pulls, so no column changed value.

### PULL 3 vs PULL 2

- Earlier (PULL 2): 197 rows; later (PULL 3): 200 rows.
- New: 200; gone: 197; changed: 0.
- Check: later = earlier + new − gone → 200 = 197 + 200 − 197 (True).

New accessions (in later pull only):

- `0000019617-26-000407`
- `0000037996-26-000193`
- `0000049071-26-000070`
- `0000057131-26-000042`
- `0000060667-26-000122`
- `0000064040-26-000063`
- `0000092122-26-000082`
- `0000103730-26-000086`
- `0000320187-26-000207`
- `0000775215-26-000103`
- `0000807882-26-000100`
- `0000817720-26-000111`
- `0000878927-26-000035`
- `0000885725-26-000073`
- `0000885978-26-000083`
- `0000909494-26-000016`
- `0000911147-26-000057`
- `0000943374-26-000492`
- `0000950103-26-017597`
- `0000950103-26-017684`
- `0000950142-26-003100`
- `0000950142-26-003101`
- `0000950157-26-001267`
- `0001020859-26-000033`
- `0001026655-26-000078`
- `0001045810-26-000088`
- `0001079973-26-001549`
- `0001096906-26-001809`
- `0001104659-26-128825`
- `0001104659-26-128843`
- `0001104659-26-128845`
- `0001104659-26-128849`
- `0001104659-26-128856`
- `0001104659-26-128862`
- `0001104659-26-128871`
- `0001104659-26-128886`
- `0001104659-26-129041`
- `0001104659-26-129043`
- `0001104659-26-129050`
- `0001104659-26-129055`
- `0001104659-26-129057`
- `0001104659-26-129066`
- `0001104659-26-129070`
- `0001104659-26-129089`
- `0001104659-26-129104`
- `0001104659-26-129125`
- `0001104659-26-129142`
- `0001104659-26-129162`
- `0001104659-26-129163`
- `0001104659-26-129165`
- `0001104659-26-129167`
- `0001140361-26-044343`
- `0001140361-26-044354`
- `0001140361-26-044356`
- `0001140361-26-044548`
- `0001171843-26-007505`
- `0001171843-26-007509`
- `0001171843-26-007511`
- `0001171843-26-007521`
- `0001175680-26-000042`
- `0001185185-26-005509`
- `0001193125-26-464750`
- `0001193125-26-464751`
- `0001193125-26-464780`
- `0001193125-26-464792`
- `0001193125-26-464836`
- `0001193125-26-464841`
- `0001193125-26-464853`
- `0001193125-26-464854`
- `0001193125-26-464874`
- `0001193125-26-465082`
- `0001193125-26-465087`
- `0001193125-26-465134`
- `0001193125-26-465150`
- `0001193125-26-465257`
- `0001193125-26-465488`
- `0001193125-26-465502`
- `0001193125-26-465504`
- `0001193125-26-465507`
- `0001193125-26-465510`
- `0001193125-26-465513`
- `0001193125-26-465518`
- `0001193125-26-465535`
- `0001193125-26-465542`
- `0001193125-26-465550`
- `0001193125-26-465600`
- `0001193125-26-465606`
- `0001193125-26-465607`
- `0001193125-26-465632`
- `0001193125-26-465633`
- `0001193125-26-465667`
- `0001193125-26-465668`
- `0001193125-26-465677`
- `0001193125-26-465741`
- `0001193125-26-465750`
- `0001210708-26-000113`
- `0001213900-26-121103`
- `0001213900-26-121109`
- `0001213900-26-121118`
- `0001213900-26-121132`
- `0001213900-26-121133`
- `0001213900-26-121397`
- `0001213900-26-121401`
- `0001213900-26-121407`
- `0001213900-26-121461`
- `0001213900-26-121478`
- `0001214659-26-014504`
- `0001214659-26-014510`
- `0001316944-26-000189`
- `0001325814-26-000181`
- `0001325878-26-000239`
- `0001326771-26-000184`
- `0001330399-26-000161`
- `0001331451-26-000219`
- `0001331463-26-000221`
- `0001331465-26-000210`
- `0001331754-26-000225`
- `0001331757-26-000207`
- `0001388658-26-000101`
- `0001437749-26-037305`
- `0001437749-26-037306`
- `0001437749-26-037320`
- `0001437749-26-037324`
- `0001437749-26-037331`
- `0001437749-26-037390`
- `0001437749-26-037393`
- `0001437749-26-037406`
- `0001437749-26-037415`
- `0001437749-26-037420`
- `0001437749-26-037422`
- `0001437749-26-037424`
- `0001462120-26-000087`
- `0001476765-26-000083`
- `0001476765-26-000084`
- `0001477932-26-007074`
- `0001477932-26-007091`
- `0001477932-26-007123`
- `0001493152-26-052703`
- `0001493152-26-052713`
- `0001493152-26-052714`
- `0001493152-26-052715`
- `0001493152-26-052720`
- `0001493152-26-052726`
- `0001493152-26-052739`
- `0001493152-26-052740`
- `0001493152-26-052751`
- `0001493152-26-052765`
- `0001493152-26-052781`
- `0001493152-26-052818`
- `0001493152-26-052822`
- `0001493152-26-052831`
- `0001493152-26-052832`
- `0001493152-26-052833`
- `0001493152-26-052840`
- `0001493152-26-052841`
- `0001493152-26-052862`
- `0001493152-26-052865`
- `0001493152-26-052871`
- `0001493152-26-052892`
- `0001493152-26-052894`
- `0001493152-26-052895`
- `0001493152-26-052897`
- `0001517375-26-000075`
- `0001539497-26-003027`
- `0001539497-26-003030`
- `0001570585-26-000158`
- `0001584207-26-000044`
- `0001606757-26-000084`
- `0001628280-26-074359`
- `0001628280-26-074363`
- `0001628280-26-074365`
- `0001628280-26-074373`
- `0001628280-26-074422`
- `0001628280-26-074426`
- `0001628280-26-074499`
- `0001628280-26-074500`
- `0001628280-26-074518`
- `0001628280-26-074572`
- `0001628280-26-074587`
- `0001654954-26-009901`
- `0001654954-26-009929`
- `0001655210-26-000084`
- `0001682220-26-000075`
- `0001683168-26-008892`
- `0001683168-26-008915`
- `0001728688-26-000051`
- `0001728951-26-000079`
- `0001747079-26-000112`
- `0001753926-26-002169`
- `0001772921-26-000057`
- `0001783398-26-000145`
- `0001834488-26-000060`
- `0001849056-26-000055`
- `0001874178-26-000073`
- `0001898795-26-000125`
- `0001901440-26-000037`
- `0002007919-26-000063`
- `0002035428-26-000074`
- `0002040491-26-000060`
- `0002104052-26-000147`

Gone accessions (in earlier pull only):

- `0000017843-26-000052`
- `0000025232-26-000082`
- `0000048465-26-000065`
- `0000067716-26-000089`
- `0000074208-26-000090`
- `0000076605-26-000113`
- `0000080420-26-000139`
- `0000106535-26-000015`
- `0000350852-26-000079`
- `0000715072-26-000092`
- `0000716634-26-000042`
- `0000776901-26-000174`
- `0000795266-26-000080`
- `0000911147-26-000055`
- `0000912593-26-000286`
- `0000926617-26-000058`
- `0000950142-26-003058`
- `0000950157-26-001261`
- `0001053507-26-000167`
- `0001062993-26-006086`
- `0001072613-26-000900`
- `0001079973-26-001517`
- `0001079973-26-001525`
- `0001087294-26-000086`
- `0001087294-26-000087`
- `0001096906-26-001785`
- `0001096906-26-001789`
- `0001099219-26-000064`
- `0001104659-26-128139`
- `0001104659-26-128140`
- `0001104659-26-128161`
- `0001104659-26-128251`
- `0001104659-26-128260`
- `0001104659-26-128272`
- `0001104659-26-128282`
- `0001104659-26-128300`
- `0001104659-26-128328`
- `0001104659-26-128336`
- `0001104659-26-128338`
- `0001104659-26-128350`
- `0001104659-26-128377`
- `0001104659-26-128406`
- `0001104659-26-128450`
- `0001104659-26-128453`
- `0001104659-26-128485`
- `0001104659-26-128533`
- `0001104659-26-128553`
- `0001104659-26-128565`
- `0001104659-26-128573`
- `0001104659-26-128592`
- `0001140361-26-044139`
- `0001140361-26-044210`
- `0001140361-26-044219`
- `0001185185-26-005466`
- `0001193125-26-463071`
- `0001193125-26-463356`
- `0001193125-26-463384`
- `0001193125-26-463400`
- `0001193125-26-463409`
- `0001193125-26-463442`
- `0001193125-26-463444`
- `0001193125-26-463447`
- `0001193125-26-463453`
- `0001193125-26-463456`
- `0001193125-26-463461`
- `0001193125-26-463483`
- `0001193125-26-463495`
- `0001193125-26-463506`
- `0001193125-26-463508`
- `0001193125-26-463553`
- `0001193125-26-463554`
- `0001193125-26-463558`
- `0001193125-26-463559`
- `0001193125-26-463573`
- `0001193125-26-463583`
- `0001193125-26-463591`
- `0001193125-26-463597`
- `0001193125-26-463626`
- `0001193125-26-463696`
- `0001193125-26-463704`
- `0001193125-26-463733`
- `0001193125-26-463741`
- `0001193125-26-463781`
- `0001193125-26-463865`
- `0001193125-26-463901`
- `0001213900-26-120471`
- `0001213900-26-120540`
- `0001213900-26-120603`
- `0001213900-26-120608`
- `0001213900-26-120624`
- `0001213900-26-120625`
- `0001213900-26-120720`
- `0001213900-26-120724`
- `0001213900-26-120734`
- `0001213900-26-120737`
- `0001213900-26-120793`
- `0001213900-26-120816`
- `0001213900-26-120828`
- `0001214659-26-014423`
- `0001214659-26-014450`
- `0001298675-26-000052`
- `0001298946-26-000052`
- `0001306830-26-000136`
- `0001437749-26-037155`
- `0001437749-26-037158`
- `0001437749-26-037162`
- `0001437749-26-037166`
- `0001437749-26-037172`
- `0001437749-26-037175`
- `0001437749-26-037176`
- `0001437749-26-037179`
- `0001437749-26-037194`
- `0001437749-26-037201`
- `0001437749-26-037204`
- `0001437749-26-037257`
- `0001437958-26-000086`
- `0001472375-26-000229`
- `0001493152-26-052288`
- `0001493152-26-052291`
- `0001493152-26-052323`
- `0001493152-26-052331`
- `0001493152-26-052332`
- `0001493152-26-052334`
- `0001493152-26-052349`
- `0001493152-26-052352`
- `0001493152-26-052377`
- `0001493152-26-052409`
- `0001493152-26-052414`
- `0001493152-26-052431`
- `0001493152-26-052451`
- `0001493152-26-052458`
- `0001493152-26-052460`
- `0001493152-26-052461`
- `0001493152-26-052466`
- `0001493152-26-052467`
- `0001493152-26-052468`
- `0001493152-26-052471`
- `0001493152-26-052478`
- `0001493152-26-052519`
- `0001493152-26-052548`
- `0001493152-26-052554`
- `0001493152-26-052559`
- `0001493152-26-052599`
- `0001500435-26-000075`
- `0001516912-26-000070`
- `0001539497-26-002999`
- `0001539497-26-003003`
- `0001600033-26-000052`
- `0001603978-26-000116`
- `0001628280-26-074089`
- `0001628280-26-074161`
- `0001628280-26-074168`
- `0001628280-26-074169`
- `0001628280-26-074184`
- `0001628280-26-074187`
- `0001628280-26-074189`
- `0001628280-26-074196`
- `0001628280-26-074199`
- `0001628280-26-074200`
- `0001628280-26-074209`
- `0001628280-26-074211`
- `0001628280-26-074213`
- `0001628280-26-074216`
- `0001628280-26-074241`
- `0001628280-26-074246`
- `0001628280-26-074264`
- `0001628280-26-074279`
- `0001628280-26-074280`
- `0001649749-26-000071`
- `0001654954-26-009844`
- `0001654954-26-009852`
- `0001654954-26-009854`
- `0001664710-26-000072`
- `0001682852-26-000208`
- `0001683168-26-008827`
- `0001683168-26-008851`
- `0001683168-26-008860`
- `0001683168-26-008861`
- `0001687229-26-000059`
- `0001718939-26-000071`
- `0001747079-26-000106`
- `0001753926-26-002153`
- `0001758766-26-000092`
- `0001758766-26-000094`
- `0001775734-26-000038`
- `0001784254-26-000054`
- `0001794783-26-000110`
- `0001801170-26-000306`
- `0001801661-26-000128`
- `0001805526-26-000177`
- `0001829126-26-012518`
- `0001835268-26-000045`
- `0001837607-26-000087`
- `0001941536-26-000038`
- `0001999371-26-025521`
- `0002015845-26-000065`
- `0002048951-26-000039`

Changed accessions: none — no accession appears in both pulls, so no column changed value.

The feed turned over completely between pulls (a new day of filings each time), which is why both diffs show new + gone counts equal to the full row counts and zero changed accessions.

## Verification (mechanical, this assembly)

- Assembly checks: 52/52 PASS (columns, row counts, key uniqueness, tallies recomputed from the final CSVs, SHA-256 recomputed, raw-feed agreement, review selection and item-code match, diff arithmetic).
- Per-pull verification at pull time: 20/20 checks PASS for PULL 1, PULL 2 and PULL 3 (re-run 2026-11-18, including a live spot-check that the first 5 review index pages per pull re-open with HTTP 200).
- Review verification (Revision 1): the 108 summaries are own-words paraphrases by design, so the verbatim-summary sub-check of review_8k.py --verify is superseded for summaries; re-run after the rewrite, its only flags are exactly those 108 paraphrases, and every structural check passes for all 40 filings (status complete, raw files present, every heading found at its recorded line, item codes match the feed). A dedicated Revision-1 QA re-verified each corrected PROOF quote verbatim against the saved filing text and scanned all 108 summaries for truncation markers, abbreviation fragments and signature/forward-looking boilerplate (0 found).
- Review verification (Revision 2): a dedicated Revision-2 QA re-verified every extended PROOF quote verbatim against the saved filing text and re-checked every one of the 108 summaries, fact by fact, against its extended excerpt; all 108 summaries are unchanged from Revision 1 (own-words paraphrases, as required by A3).
- Review verification (Revision 3): a dedicated Revision-3 QA re-verified every extended PROOF quote verbatim against the saved filing text and re-checked every one of the 108 summaries, fact by fact, against its excerpt with a strict scanner (0 flags after the fixes); every amount, date, name, count and causal claim in every summary is now stated verbatim, or as the same value in the filing's own notation, in the excerpt under its heading. The 8 summary trims are listed in Revision 3 corrections; the CSVs are unchanged (same SHA-256 as Revision 1).
- Live re-check 2026-11-18: all 40 reviewed index pages return HTTP 200 and contain their accession number.
- CSV SHA-256 (corrected deliverable CSVs): PULL 1 `5b306f6544f4ef60a52eedcc2bd31763a75c194a39b53115a8abf01f9142018d`, PULL 2 `75c4d582ced44520facea8b9d005dfda09adc878f6481e69f3887b9f01734f1a`, PULL 3 `b20ba9ae89d878e1351b7f76a4bb4656f50a975f78acb78d5696705d237a7150`. The CSVs as pulled keep the hashes recorded in the PULL notes above; only the company column of the attached copies was cleaned (see Revision 1 corrections).

## Revision 1 corrections

Made for Revision 1 (round 1 of 3) at the evaluator's request; everything not listed here is unchanged from the first submission.

- CSV company column (D2-D4): for every row whose form is not a plain 8-K (8-K/A or 8-K12B), the company value no longer carries the feed-title form: the "<form> - " prefix and the trailing " (CIK) (Filer)" were stripped, matching the plain 8-K rows. Rows cleaned: PULL 1: 11, PULL 2: 7, PULL 3: 5. Row counts unchanged (198 / 197 / 200); no other field or row changed. New SHA-256: PULL 1 `5b306f6544f4ef60a52eedcc2bd31763a75c194a39b53115a8abf01f9142018d`, PULL 2 `75c4d582ced44520facea8b9d005dfda09adc878f6481e69f3887b9f01734f1a`, PULL 3 `b20ba9ae89d878e1351b7f76a4bb4656f50a975f78acb78d5696705d237a7150`. The platform PULL notes carry the hashes of the CSVs as originally pulled; `CORRECTED PULL k:` notes with the corrected row counts and these new hashes accompany this resubmission.
- Review table: all 108 item summaries rewritten as one-line summaries in our own words of the sentence(s) under each heading; review row 15's company now reads "Versa Bancorp".
- PROOF (feed requests): the raw first and last `<entry>` elements of each of the six feed pages are now quoted exactly as the saved feed responses returned them, next to the updated-line quotes.
- PROOF (reviewed filings): each filing now lists its index-page and document requests with the full URL and the UTC time each was actually fetched (recorded by the review tool at fetch time).
- PROOF (filing excerpts): the excerpts for the items the evaluator named, and every other excerpt of the same classes, now give the heading as printed followed by the complete first sentence(s) under it - no abbreviation breaks, no 900-character truncation, no signature-block or forward-looking boilerplate.

## Revision 2 corrections

Made for Revision 2 (round 2 of 3) at the evaluator's request; everything not listed here is unchanged from the Revision 1 resubmission. The three CSVs are unchanged (same rows, same values, same SHA-256 as Revision 1); no summary was rewritten.

- CSV company column (D2-D4): the company values are already correct in all three CSVs, as the evaluator's own sampling confirmed (PULL 1 rows 43/177/181, PULL 2 rows 29/144/189, PULL 3 rows 38/61/62: items joined with semicolons, updated as printed, updated-utc correctly converted, size as printed, company a plain name, no empty cells). The proving sentences from the CORRECTED PULL notes, reproduced here character for character, are:

  - Company column corrected on 11 rows (8-K/A and 8-K12B): form prefix and trailing (CIK) (Filer) stripped, as already done for 8-K rows.
  - Company column corrected on 7 rows (8-K/A and 8-K12B): form prefix and trailing (CIK) (Filer) stripped, as already done for 8-K rows.
  - Company column corrected on 5 rows (8-K/A and 8-K12B): form prefix and trailing (CIK) (Filer) stripped, as already done for 8-K rows.

- PROOF (filing excerpts, A4): for every item whose summary states facts beyond the first sentence(s) under its heading, the excerpt now also quotes verbatim the further sentence(s) or exhibit-list lines those facts come from, so each summary can be read from the sentence(s) excerpted under its heading. This covers the items the evaluator named (Western Union 1.02/2.03, 3D Systems 1.01/3.02, Flux Power 1.01/3.01, Datavault 3.01, Douglas Elliman 5.02, Azio 5.07, Co-Diagnostics 5.02/5.07, Q/C 3.01, Accuray 3.03/5.03, Apollo 1.01/8.01, Panamera 4.02, IonQ 5.02, Versa Bancorp 1.01/3.03/5.02/5.03/9.01), every other narrative item of the same classes, and all 9.01 exhibit-list excerpts, which now quote the complete exhibit list. No summary was cut or rewritten; no excerpt was restructured.

## Revision 3 corrections

Made for Revision 3 (round 3 of 3, the last) at the evaluator's request; everything not listed here is unchanged from the Revision 2 resubmission. The three CSVs are unchanged (same rows, same values, same SHA-256 as Revision 1); no CSV was re-uploaded.

- PROOF (filing excerpts, A4): the excerpts of the six items the evaluator named now also quote verbatim the further sentence(s) their summaries state: Western Union 2.03 (proceeds to repay in full the $800,000,000 term loan under the 2024 Term Loan Agreement, maturing December 2027); 3D Systems 1.02 (the 2030 Notes Indenture satisfied and discharged, guarantees and liens released); Navient 5.02 (the retirement is not the result of any disagreement); IonQ 5.02 (Merrill previously Chief Financial Officer of Commvault) and 8.01 (Austin previously Chief Accounting Officer for Juniper Networks); BRC Group 5.02 (Weitzman no longer a Section 16 or executive officer). Three further excerpts of the same class were extended on re-checking all 108 summaries: National Health Investors 5.02 (indemnification to the maximum extent permitted by Maryland law), Flux Power 1.01 (all other loan terms remain unchanged), QUALCOMM 8.01 (the offering under the Form S-3 shelf registration statement). No summary was cut or rewritten except as listed below; no excerpt was restructured.
- Review table (A3): eight small trims, each removing a total or a count that no filing sentence states (the components are all quoted; the total or count itself is not): Booking Holdings 1.01 and 2.03 (the 3.55 billion euro total), QUALCOMM 1.01 (the 4.0 billion dollar total), Contango 1.01 (the eight co-agents), Cingulate 1.01 (the second sales agent), QUALCOMM 9.01 (the five series of notes), Booking Holdings 9.01 (the four senior notes and the four officers' certificates), CareTrust 9.01 (the four forward confirmations). Every other summary is unchanged from Revision 2.

## Data files (Synmerco Rule 25)

The three pull CSVs are attached to this escrow as Synmerco data files (uploaded and verified before submission):

```synmerco-data
5b306f6544f4ef60a52eedcc2bd31763a75c194a39b53115a8abf01f9142018d 8k-feed-pull1.csv
75c4d582ced44520facea8b9d005dfda09adc878f6481e69f3887b9f01734f1a 8k-feed-pull2.csv
b20ba9ae89d878e1351b7f76a4bb4656f50a975f78acb78d5696705d237a7150 8k-feed-pull3.csv
```
