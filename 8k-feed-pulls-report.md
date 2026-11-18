# 8-K current-feed pulls: three daily snapshots, item tallies, changes and 40 non-routine filings read

Three timed EDGAR current-feed pulls, 198 / 197 / 200 unique 8-K filings, 20/20 mechanical checks passed per pull (including live spot-checks against source documents), and 40 non-routine filings read in full (108 items).

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

Each PULL note is at least 24 hours after the previous one, and each carries the row count and the SHA-256 of its CSV. No pull failed and no pull was corrected, so no `CORRECTED PULL k:` note applies.

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

Selection rule: the first 40 unique accessions in PULL 1 feed order whose items include at least one item other than 7.01, 8.01, 9.01. All 40 are complete; parsed item codes match the feed for all 40. One line per item, taken from the first sentence under that item's heading in the filing document.

| # | Accession | Company | CIK | Form | Document path | Items (one-line summary each) |
|---|---|---|---|---|---|---|
| 1 | `0001213900-26-119916` | Tempest Therapeutics, Inc. | 0001544227 | 8-K | `/Archives/edgar/data/1544227/000121390026119916/ea0312157-8k_tempest.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, Tempest Therapeutics, Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026 and other business highlights.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 2 | `0001171843-26-007431` | BeyondSpring Inc. | 0001677940 | 8-K | `/Archives/edgar/data/1677940/000117184326007431/f8k_111326.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, BeyondSpring Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 3 | `0001193125-26-461047` | BCP Investment Corp | 0001372807 | 8-K | `/Archives/edgar/data/1372807/000119312526461047/d520705d8k.htm` | **2.02** Results of Operations and Financial Condition. — On November 11, 2026, BCP Investment Corporation (the “Company”) issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits: Exhibit Number Description 99.1 Press Release, dated November 11, 2026 99.2 Investor Presentation, dated November 12, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL Document) |
| 4 | `0001140361-26-043831` | CareTrust REIT, Inc. | 0001590717 | 8-K | `/Archives/edgar/data/1590717/000114036126043831/ny20085288x3_8k.htm` | **1.01** Entry into a Material Definitive Agreement — On November 11, 2026, CareTrust REIT, Inc. (the “Company”) entered into separate forward sale agreements (the “Initial Forward Sale Agreements”) with each of Bank of America, N.A. and Morgan Stanley & Co. LLC (the “Forward Purchasers”), relating to an aggregate of 17,000,000 shares of the Company’s common stock, par value $0.01 per share (“Common Stock”).<br>**8.01** Other Events — On November 11, 2026, the Company and the Partnership entered into the Underwriting Agreement with the Underwriters, the Forward Purchasers and the Forward Sellers, relating to the registered public offering and sale of 17,000,000 shares of Common Stock (the “Offering”).<br>**9.01** Financial Statements and Exhibits — (d) Exhibits. |
| 5 | `0001493152-26-051858` | MANGOCEUTICALS, INC. | 0001938046 | 8-K | `/Archives/edgar/data/1938046/000149315226051858/form8-k.htm` | **3.03** Material Modification to Rights of Security Holders. — As described in Item 5.03, which is incorporated by reference into this Item 3.03, Mangoceuticals, Inc. (the “Company”) amended its Series B and Series C preferred stock designations effective November 9, 2026, and established its Series D Preferred Stock effective November 9, 2026.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — On November 9, 2026, the Company filed with the Texas Secretary of State a certificate of amendment to each of the previously filed certificates of designations governing its Series B Convertible Preferred Stock (the “Series B Preferred Stock”) and its 6% Series C Convertible Cumulative Preferred Stock (the “Series C Preferred Stock”), as amended.<br>**5.07** Submission of Matters to a Vote of Security Holders. — On November 6, 2026, the holder of all 980,000 outstanding shares of Series C Preferred Stock, acting by written consent in lieu of a meeting, approved the Series C Amendment and the Series D Designation and the transactions contemplated thereby, including the proposed sale of up to 1,000,000 shares of Series D Preferred Stock at $10.00 per share pursuant to Regulation A.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 6 | `0001193125-26-461028` | Western Union CO | 0001365135 | 8-K | `/Archives/edgar/data/1365135/000119312526461028/d152329d8k.htm` | **1.02** Termination of a Material Definitive Agreement. — As previously reported by The Western Union Company (the “Company”), in the Current Report on Form 8-K filed with the Securities and Exchange Commission (the “SEC”) on June 28, 2024, the Company entered into a delayed draw term loan credit agreement, dated as of June 25, 2024, with the lenders party thereto and Bank of America, N.A., as administrative agent (the “2024 Term Loan Agreement”).<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — As previously reported by the Company, in the Current Report on Form 8-K filed with the SEC on January 9, 2026 (the “Closing Date 8-K”), the Company entered into a delayed draw term loan credit agreement, dated as of January 9, 2026 (as amended by the First Amendment thereto, dated as of June 17, 2026, the “Term Loan Agreement”), with the lenders party thereto and Bank of America, N.A., as administrative agent. |
| 7 | `0001193125-26-461027` | 3D SYSTEMS CORP | 0000910638 | 8-K | `/Archives/edgar/data/910638/000119312526461027/d533328d8k.htm` | **1.01** Entry into a Material Definitive Agreement. — As previously disclosed, on November 4, 2026, 3D Systems Corporation (the “Company”) entered into separate, privately negotiated agreements (the “Exchange Agreements”) with all of the holders (the “Transaction Participants”) of the Company’s currently outstanding 5.875% Convertible Senior Secured Notes due 2030 (the “2030 Notes”).<br>**1.02** Termination of a Material Definitive Agreement. — On November 12, 2026, following the exchange of all of the outstanding 2030 Notes pursuant to the Exchange Agreements, the Company delivered to Wilmington Savings Fund Society, FSB, as trustee and collateral agent (“WSFS”), an order for the cancellation of all of the outstanding 2030 Notes issued under the indenture, dated as of June 23, 2025 (as supplemented, the “2030 Notes Indenture”), among the Company, the guarantors party thereto and WSFS.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the 2031 Notes Indenture and the 2031 Notes is incorporated herein by reference.<br>**3.02** Unregistered Sales of Equity Securities. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the issuance of the Shares and the 2031 Notes is incorporated herein by reference.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. 4.1 Indenture, dated as of November 12, 2026, between 3D Systems Corporation and U.S. Bank Trust Company, National Association, as trustee 4.2 Form of 3.30% Convertible Senior Notes due 2031 (included in Exhibit 4.1) 104 Cover Page Interactive Data File (embedded as Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. 3D SYSTEMS CORPORATION Date: November 13, 2026 By: /s/ Phyllis Nordstrom Phyllis Nordstrom Chief Financial Officer and Chief Administrative Officer |
| 8 | `0001140361-26-043829` | Navient Holdings, Inc. | 0002152623 | 8-K | `/Archives/edgar/data/2152623/000114036126043829/ef20085597_8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 11, 2026, Frederick Arnold, a member of the Board of Directors (the “Board”) of Navient Holdings, Inc. (the “Company”), informed the Company that he was voluntarily retiring from the Board effective immediately. |
| 9 | `0001493152-26-051849` | Polomar Health Services, Inc. | 0001265521 | 8-K | `/Archives/edgar/data/1265521/000149315226051849/form8-k.htm` | **1.01** Entry Into a Material Definitive Agreement. — The information set forth under Item 2.03 of this Current Report on Form 8-K is incorporated by reference into this Item 1.01.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation. — Effective November 9, 2026, Polomar Health Services, Inc. (the “Company”) executed a Promissory Note and Loan Agreement (the “Note”) in favor of Island 40 Group, LLC (“I4G” or the “Lender”) in the principal amount of $450,000 reflecting the amount of commissions due and owing to I4G for services provided to the Company by I4G pursuant to the terms of a certain Sales Director and Distribution Agreement in effect between the Company and I4G.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 10 | `0001193125-26-461016` | IonQ, Inc. | 0001824920 | 8-K | `/Archives/edgar/data/1824920/000119312526461016/ionq-20261110.htm` | **3.02** Unregistered Sales of Equity Securities. — On November 13, 2026, IonQ, Inc. (the “Company”) filed with the Securities and Exchange Commission (the “SEC”) a prospectus supplement to the prospectus included in the Company’s Registration Statement on Form S-3ASR filed with the SEC on February 26, 2025 (File No. 333-285279) (the “Registration Statement”), covering the resale by certain selling stockholders of an aggregate of 34,580,646 shares of Company common stock, par value $0.0001 per share.<br>**5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Also on November 13, 2026, the Company announced that, on November 10, 2026, the Company appointed Gary Merrill as Chief Financial Officer, Treasurer, principal financial officer and principal accounting officer of the Company, to be effective upon his first day of employment, which is expected to be December 3, 2026 (the “Start Date”).<br>**8.01** Other Events. — Also on November 13, 2026, the Company announced that, effective on November 16, 2026, Thomas A.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 11 | `0001193125-26-461010` | Dolby Laboratories, Inc. | 0001308547 | 8-K | `/Archives/edgar/data/1308547/000119312526461010/d101237d8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 10, 2026, the Compensation Committee (the “Committee”) of the Board of Directors of Dolby Laboratories, Inc. (the “Company”) adopted an executive cash bonus plan for fiscal 2027, titled the 2027 Dolby Executive Bonus Plan (the “2027 Executive Plan”). |
| 12 | `0001640334-26-001797` | Panamera Holdings Corp | 0001620749 | 8-K | `/Archives/edgar/data/1620749/000164033426001797/pnht_8k.htm` | **4.02** Non-Reliance on Previously Issued Financial Statements or a Related Audit Report or Interim Review — Pursuant to the 8K filed on October 26,2026 regarding an unreported employment agreement and resulting unreported lawsuit that caused the reporting to be affected by Item 4.02 Non-Reliance on Previously Issue Financial Statements or a Related Audit Report or Interim Review. |
| 13 | `0001493152-26-051841` | Cingulate Inc. | 0001862150 | 8-K | `/Archives/edgar/data/1862150/000149315226051841/form8-k.htm` | **1.01** Entry into Material Definitive Agreement — As previously disclosed, on March 24, 2026, Cingulate Inc. (the “Company”) entered into an ATM Sales Agreement, or the ATM Agreement, with A.G.P./Alliance Global Partners (“A.G.P.”) as sales agent (the “Agent”), pursuant to which the Company may offer and sell, our common stock, par value $0.0001 per share, or common stock, having an aggregate offering price of up to $100,000,000, from time to time, through the Agent.<br>**2.02** Results of Operations and Financial Condition. — On November 13, 2026, Cingulate Inc. issued a press release announcing its financial results for the quarter ended September 30, 2026 and providing a regulatory update.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Amendment No. 1 to ATM Agreement, by and among the Company, A.G.P. and Maxim, dated November 13, 2026 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. |
| 14 | `0001493152-26-051839` | Flux Power Holdings, Inc. | 0001083743 | 8-K | `/Archives/edgar/data/1083743/000149315226051839/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — As previously disclosed, on September 17, 2026 (the “Effective Date”), Flux Power Holdings, Inc. (the “Registrant”) and Flux Power, Inc., a wholly-owned subsidiary of the Registrant (“Flux” and together with the Registrant, the “Company”), entered into Amendment No. 7 to the Loan and Security Agreement (as amended, the “Loan and Security Agreement”) with Gibraltar Business Capital, LLC (“GBC”), pursuant to which the Company is required to, among other things, complete a sale of equity interests resulting in net proceeds of not less than $4.0 million (the “Equity Raise Requirement”) within 50 days of the Effective Date (the “Initial Equity Raise Deadline”), or such later date as may be agreed to in writing by GBC in GBC’s sole discretion.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information required by Item 2.03 contained in Item 1.01 of this Current Report on Form 8-K is incorporated herein by reference.<br>**3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 9, 2026, the Company received a notice (the “Notice”) from The NASDAQ Stock Market LLC (“Nasdaq”) notifying the Company that based on its stockholders’ deficit of ($431,000) as reported in its Form 10-Q for the fiscal quarter ended September 30, 2026, the Company is no longer in compliance with Nasdaq Listing Rule 5550(b)(1), which requires the Company to maintain a minimum of $2,500,000 in stockholders’ equity for continued listing on The Nasdaq Capital Market (the “Stockholders’ Equity Requirement”).<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 15 | `0001104659-26-127233` | 8-K12B - Versa Bancorp (0002100848) (Filer) | 0002100848 | 8-K12B | `/Archives/edgar/data/2100848/000110465926127233/tm2629642d1_8k12b.htm` | **1.01** Entry into a Material Definitive Agreement. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 1.01 by reference.<br>**2.01** Completion of Acquisition or Disposition of Assets. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 2.01 by reference.<br>**3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 3.01 by reference.<br>**3.03** Material Modification to Rights of Security Holders. — The information set forth in the Introductory Note and Item 5.03 of this Current Report on Form 8-K is incorporated into this Item 3.03 by reference.<br>**5.01** Changes in Control of Registrant. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 5.01 by reference.<br>**5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, the Board received notice from Patrick DeLacey of his resignation from the Board.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — In anticipation of the completion of the Reorganization, on November 12, 2026, Versa Bancorp filed a certificate of amendment with the Secretary of State of the State of Delaware amending its certificate of incorporation, as amended (the “Amended Certificate of Incorporation”) to (i) increase the authorized number of Versa Bancorp Shares to 350,000,000 and (ii) provide for indemnification of Versa Bancorp’s officers and directors, and authorize indemnification of such employees and agents as Versa Bancorp determines to be appropriate, to the fullest extent permitted by Delaware law and other applicable law.<br>**7.01** Regulation FD Disclosure. — On November 13, 2026, Versa Bancorp issued a press release announcing the completion of the Reorganization.<br>**9.01** Financial Statements and Exhibits. — (a) Financial statements of businesses or funds acquired. |
| 16 | `0001104659-26-127230` | Datavault AI Inc. | 0001682149 | 8-K | `/Archives/edgar/data/1682149/000110465926127230/tm2629197d1_8k.htm` | **3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 10, 2026, Datavault AI Inc., a Delaware corporation (the “Company”), received a letter (the “Letter”) from the Listing Qualifications department of The Nasdaq Stock Market LLC (“Nasdaq”) notifying the Company that the Company’s common stock, par value $0.0001 per share (“Common Stock”), was subject to delisting from Nasdaq due to the Company’s non-compliance with the $1.00 bid price requirement set forth in Nasdaq Listing Rule 5550(a)(2) (the “Bid Price Rule”), unless the Company timely requests a hearing before the Nasdaq Hearings Panel (the “Panel”), which the Company intends to do.<br>**8.01** Other Events. — On November 13, 2026, the Company issued a press release (the “Press Release”) announcing receipt of the Letter and the Nasdaq trading suspension, as required under Nasdaq Listing Rule 5810(c)(3)(A)(iii).<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release, dated November 13, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 17 | `0001878897-26-000055` | Douglas Elliman Inc. | 0001878897 | 8-K | `/Archives/edgar/data/1878897/000187889726000055/doug-20261113.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers — On November 13, 2026, Douglas Elliman Inc. (the “Company”) and James B. |
| 18 | `0001104659-26-127228` | CHEETAH NET SUPPLY CHAIN SERVICE INC. | 0001951667 | 8-K | `/Archives/edgar/data/1951667/000110465926127228/tm2629774d1_8k.htm` | **2.02** Results of Operations and Financial Condition — On November 13, 2026, Cheetah Net Supply Chain Service Inc. issued a press release announcing its financial results for the third quarter of 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 19 | `0001493152-26-051834` | AIRWA INC. | 0001674440 | 8-K | `/Archives/edgar/data/1674440/000149315226051834/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — On November 9, 2026, AiRWA Inc. (the “Company”) entered into securities purchase agreements (the “Purchase Agreement”) with certain investors, pursuant to which the Company agreed to sell to the investors an aggregate of 1,800,000 shares of common stock of the Company, par value $0.001 per share (the “Common Stock”), at a purchase price of $0.8332 per share of Common Stock, which was the closing price of the Common Stock on the preceding trading day (the “Transaction”).<br>**3.02** Unregistered Sales of Equity Securities. — The information provided in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 3.02.<br>**9.01** Financial Statements and Exhibits. — The following exhibits are furnished with this Form 8-K: Exhibit No. Description 10.1 Form of Securities Purchase Agreement 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) Forward-Looking Statements This Current Report on Form 8-K contains forward-looking statements within the meaning of Section 27A of the Securities Act of 1933, as amended, and Section 21E of the Securities Exchange Act of 1934, as amended. |
| 20 | `0001437749-26-036953` | AZIO AI HOLDINGS, INC. | 0001563568 | 8-K | `/Archives/edgar/data/1563568/000143774926036953/adom20261113_8k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, at the 2026 Annual Meeting of Stockholders (the “Annual Meeting”) of Azio AI Holdings, Inc., a Delaware corporation (the “Company”), the Company’s stockholders approved the Azio AI Holdings, Inc. 2026 Equity Incentive Plan (the “2026 Plan”), which the Board of Directors of the Company (the “Board”) previously approved on July 2, 2026, subject to stockholder approval.<br>**5.07** Submission of Matters to a Vote of Security Holders. — On November 13, 2026, the Company reconvened and held the Annual Meeting, which was originally convened on November 2, 2026, and adjourned to November 13, 2026, due to a lack of quorum. |
| 21 | `0001493152-26-051832` | Where Food Comes From, Inc. | 0001360565 | 8-K | `/Archives/edgar/data/1360565/000149315226051832/form8-k.htm` | **2.02** Results of Operations and Financial Condition Reference — is made to the Where Food Comes From, Inc. (the “Company”) press release on November 12, 2026 and conference call transcript, attached hereto as Exhibits 99.1 and 99.2, respectively, and incorporated by reference herein (including, without limitation, the information set forth in the cautionary statement contained in the press release and conference call transcript), relating to the Company’s financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits (d) — Exhibits Exhibit No. Description 99.1 Press Release issued and dated November 12, 2026 99.2 Transcript for November 12, 2026 conference call 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the Registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. |
| 22 | `0001104659-26-127223` | Booking Holdings Inc. | 0001075531 | 8-K | `/Archives/edgar/data/1075531/000110465926127223/tm2629703d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — Senior Notes On November 13, 2026, Booking Holdings Inc. (the “Company”) executed four Officers’ Certificates (the “Officers’ Certificates”), in accordance with Sections 2.02 and 10.04 of the Indenture dated August 8, 2017 (the “Base Indenture” and, together with the Officers’ Certificates, the “Indenture”) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the “Trustee”) and registrar, in connection with the sale of €1,250,000,000 aggregate principal amount of the Company’s 3.950% Senior Notes due 2029 (the “2029 Notes”), €800,000,000 aggregate principal amount of the Company’s 4.375% Senior Notes due 2032 (the “2032 Notes”), €750,000,000 aggregate principal amount of the Company’s 4.750% Senior Notes due 2035 (the “2035 Notes”), and €750,000,000 aggregate principal amount of the Company’s [...]<br>**2.03** Creation of a Direct Financial Obligation or an Obligation — Under an Off-Balance Sheet Arrangement of the Registrant.<br>**8.01** Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the “Underwriting Agreement”) with Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto (the “Underwriters”), pursuant to which the Company agreed to issue and sell to the Underwriters €3,550,000,000 aggregate principal amount of Senior Notes in a registered public offering (the “Offering”).<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit Description 1.1* Underwriting Agreement, dated November 9, 2026, among Booking Holdings Inc., Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto. 4.1 Form of 3.950% Senior Note due 2029. 4.2 Form of 4.375% Senior Note due 2032. 4.3 Form of 4.750% Senior Note due 2035. 4.4 Form of 5.000% Senior Note due 2038. 4.5* Officers’ Certificate, dated November 13, 2026, with respect to the 3.950% Senior Note due 2029 issued pursuant to the Base Indenture. 4.6* Officers’ Certificate, dated November 13, 2026, with respect to the 4.375% Senior Note due 2032 issued pursuant to the Base Indenture. 4.7* Officers’ Certificate, dated November 13, 2026, with respect to the 4.750% Senior Note due 2035 issued pursuant to the Base Indenture. 4.8* [...] |
| 23 | `0001193125-26-460951` | BEASLEY BROADCAST GROUP INC | 0001099160 | 8-K | `/Archives/edgar/data/1099160/000119312526460951/bbgi-20261113.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, Beasley Broadcast Group, Inc. issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — Exhibit Number Description 99.1 Press Release dated November 13, 2026 issued by Beasley Broadcast Group, Inc. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). |
| 24 | `0001213900-26-119857` | Health In Tech, Inc. | 0002019505 | 8-K | `/Archives/edgar/data/2019505/000121390026119857/ea0311991-8k_health.htm` | **2.02** Results of Operations and Financial Condition. — On November 12, 2026, Health In Tech, Inc., a Nevada corporation (the “Company”) issued a press release announcing its results of operations for the quarter ended September 30, 2026, attached hereto as Exhibit 99.1.<br>**7.01** Regulation FD Disclosure. — As disclosed in Item 2.02 above, on November 12, 2026, the Company issued a press release announcing its results of operations for the quarter ended September 30, 2026, attached hereto as Exhibit 99.1.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits: Exhibit No. Description 99.1 Press release dated November 12, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) 1 |
| 25 | `0000877860-26-000230` | NATIONAL HEALTH INVESTORS INC | 0000877860 | 8-K | `/Archives/edgar/data/877860/000087786026000230/nhi-20261109.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, National Health Investors, Inc. (the “Company”) entered into an Indemnification Agreement (each, an “Indemnification Agreement”) with each of the Company’s directors and certain of the Company’s officers, including each of the Company’s executive officers.<br>**9.01** Financial Statements and Exhibits. — Exhibit Index Number Exhibit 10.1 Form of Indemnification Agreement 104 Cover Page Interactive Data File (formatted as inline XBRL and contained in Exhibit 101). .. |
| 26 | `0001628280-26-073911` | DocGo Inc. | 0001822359 | 8-K | `/Archives/edgar/data/1822359/000162828026073911/dcgo-20261113.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — As previously announced, DocGo Inc. (the “Company”) is conducting a search for a new Chief Executive Officer as the employment agreement of the Company’s current CEO, Lee Bienstock, expires December 31, 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Transition Services and Separation Agreement, dated November 13, 2026, by and between the Company and Lee Bienstock 104 Cover Page Interactive Data File (formatted as Inline XBRL). 1 SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. |
| 27 | `0001437749-26-036943` | ACCURAY INC | 0001138723 | 8-K | `/Archives/edgar/data/1138723/000143774926036943/aray20261111_8k.htm` | **3.02** Unregistered Sales of Equity Securities. — The information related to the issuance of the Series A Preferred Stock (as defined below) contained in Item 3.03 of this Current Report on Form 8-K is incorporated herein by reference.<br>**3.03** Material Modification to Rights of Security Holders. — As previously disclosed, the Company entered into that certain Securities Purchase Agreement, dated as of July 29, 2026 (as amended to date, the “Purchase Agreement”) with certain existing investors of the Company party thereto (the “Investors”), pursuant to which the Company agreed to sell, and the Investors agreed to purchase, an aggregate of 55,000 shares of the Company’s Series A Convertible Preferred Stock, par value $0.001 per share (the “Series A Preferred Stock”), for an aggregate purchase price of $55.0 million, or $1,000 per share, comprised of $15.0 million in cash and the conversion of $40.0 million of existing indebtedness held by the Investors.<br>**5.03** Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — As previously disclosed, on November 4, 2026, the Company announced that its board of directors had selected a 1-for-40 ratio for the previously approved reverse stock split of the Common Stock.<br>**7.01** Regulation FD Disclosure — Canceled Warrants In connection with the closing of the Purchase Agreement, certain outstanding warrants were automatically canceled and extinguished (the “Canceled Warrants”).<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 28 | `0001104659-26-127202` | Contango Silver & Gold Inc. | 0001502377 | 8-K | `/Archives/edgar/data/1502377/000110465926127202/tm2629486d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — On November 13, 2026, Contango Silver & Gold Inc. (the “Company”) entered into a Controlled Equity OfferingSM Sales Agreement (the “Sales Agreement”) with Cantor Fitzgerald & Co. (the “Lead Agent”) and ATB Capital Markets USA Inc., BTIG, LLC, Canaccord Genuity LLC, Haywood Securities Inc., National Bank Financial Inc., Freedom Capital Markets, Maxim Group LLC, and Research Capital USA Inc. (the “Co-Agents” and, collectively with the Lead Agent, the “Agents”) , pursuant to which the Company may offer and sell from time to time shares of the Company’s common stock, par value $0.01 per share (the “Shares”), having an aggregate offering price of up to $75,000,000 through the Agents.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 29 | `0001213900-26-119843` | SOUNDHOUND AI, INC. | 0001840856 | 8-K | `/Archives/edgar/data/1840856/000121390026119843/ea0312272-8k_sound.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Effective November 9, 2026, Tyler Moore assumed the role of principal accounting officer of SoundHound AI, Inc. (the “Company”).<br>**9.01** Financial Statement and Exhibits. Exhibit Number — Description 104 Cover Page Interactive Data File (formatted as inline XBRL) 1 SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this Current Report on Form 8-K to be signed on its behalf by the undersigned hereunto duly authorized. |
| 30 | `0001493152-26-051809` | NextBoat Inc. | 0002067767 | 8-K | `/Archives/edgar/data/2067767/000149315226051809/form8-k.htm` | **1.01** Entry into a Material Definitive Agreement. — Lease of Cape Fear Marina Boat Slips On November 4, 2026, Off The Hook Yacht Sales NC, LLC, (“OTH NC”), a North Carolina limited liability company and a wholly owned subsidiary of NextBoat Inc. (the “Company”), entered into a triple-net lease (the “Lease”) with Hadley Harbor Group LLC (the “Landlord”) for 22 boat slips at Cape Fear Marina in Wilmington, North Carolina.<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth in Item 1.01 of this Current Report on Form 8-K is incorporated by reference into this Item 2.03.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 31 | `0001493152-26-051811` | Co-Diagnostics, Inc. | 0001692415 | 8-K | `/Archives/edgar/data/1692415/000149315226051811/form8-k.htm` | **5.02** Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, Co-Diagnostics, Inc. (the “Company”) held a court-ordered special meeting of shareholders (the “Special Meeting”).<br>**5.07** Submission of Matters to a Vote of Security Holders — On November 13, 2026, the Company held a Special Meeting of shareholders at which the following matters were voted on: Proposal No. 1: Election of Directors.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 32 | `0001493152-26-051810` | Beyond Air, Inc. | 0001641631 | 8-K | `/Archives/edgar/data/1641631/000149315226051810/form8-k.htm` | **2.02** Results of Operations and Financial Condition. — On November 11, 2026, Beyond Air, Inc. (the “Company”) issued a press release announcing financial results for its fiscal quarter ended September 30, 2026, and certain recent corporate developments.<br>**7.01** Regulation FD Disclosure. — The information under Item 2.02 above is incorporated herein by reference.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 33 | `0001493152-26-051808` | Q/C TECHNOLOGIES, INC. | 0001321834 | 8-K | `/Archives/edgar/data/1321834/000149315226051808/form8-k.htm` | **3.01** Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 6, 2026, Q/C Technologies, Inc. (the “Company”) received a letter from the Listing Qualifications staff of The Nasdaq Stock Market (“Nasdaq”) notifying the Company that, based on the closing bid price of the Company’s common stock for the last 30 consecutive business days from September 25, 2026 to November 5, 2026, the Company no longer meets the continued listing requirement of Nasdaq under Nasdaq Listing Rule 5550(a)(2) to maintain a minimum bid price of $1.00 per share. |
| 34 | `0001213900-26-119839` | BRC Group Holdings, Inc. | 0001464790 | 8-K | `/Archives/edgar/data/1464790/000121390026119839/ea0312286-8k_brcgroup.htm` | **5.02** (b) Departure of Directors or Certain — Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. |
| 35 | `0001493152-26-051806` | Evofem Biosciences, Inc. | 0001618835 | 8-K | `/Archives/edgar/data/1618835/000149315226051806/form8-k.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, Evofem Biosciences, Inc. (the “Company”) issued a press release announcing its financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). |
| 36 | `0001193125-26-460888` | Seritage Growth Properties | 0001628063 | 8-K | `/Archives/edgar/data/1628063/000119312526460888/srg-20261113.htm` | **2.02** Results of Operations and Financial Condition. — On November 13 2026, the Company issued a press release regarding its financial results for the three and nine months ended September 30, 2026.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the Registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. |
| 37 | `0001193125-26-460887` | CERENOME, INC. | 0001095981 | 8-K | `/Archives/edgar/data/1095981/000119312526460887/cnsy-20261113.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, Cerenome, Inc. (the “Company”) reported financial results for the third quarter ended September 30, 2026 and other recent corporate updates.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits. |
| 38 | `0001193125-26-460879` | Apollo Global Management, Inc. | 0001858681 | 8-K | `/Archives/edgar/data/1858681/000119312526460879/d143669d8k.htm` | **1.01** Entry into a Material Definitive Agreement. — On November 13, 2026, Apollo Global Management, Inc. (the “Company”) issued $600,000,000 aggregate principal amount of its 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056 (the “Notes”), pursuant to a previously announced underwritten public offering (the “Offering”).<br>**2.03** Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 2.03.<br>**8.01** Other Events. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 8.01.<br>**9.01** Financial Statements and Exhibits. — The exhibits to this Current Report on Form 8-K (except Exhibit 104) are hereby incorporated by reference into the Registration Statement. (d) Exhibits. |
| 39 | `0001628280-26-073897` | American Strategic Investment Co. | 0001595527 | 8-K | `/Archives/edgar/data/1595527/000162828026073897/nycr-20261113.htm` | **2.02** Results of Operations and Financial Condition. — On November 13, 2026, American Strategic Investment Co. (the “Company”) issued a press release announcing its results of operations for the quarter ended September 30, 2026, and supplemental financial information for the quarter ended September 30, 2026, attached hereto as Exhibits 99.1 and 99.2, respectively.<br>**7.01** Regulation FD Disclosure. — As disclosed in Item 2.02 above, on November 13, 2026, the Company issued a press release announcing its results of operations for the quarter ended September 30, 2026, and supplemental financial information for the quarter ended September 30, 2026, attached hereto as Exhibits 99.1 and 99.2, respectively.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release dated November 13, 2026 99.2 Supplemental information for the quarter ended September 30, 2026 104 Cover Page Interactive Data File - the cover page XBRL tags are embedded within the Inline XBRL document |
| 40 | `0001104659-26-127163` | QUALCOMM INC/DE | 0000804328 | 8-K | `/Archives/edgar/data/804328/000110465926127163/tm2629667d1_8k.htm` | **1.01** Entry into a Material Definitive Agreement. — On November 12, 2026, QUALCOMM Incorporated (the Company) executed an Officers’ Certificate (the Officers’ Certificate), in accordance with Sections 2.02, 2.03, 10.04 and 10.05 of the Indenture dated May 20, 2015 (the Base Indenture and, together with the Officers’ Certificate, the Indenture) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the Trustee), in connection with the sale of $750,000,000 in aggregate principal amount of the Company’s 5.000% Notes due 2028 (the 2028 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.150% Notes due 2029 (the 2029 Notes), $1,000,000,000 in aggregate principal amount of the Company’s 5.350% Notes due 2031 (the 2031 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.600% Notes due 2033 (the 2033 Notes) and [...]<br>**8.01** Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the Underwriting Agreement) with BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P.<br>**9.01** Financial Statements and Exhibits. — (d) Exhibits Exhibit No Description 1.1 Underwriting Agreement, dated November 9, 2026, among QUALCOMM Incorporated, BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P. |

Truncation flags (3 of 108 item summaries): the first sentence under the heading ran past the 900-character capture cap, so the summary is cut there and marked ` [...]`. The affected items are:

- `0001104659-26-127223` Item 1.01
- `0001104659-26-127223` Item 9.01
- `0001104659-26-127163` Item 1.01

All other 105 summaries are complete first sentences.

## PROOF — feed requests

Every request: host `www.sec.gov`, endpoint `/cgi-bin/browse-edgar`, parameters `action=getcurrent`, `type=8-K`, `owner=include`, `count=100`, `output=atom`, `start=0` or `start=100`. User-Agent: `BOSS-NERO research/1.0 (contact: fadliar010817@gmail.com)`. Each page below quotes its raw `<updated>` line verbatim and its first and last entries; the attached CSVs contain every entry.

### PULL 1

Page `start=0` — requested 2026-11-16T10:32:56Z, responded 2026-11-16T10:33:08Z, HTTP 200, Date header `Mon, 16 Nov 2026 10:33:09 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-16T05:32:44-05:00</updated>`

First entry: `8-K - MACROGENICS INC (0001125345) (Filer)` — updated `2026-11-13T17:28:39-05:00` — <https://www.sec.gov/Archives/edgar/data/1125345/000112534526000077/0001125345-26-000077-index.htm>

Last entry: `8-K/A - NIQ Global Intelligence plc (0002054696) (Filer)` — updated `2026-11-13T16:29:35-05:00` — <https://www.sec.gov/Archives/edgar/data/2054696/000205469626000030/0002054696-26-000030-index.htm>

Page `start=100` — requested 2026-11-16T10:33:09Z, responded 2026-11-16T10:33:12Z, HTTP 200, Date header `Mon, 16 Nov 2026 10:33:13 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-16T05:33:03-05:00</updated>`

First entry: `8-K - PharmaCyte Biotech, Inc. (0001157075) (Filer)` — updated `2026-11-13T16:28:19-05:00` — <https://www.sec.gov/Archives/edgar/data/1157075/000168316826008705/0001683168-26-008705-index.htm>

Last entry: `8-K - AAON, INC. (0000824142) (Filer)` — updated `2026-11-13T15:16:30-05:00` — <https://www.sec.gov/Archives/edgar/data/824142/000162828026073758/0001628280-26-073758-index.htm>

### PULL 2

Page `start=0` — requested 2026-11-17T10:40:43Z, responded 2026-11-17T10:40:45Z, HTTP 200, Date header `Tue, 17 Nov 2026 10:40:45 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-17T05:40:45-05:00</updated>`

First entry: `8-K - Envela Corp (0000701719) (Filer)` — updated `2026-11-16T17:31:11-05:00` — <https://www.sec.gov/Archives/edgar/data/701719/000110465926128592/0001104659-26-128592-index.htm>

Last entry: `8-K - BLUE DOLPHIN ENERGY CO (0000793306) (Filer)` — updated `2026-11-16T16:18:18-05:00` — <https://www.sec.gov/Archives/edgar/data/793306/000143774926037179/0001437749-26-037179-index.htm>

Page `start=100` — requested 2026-11-17T10:40:45Z, responded 2026-11-17T10:40:49Z, HTTP 200, Date header `Tue, 17 Nov 2026 10:40:49 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-17T05:40:49-05:00</updated>`

First entry: `8-K - NEIGHBORHOOD INTELLIGENCE, INC. (0001130713) (Filer)` — updated `2026-11-16T16:18:08-05:00` — <https://www.sec.gov/Archives/edgar/data/1130713/000114036126044210/0001140361-26-044210-index.htm>

Last entry: `8-K - BBCMS Mortgage Trust 2026-5C43 (0002153909) (Filer)` — updated `2026-11-16T13:40:29-05:00` — <https://www.sec.gov/Archives/edgar/data/2153909/000153949726002999/0001539497-26-002999-index.htm>

### PULL 3

Page `start=0` — requested 2026-11-18T10:41:45Z, responded 2026-11-18T10:41:47Z, HTTP 200, Date header `Wed, 18 Nov 2026 10:41:48 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-18T05:41:48-05:00</updated>`

First entry: `8-K - GridAI Technologies Corp. (0001604191) (Filer)` — updated `2026-11-17T17:29:47-05:00` — <https://www.sec.gov/Archives/edgar/data/1604191/000110465926129167/0001104659-26-129167-index.htm>

Last entry: `8-K - NEPHROS INC (0001196298) (Filer)` — updated `2026-11-17T16:05:37-05:00` — <https://www.sec.gov/Archives/edgar/data/1196298/000149315226052831/0001493152-26-052831-index.htm>

Page `start=100` — requested 2026-11-18T10:41:48Z, responded 2026-11-18T10:41:50Z, HTTP 200, Date header `Wed, 18 Nov 2026 10:41:51 GMT`, 100 entries.

Raw feed line: `<updated>2026-11-18T05:41:51-05:00</updated>`

First entry: `8-K - IMPACT BIOMEDICAL INC. (0001834105) (Filer)` — updated `2026-11-17T16:05:36-05:00` — <https://www.sec.gov/Archives/edgar/data/1834105/000149315226052822/0001493152-26-052822-index.htm>

Last entry: `8-K - UL Solutions Inc. (0001901440) (Filer)` — updated `2026-11-17T07:03:35-05:00` — <https://www.sec.gov/Archives/edgar/data/1901440/000190144026000037/0001901440-26-000037-index.htm>

## PROOF — reviewed filings

Per filing: the Documents table from its EDGAR index page (verbatim rows), then each item heading with the first sentence under it. A quote is the heading as printed, an em dash, then the first sentence verbatim; the three summaries flagged above are cut at 900 characters and marked ` [...]`. Index and document URLs resolve live (all 40 index pages re-opened with HTTP 200 when re-checked 2026-11-18).

### 1. Tempest Therapeutics, Inc. — `0001213900-26-119916`

CIK 0001544227, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/0001213900-26-119916-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1544227/000121390026119916/ea0312157-8k_tempest.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312157-8k_tempest.htm iXBRL | 8-K | 34053 |
| 2 | PRESS RELEASE DATED NOVEMBER 13, 2026 | ea031215701ex99-1.htm | EX-99.1 | 66662 |
| 3 | GRAPHIC | ea031215701_ex99-1img1.jpg | GRAPHIC | 13928 |
|  | Complete submission text file | 0001213900-26-119916.txt |  | 339838 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Tempest Therapeutics, Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026 and other business highlights.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 2. BeyondSpring Inc. — `0001171843-26-007431`

CIK 0001677940, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/0001171843-26-007431-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1677940/000117184326007431/f8k_111326.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | f8k_111326.htm iXBRL | 8-K | 15737 |
| 2 | PRESS RELEASE | exh_991.htm | EX-99.1 | 92889 |
|  | Complete submission text file | 0001171843-26-007431.txt |  | 313879 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, BeyondSpring Inc. (the “Company”) issued a press release announcing its financial results for the quarter ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 3. BCP Investment Corp — `0001193125-26-461047`

CIK 0001372807, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/0001193125-26-461047-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1372807/000119312526461047/d520705d8k.htm>.

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

- Item 2.02 Results of Operations and Financial Condition. — On November 11, 2026, BCP Investment Corporation (the “Company”) issued a press release announcing its financial results for the fiscal quarter ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits: Exhibit Number Description 99.1 Press Release, dated November 11, 2026 99.2 Investor Presentation, dated November 12, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL Document)

### 4. CareTrust REIT, Inc. — `0001140361-26-043831`

CIK 0001590717, form 8-K, feed items 1.01, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/0001140361-26-043831-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1590717/000114036126043831/ny20085288x3_8k.htm>.

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

- Item 1.01 Entry into a Material Definitive Agreement — On November 11, 2026, CareTrust REIT, Inc. (the “Company”) entered into separate forward sale agreements (the “Initial Forward Sale Agreements”) with each of Bank of America, N.A. and Morgan Stanley & Co. LLC (the “Forward Purchasers”), relating to an aggregate of 17,000,000 shares of the Company’s common stock, par value $0.01 per share (“Common Stock”).
- Item 8.01 Other Events — On November 11, 2026, the Company and the Partnership entered into the Underwriting Agreement with the Underwriters, the Forward Purchasers and the Forward Sellers, relating to the registered public offering and sale of 17,000,000 shares of Common Stock (the “Offering”).
- Item 9.01 Financial Statements and Exhibits — (d) Exhibits.

### 5. MANGOCEUTICALS, INC. — `0001493152-26-051858`

CIK 0001938046, form 8-K, feed items 3.03, 5.03, 5.07, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/0001493152-26-051858-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1938046/000149315226051858/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 75576 |
|  | Complete submission text file | 0001493152-26-051858.txt |  | 251805 |

- Item 3.03 Material Modification to Rights of Security Holders. — As described in Item 5.03, which is incorporated by reference into this Item 3.03, Mangoceuticals, Inc. (the “Company”) amended its Series B and Series C preferred stock designations effective November 9, 2026, and established its Series D Preferred Stock effective November 9, 2026.
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — On November 9, 2026, the Company filed with the Texas Secretary of State a certificate of amendment to each of the previously filed certificates of designations governing its Series B Convertible Preferred Stock (the “Series B Preferred Stock”) and its 6% Series C Convertible Cumulative Preferred Stock (the “Series C Preferred Stock”), as amended.
- Item 5.07 Submission of Matters to a Vote of Security Holders. — On November 6, 2026, the holder of all 980,000 outstanding shares of Series C Preferred Stock, acting by written consent in lieu of a meeting, approved the Series C Amendment and the Series D Designation and the transactions contemplated thereby, including the proposed sale of up to 1,000,000 shares of Series D Preferred Stock at $10.00 per share pursuant to Regulation A.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 6. Western Union CO — `0001193125-26-461028`

CIK 0001365135, form 8-K, feed items 1.02, 2.03. Index: <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/0001193125-26-461028-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1365135/000119312526461028/d152329d8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d152329d8k.htm iXBRL | 8-K | 27002 |
|  | Complete submission text file | 0001193125-26-461028.txt |  | 138593 |

- Item 1.02 Termination of a Material Definitive Agreement. — As previously reported by The Western Union Company (the “Company”), in the Current Report on Form 8-K filed with the Securities and Exchange Commission (the “SEC”) on June 28, 2024, the Company entered into a delayed draw term loan credit agreement, dated as of June 25, 2024, with the lenders party thereto and Bank of America, N.A., as administrative agent (the “2024 Term Loan Agreement”).
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — As previously reported by the Company, in the Current Report on Form 8-K filed with the SEC on January 9, 2026 (the “Closing Date 8-K”), the Company entered into a delayed draw term loan credit agreement, dated as of January 9, 2026 (as amended by the First Amendment thereto, dated as of June 17, 2026, the “Term Loan Agreement”), with the lenders party thereto and Bank of America, N.A., as administrative agent.

### 7. 3D SYSTEMS CORP — `0001193125-26-461027`

CIK 0000910638, form 8-K, feed items 1.01, 1.02, 2.03, 3.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/0001193125-26-461027-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/910638/000119312526461027/d533328d8k.htm>.

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

- Item 1.01 Entry into a Material Definitive Agreement. — As previously disclosed, on November 4, 2026, 3D Systems Corporation (the “Company”) entered into separate, privately negotiated agreements (the “Exchange Agreements”) with all of the holders (the “Transaction Participants”) of the Company’s currently outstanding 5.875% Convertible Senior Secured Notes due 2030 (the “2030 Notes”).
- Item 1.02 Termination of a Material Definitive Agreement. — On November 12, 2026, following the exchange of all of the outstanding 2030 Notes pursuant to the Exchange Agreements, the Company delivered to Wilmington Savings Fund Society, FSB, as trustee and collateral agent (“WSFS”), an order for the cancellation of all of the outstanding 2030 Notes issued under the indenture, dated as of June 23, 2025 (as supplemented, the “2030 Notes Indenture”), among the Company, the guarantors party thereto and WSFS.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the 2031 Notes Indenture and the 2031 Notes is incorporated herein by reference.
- Item 3.02 Unregistered Sales of Equity Securities. — The information set forth under Item 1.01 of this Current Report on Form 8-K with respect to the issuance of the Shares and the 2031 Notes is incorporated herein by reference.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits. 4.1 Indenture, dated as of November 12, 2026, between 3D Systems Corporation and U.S. Bank Trust Company, National Association, as trustee 4.2 Form of 3.30% Convertible Senior Notes due 2031 (included in Exhibit 4.1) 104 Cover Page Interactive Data File (embedded as Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized. 3D SYSTEMS CORPORATION Date: November 13, 2026 By: /s/ Phyllis Nordstrom Phyllis Nordstrom Chief Financial Officer and Chief Administrative Officer

### 8. Navient Holdings, Inc. — `0001140361-26-043829`

CIK 0002152623, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/0001140361-26-043829-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2152623/000114036126043829/ef20085597_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | ef20085597_8k.htm iXBRL | 8-K | 28917 |
|  | Complete submission text file | 0001140361-26-043829.txt |  | 154717 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 11, 2026, Frederick Arnold, a member of the Board of Directors (the “Board”) of Navient Holdings, Inc. (the “Company”), informed the Company that he was voluntarily retiring from the Board effective immediately.

### 9. Polomar Health Services, Inc. — `0001493152-26-051849`

CIK 0001265521, form 8-K, feed items 1.01, 2.03, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/0001493152-26-051849-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1265521/000149315226051849/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 31282 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 46251 |
|  | Complete submission text file | 0001493152-26-051849.txt |  | 252832 |

- Item 1.01 Entry Into a Material Definitive Agreement. — The information set forth under Item 2.03 of this Current Report on Form 8-K is incorporated by reference into this Item 1.01.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation. — Effective November 9, 2026, Polomar Health Services, Inc. (the “Company”) executed a Promissory Note and Loan Agreement (the “Note”) in favor of Island 40 Group, LLC (“I4G” or the “Lender”) in the principal amount of $450,000 reflecting the amount of commissions due and owing to I4G for services provided to the Company by I4G pursuant to the terms of a certain Sales Director and Distribution Agreement in effect between the Company and I4G.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 10. IonQ, Inc. — `0001193125-26-461016`

CIK 0001824920, form 8-K, feed items 3.02, 5.02, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/0001193125-26-461016-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1824920/000119312526461016/ionq-20261110.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | ionq-20261110.htm iXBRL | 8-K | 57111 |
| 2 | EX-5.1 | ionq-ex5_1.htm | EX-5.1 | 24184 |
| 3 | EX-99.1 | ionq-ex99_1.htm | EX-99.1 | 26100 |
| 4 | GRAPHIC | img1365411_0.jpg | GRAPHIC | 15584 |
|  | Complete submission text file | 0001193125-26-461016.txt |  | 245055 |

- Item 3.02 Unregistered Sales of Equity Securities. — On November 13, 2026, IonQ, Inc. (the “Company”) filed with the Securities and Exchange Commission (the “SEC”) a prospectus supplement to the prospectus included in the Company’s Registration Statement on Form S-3ASR filed with the SEC on February 26, 2025 (File No. 333-285279) (the “Registration Statement”), covering the resale by certain selling stockholders of an aggregate of 34,580,646 shares of Company common stock, par value $0.0001 per share.
- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Also on November 13, 2026, the Company announced that, on November 10, 2026, the Company appointed Gary Merrill as Chief Financial Officer, Treasurer, principal financial officer and principal accounting officer of the Company, to be effective upon his first day of employment, which is expected to be December 3, 2026 (the “Start Date”).
- Item 8.01 Other Events. — Also on November 13, 2026, the Company announced that, effective on November 16, 2026, Thomas A.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 11. Dolby Laboratories, Inc. — `0001193125-26-461010`

CIK 0001308547, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/0001193125-26-461010-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1308547/000119312526461010/d101237d8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d101237d8k.htm iXBRL | 8-K | 30850 |
|  | Complete submission text file | 0001193125-26-461010.txt |  | 143851 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 10, 2026, the Compensation Committee (the “Committee”) of the Board of Directors of Dolby Laboratories, Inc. (the “Company”) adopted an executive cash bonus plan for fiscal 2027, titled the 2027 Dolby Executive Bonus Plan (the “2027 Executive Plan”).

### 12. Panamera Holdings Corp — `0001640334-26-001797`

CIK 0001620749, form 8-K, feed items 4.02. Index: <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/0001640334-26-001797-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1620749/000164033426001797/pnht_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | pnht_8k.htm iXBRL | 8-K | 20200 |
|  | Complete submission text file | 0001640334-26-001797.txt |  | 124344 |

- Item 4.02 Non-Reliance on Previously Issued Financial Statements or a Related Audit Report or Interim Review — Pursuant to the 8K filed on October 26,2026 regarding an unreported employment agreement and resulting unreported lawsuit that caused the reporting to be affected by Item 4.02 Non-Reliance on Previously Issue Financial Statements or a Related Audit Report or Interim Review.

### 13. Cingulate Inc. — `0001493152-26-051841`

CIK 0001862150, form 8-K, feed items 1.01, 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/0001493152-26-051841-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1862150/000149315226051841/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 44022 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 32083 |
| 3 | EX-99.1 | ex99-1.htm | EX-99.1 | 41506 |
|  | Complete submission text file | 0001493152-26-051841.txt |  | 341695 |

- Item 1.01 Entry into Material Definitive Agreement — As previously disclosed, on March 24, 2026, Cingulate Inc. (the “Company”) entered into an ATM Sales Agreement, or the ATM Agreement, with A.G.P./Alliance Global Partners (“A.G.P.”) as sales agent (the “Agent”), pursuant to which the Company may offer and sell, our common stock, par value $0.0001 per share, or common stock, having an aggregate offering price of up to $100,000,000, from time to time, through the Agent.
- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Cingulate Inc. issued a press release announcing its financial results for the quarter ended September 30, 2026 and providing a regulatory update.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Amendment No. 1 to ATM Agreement, by and among the Company, A.G.P. and Maxim, dated November 13, 2026 99.1 Press Release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized.

### 14. Flux Power Holdings, Inc. — `0001493152-26-051839`

CIK 0001083743, form 8-K, feed items 1.01, 2.03, 3.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/0001493152-26-051839-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1083743/000149315226051839/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 49859 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 16812 |
| 3 | GRAPHIC | ex10-1_001.jpg | GRAPHIC | 20951 |
| 4 | GRAPHIC | ex10-1_002.jpg | GRAPHIC | 22454 |
|  | Complete submission text file | 0001493152-26-051839.txt |  | 296501 |

- Item 1.01 Entry into a Material Definitive Agreement. — As previously disclosed, on September 17, 2026 (the “Effective Date”), Flux Power Holdings, Inc. (the “Registrant”) and Flux Power, Inc., a wholly-owned subsidiary of the Registrant (“Flux” and together with the Registrant, the “Company”), entered into Amendment No. 7 to the Loan and Security Agreement (as amended, the “Loan and Security Agreement”) with Gibraltar Business Capital, LLC (“GBC”), pursuant to which the Company is required to, among other things, complete a sale of equity interests resulting in net proceeds of not less than $4.0 million (the “Equity Raise Requirement”) within 50 days of the Effective Date (the “Initial Equity Raise Deadline”), or such later date as may be agreed to in writing by GBC in GBC’s sole discretion.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information required by Item 2.03 contained in Item 1.01 of this Current Report on Form 8-K is incorporated herein by reference.
- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 9, 2026, the Company received a notice (the “Notice”) from The NASDAQ Stock Market LLC (“Nasdaq”) notifying the Company that based on its stockholders’ deficit of ($431,000) as reported in its Form 10-Q for the fiscal quarter ended September 30, 2026, the Company is no longer in compliance with Nasdaq Listing Rule 5550(b)(1), which requires the Company to maintain a minimum of $2,500,000 in stockholders’ equity for continued listing on The Nasdaq Capital Market (the “Stockholders’ Equity Requirement”).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 15. 8-K12B - Versa Bancorp (0002100848) (Filer) — `0001104659-26-127233`

CIK 0002100848, form 8-K12B, feed items 1.01, 2.01, 3.01, 3.03, 5.01, 5.02, 5.03, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/0001104659-26-127233-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2100848/000110465926127233/tm2629642d1_8k12b.htm>.

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

- Item 1.01 Entry into a Material Definitive Agreement. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 1.01 by reference.
- Item 2.01 Completion of Acquisition or Disposition of Assets. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 2.01 by reference.
- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 3.01 by reference.
- Item 3.03 Material Modification to Rights of Security Holders. — The information set forth in the Introductory Note and Item 5.03 of this Current Report on Form 8-K is incorporated into this Item 3.03 by reference.
- Item 5.01 Changes in Control of Registrant. — The information set forth in the Introductory Note of this Current Report on Form 8-K is incorporated into this Item 5.01 by reference.
- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, the Board received notice from Patrick DeLacey of his resignation from the Board.
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — In anticipation of the completion of the Reorganization, on November 12, 2026, Versa Bancorp filed a certificate of amendment with the Secretary of State of the State of Delaware amending its certificate of incorporation, as amended (the “Amended Certificate of Incorporation”) to (i) increase the authorized number of Versa Bancorp Shares to 350,000,000 and (ii) provide for indemnification of Versa Bancorp’s officers and directors, and authorize indemnification of such employees and agents as Versa Bancorp determines to be appropriate, to the fullest extent permitted by Delaware law and other applicable law.
- Item 7.01 Regulation FD Disclosure. — On November 13, 2026, Versa Bancorp issued a press release announcing the completion of the Reorganization.
- Item 9.01 Financial Statements and Exhibits. — (a) Financial statements of businesses or funds acquired.

### 16. Datavault AI Inc. — `0001104659-26-127230`

CIK 0001682149, form 8-K, feed items 3.01, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/0001104659-26-127230-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1682149/000110465926127230/tm2629197d1_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629197d1_8k.htm iXBRL | 8-K | 30339 |
| 2 | EXHIBIT 99.1 | tm2629197d1_ex99-1.htm | EX-99.1 | 6891 |
|  | Complete submission text file | 0001104659-26-127230.txt |  | 207504 |

- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 10, 2026, Datavault AI Inc., a Delaware corporation (the “Company”), received a letter (the “Letter”) from the Listing Qualifications department of The Nasdaq Stock Market LLC (“Nasdaq”) notifying the Company that the Company’s common stock, par value $0.0001 per share (“Common Stock”), was subject to delisting from Nasdaq due to the Company’s non-compliance with the $1.00 bid price requirement set forth in Nasdaq Listing Rule 5550(a)(2) (the “Bid Price Rule”), unless the Company timely requests a hearing before the Nasdaq Hearings Panel (the “Panel”), which the Company intends to do.
- Item 8.01 Other Events. — On November 13, 2026, the Company issued a press release (the “Press Release”) announcing receipt of the Letter and the Nasdaq trading suspension, as required under Nasdaq Listing Rule 5810(c)(3)(A)(iii).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press Release, dated November 13, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

### 17. Douglas Elliman Inc. — `0001878897-26-000055`

CIK 0001878897, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/0001878897-26-000055-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1878897/000187889726000055/doug-20261113.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | doug-20261113.htm iXBRL | 8-K | 39227 |
|  | Complete submission text file | 0001878897-26-000055.txt |  | 154928 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers — On November 13, 2026, Douglas Elliman Inc. (the “Company”) and James B.

### 18. CHEETAH NET SUPPLY CHAIN SERVICE INC. — `0001104659-26-127228`

CIK 0001951667, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/0001104659-26-127228-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1951667/000110465926127228/tm2629774d1_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629774d1_8k.htm iXBRL | 8-K | 25433 |
| 2 | EXHIBIT 99.1 | tm2629774d1_ex99-1.htm | EX-99.1 | 128512 |
| 6 | GRAPHIC | tm2629774d1_ex99-1img001.jpg | GRAPHIC | 21370 |
| 7 | GRAPHIC | tm2629774d1_ex99-1img002.jpg | GRAPHIC | 32855 |
|  | Complete submission text file | 0001104659-26-127228.txt |  | 409082 |

- Item 2.02 Results of Operations and Financial Condition — On November 13, 2026, Cheetah Net Supply Chain Service Inc. issued a press release announcing its financial results for the third quarter of 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 19. AIRWA INC. — `0001493152-26-051834`

CIK 0001674440, form 8-K, feed items 1.01, 3.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/0001493152-26-051834-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1674440/000149315226051834/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 42427 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 230734 |
|  | Complete submission text file | 0001493152-26-051834.txt |  | 480566 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 9, 2026, AiRWA Inc. (the “Company”) entered into securities purchase agreements (the “Purchase Agreement”) with certain investors, pursuant to which the Company agreed to sell to the investors an aggregate of 1,800,000 shares of common stock of the Company, par value $0.001 per share (the “Common Stock”), at a purchase price of $0.8332 per share of Common Stock, which was the closing price of the Common Stock on the preceding trading day (the “Transaction”).
- Item 3.02 Unregistered Sales of Equity Securities. — The information provided in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 3.02.
- Item 9.01 Financial Statements and Exhibits. — The following exhibits are furnished with this Form 8-K: Exhibit No. Description 10.1 Form of Securities Purchase Agreement 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) Forward-Looking Statements This Current Report on Form 8-K contains forward-looking statements within the meaning of Section 27A of the Securities Act of 1933, as amended, and Section 21E of the Securities Exchange Act of 1934, as amended.

### 20. AZIO AI HOLDINGS, INC. — `0001437749-26-036953`

CIK 0001563568, form 8-K, feed items 5.02, 5.07. Index: <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/0001437749-26-036953-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1563568/000143774926036953/adom20261113_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | adom20261113_8k.htm iXBRL | 8-K | 65848 |
|  | Complete submission text file | 0001437749-26-036953.txt |  | 200777 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, at the 2026 Annual Meeting of Stockholders (the “Annual Meeting”) of Azio AI Holdings, Inc., a Delaware corporation (the “Company”), the Company’s stockholders approved the Azio AI Holdings, Inc. 2026 Equity Incentive Plan (the “2026 Plan”), which the Board of Directors of the Company (the “Board”) previously approved on July 2, 2026, subject to stockholder approval.
- Item 5.07 Submission of Matters to a Vote of Security Holders. — On November 13, 2026, the Company reconvened and held the Annual Meeting, which was originally convened on November 2, 2026, and adjourned to November 13, 2026, due to a lack of quorum.

### 21. Where Food Comes From, Inc. — `0001493152-26-051832`

CIK 0001360565, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/0001493152-26-051832-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1360565/000149315226051832/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 41856 |
| 2 | EX-99.1 | ex99-1.htm | EX-99.1 | 89647 |
| 3 | EX-99.2 | ex99-2.htm | EX-99.2 | 17649 |
|  | Complete submission text file | 0001493152-26-051832.txt |  | 329533 |

- Item 2.02 Results of Operations and Financial Condition Reference — is made to the Where Food Comes From, Inc. (the “Company”) press release on November 12, 2026 and conference call transcript, attached hereto as Exhibits 99.1 and 99.2, respectively, and incorporated by reference herein (including, without limitation, the information set forth in the cautionary statement contained in the press release and conference call transcript), relating to the Company’s financial results for the three and nine months ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits (d) — Exhibits Exhibit No. Description 99.1 Press Release issued and dated November 12, 2026 99.2 Transcript for November 12, 2026 conference call 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the Registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized.

### 22. Booking Holdings Inc. — `0001104659-26-127223`

CIK 0001075531, form 8-K, feed items 1.01, 2.03, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/0001104659-26-127223-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1075531/000110465926127223/tm2629703d1_8k.htm>.

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

- Item 1.01 Entry into a Material Definitive Agreement. — Senior Notes On November 13, 2026, Booking Holdings Inc. (the “Company”) executed four Officers’ Certificates (the “Officers’ Certificates”), in accordance with Sections 2.02 and 10.04 of the Indenture dated August 8, 2017 (the “Base Indenture” and, together with the Officers’ Certificates, the “Indenture”) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the “Trustee”) and registrar, in connection with the sale of €1,250,000,000 aggregate principal amount of the Company’s 3.950% Senior Notes due 2029 (the “2029 Notes”), €800,000,000 aggregate principal amount of the Company’s 4.375% Senior Notes due 2032 (the “2032 Notes”), €750,000,000 aggregate principal amount of the Company’s 4.750% Senior Notes due 2035 (the “2035 Notes”), and €750,000,000 aggregate principal amount of the Company’s [...]
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation — Under an Off-Balance Sheet Arrangement of the Registrant.
- Item 8.01 Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the “Underwriting Agreement”) with Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto (the “Underwriters”), pursuant to which the Company agreed to issue and sell to the Underwriters €3,550,000,000 aggregate principal amount of Senior Notes in a registered public offering (the “Offering”).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit Description 1.1* Underwriting Agreement, dated November 9, 2026, among Booking Holdings Inc., Banco Santander, S.A., BNP PARIBAS, Deutsche Bank AG, London Branch, Goldman Sachs & Co. LLC and HSBC Bank plc, as representatives of the several underwriters named in Schedule II thereto. 4.1 Form of 3.950% Senior Note due 2029. 4.2 Form of 4.375% Senior Note due 2032. 4.3 Form of 4.750% Senior Note due 2035. 4.4 Form of 5.000% Senior Note due 2038. 4.5* Officers’ Certificate, dated November 13, 2026, with respect to the 3.950% Senior Note due 2029 issued pursuant to the Base Indenture. 4.6* Officers’ Certificate, dated November 13, 2026, with respect to the 4.375% Senior Note due 2032 issued pursuant to the Base Indenture. 4.7* Officers’ Certificate, dated November 13, 2026, with respect to the 4.750% Senior Note due 2035 issued pursuant to the Base Indenture. 4.8* [...]

### 23. BEASLEY BROADCAST GROUP INC — `0001193125-26-460951`

CIK 0001099160, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/0001193125-26-460951-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1099160/000119312526460951/bbgi-20261113.htm>.

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

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | nhi-20261109.htm iXBRL | 8-K | 28266 |
| 2 | EX-10.1 | exhibit101to8-k502.htm | EX-10.1 | 84730 |
|  | Complete submission text file | 0000877860-26-000230.txt |  | 249449 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 9, 2026, National Health Investors, Inc. (the “Company”) entered into an Indemnification Agreement (each, an “Indemnification Agreement”) with each of the Company’s directors and certain of the Company’s officers, including each of the Company’s executive officers.
- Item 9.01 Financial Statements and Exhibits. — Exhibit Index Number Exhibit 10.1 Form of Indemnification Agreement 104 Cover Page Interactive Data File (formatted as inline XBRL and contained in Exhibit 101). ..

### 26. DocGo Inc. — `0001628280-26-073911`

CIK 0001822359, form 8-K, feed items 5.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/0001628280-26-073911-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1822359/000162828026073911/dcgo-20261113.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | dcgo-20261113.htm iXBRL | 8-K | 33541 |
| 2 | EX-10.1 | ceotransitionservicessepar.htm | EX-10.1 | 121390 |
|  | Complete submission text file | 0001628280-26-073911.txt |  | 299936 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — As previously announced, DocGo Inc. (the “Company”) is conducting a search for a new Chief Executive Officer as the employment agreement of the Company’s current CEO, Lee Bienstock, expires December 31, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 10.1 Transition Services and Separation Agreement, dated November 13, 2026, by and between the Company and Lee Bienstock 104 Cover Page Interactive Data File (formatted as Inline XBRL). 1 SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized.

### 27. ACCURAY INC — `0001437749-26-036943`

CIK 0001138723, form 8-K, feed items 3.02, 3.03, 5.03, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/0001437749-26-036943-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1138723/000143774926036943/aray20261111_8k.htm>.

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
- Item 3.03 Material Modification to Rights of Security Holders. — As previously disclosed, the Company entered into that certain Securities Purchase Agreement, dated as of July 29, 2026 (as amended to date, the “Purchase Agreement”) with certain existing investors of the Company party thereto (the “Investors”), pursuant to which the Company agreed to sell, and the Investors agreed to purchase, an aggregate of 55,000 shares of the Company’s Series A Convertible Preferred Stock, par value $0.001 per share (the “Series A Preferred Stock”), for an aggregate purchase price of $55.0 million, or $1,000 per share, comprised of $15.0 million in cash and the conversion of $40.0 million of existing indebtedness held by the Investors.
- Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year. — As previously disclosed, on November 4, 2026, the Company announced that its board of directors had selected a 1-for-40 ratio for the previously approved reverse stock split of the Common Stock.
- Item 7.01 Regulation FD Disclosure — Canceled Warrants In connection with the closing of the Purchase Agreement, certain outstanding warrants were automatically canceled and extinguished (the “Canceled Warrants”).
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 28. Contango Silver & Gold Inc. — `0001104659-26-127202`

CIK 0001502377, form 8-K, feed items 1.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/0001104659-26-127202-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1502377/000110465926127202/tm2629486d1_8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | FORM 8-K | tm2629486d1_8k.htm iXBRL | 8-K | 30927 |
| 2 | EXHIBIT 1.1 | tm2629486d1_ex1-1.htm | EX-1.1 | 337096 |
| 3 | EXHIBIT 5.1 | tm2629486d1_ex5-1.htm | EX-5.1 | 9222 |
| 7 | GRAPHIC | tm2629486d1_ex5-1img001.jpg | GRAPHIC | 2564 |
|  | Complete submission text file | 0001104659-26-127202.txt |  | 626541 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 13, 2026, Contango Silver & Gold Inc. (the “Company”) entered into a Controlled Equity OfferingSM Sales Agreement (the “Sales Agreement”) with Cantor Fitzgerald & Co. (the “Lead Agent”) and ATB Capital Markets USA Inc., BTIG, LLC, Canaccord Genuity LLC, Haywood Securities Inc., National Bank Financial Inc., Freedom Capital Markets, Maxim Group LLC, and Research Capital USA Inc. (the “Co-Agents” and, collectively with the Lead Agent, the “Agents”) , pursuant to which the Company may offer and sell from time to time shares of the Company’s common stock, par value $0.01 per share (the “Shares”), having an aggregate offering price of up to $75,000,000 through the Agents.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 29. SOUNDHOUND AI, INC. — `0001213900-26-119843`

CIK 0001840856, form 8-K, feed items 5.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/0001213900-26-119843-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1840856/000121390026119843/ea0312272-8k_sound.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312272-8k_sound.htm iXBRL | 8-K | 32861 |
|  | Complete submission text file | 0001213900-26-119843.txt |  | 243559 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — Effective November 9, 2026, Tyler Moore assumed the role of principal accounting officer of SoundHound AI, Inc. (the “Company”).
- Item 9.01 Financial Statement and Exhibits. Exhibit Number — Description 104 Cover Page Interactive Data File (formatted as inline XBRL) 1 SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the registrant has duly caused this Current Report on Form 8-K to be signed on its behalf by the undersigned hereunto duly authorized.

### 30. NextBoat Inc. — `0001493152-26-051809`

CIK 0002067767, form 8-K, feed items 1.01, 2.03, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/0001493152-26-051809-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/2067767/000149315226051809/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 42917 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 83884 |
|  | Complete submission text file | 0001493152-26-051809.txt |  | 313128 |

- Item 1.01 Entry into a Material Definitive Agreement. — Lease of Cape Fear Marina Boat Slips On November 4, 2026, Off The Hook Yacht Sales NC, LLC, (“OTH NC”), a North Carolina limited liability company and a wholly owned subsidiary of NextBoat Inc. (the “Company”), entered into a triple-net lease (the “Lease”) with Hadley Harbor Group LLC (the “Landlord”) for 22 boat slips at Cape Fear Marina in Wilmington, North Carolina.
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information set forth in Item 1.01 of this Current Report on Form 8-K is incorporated by reference into this Item 2.03.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 31. Co-Diagnostics, Inc. — `0001493152-26-051811`

CIK 0001692415, form 8-K, feed items 5.02, 5.07, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/0001493152-26-051811-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1692415/000149315226051811/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 75533 |
| 2 | EX-10.1 | ex10-1.htm | EX-10.1 | 16678 |
|  | Complete submission text file | 0001493152-26-051811.txt |  | 264278 |

- Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers. — On November 13, 2026, Co-Diagnostics, Inc. (the “Company”) held a court-ordered special meeting of shareholders (the “Special Meeting”).
- Item 5.07 Submission of Matters to a Vote of Security Holders — On November 13, 2026, the Company held a Special Meeting of shareholders at which the following matters were voted on: Proposal No. 1: Election of Directors.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 32. Beyond Air, Inc. — `0001493152-26-051810`

CIK 0001641631, form 8-K, feed items 2.02, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/0001493152-26-051810-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1641631/000149315226051810/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 39740 |
| 2 | EX-99.1 | ex99-1.htm | EX-99.1 | 101589 |
|  | Complete submission text file | 0001493152-26-051810.txt |  | 320242 |

- Item 2.02 Results of Operations and Financial Condition. — On November 11, 2026, Beyond Air, Inc. (the “Company”) issued a press release announcing financial results for its fiscal quarter ended September 30, 2026, and certain recent corporate developments.
- Item 7.01 Regulation FD Disclosure. — The information under Item 2.02 above is incorporated herein by reference.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 33. Q/C TECHNOLOGIES, INC. — `0001493152-26-051808`

CIK 0001321834, form 8-K, feed items 3.01. Index: <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/0001493152-26-051808-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1321834/000149315226051808/form8-k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | form8-k.htm iXBRL | 8-K | 36100 |
|  | Complete submission text file | 0001493152-26-051808.txt |  | 201574 |

- Item 3.01 Notice of Delisting or Failure to Satisfy a Continued Listing Rule or Standard; Transfer of Listing. — On November 6, 2026, Q/C Technologies, Inc. (the “Company”) received a letter from the Listing Qualifications staff of The Nasdaq Stock Market (“Nasdaq”) notifying the Company that, based on the closing bid price of the Company’s common stock for the last 30 consecutive business days from September 25, 2026 to November 5, 2026, the Company no longer meets the continued listing requirement of Nasdaq under Nasdaq Listing Rule 5550(a)(2) to maintain a minimum bid price of $1.00 per share.

### 34. BRC Group Holdings, Inc. — `0001213900-26-119839`

CIK 0001464790, form 8-K, feed items 5.02. Index: <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/0001213900-26-119839-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1464790/000121390026119839/ea0312286-8k_brcgroup.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | CURRENT REPORT | ea0312286-8k_brcgroup.htm iXBRL | 8-K | 36147 |
|  | Complete submission text file | 0001213900-26-119839.txt |  | 269607 |

- Item 5.02 (b) Departure of Directors or Certain — Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers.

### 35. Evofem Biosciences, Inc. — `0001493152-26-051806`

CIK 0001618835, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/0001493152-26-051806-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1618835/000149315226051806/form8-k.htm>.

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

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | srg-20261113.htm iXBRL | 8-K | 52534 |
| 2 | EX-99.1 | srg-ex99_1.htm | EX-99.1 | 454474 |
| 3 | GRAPHIC | img42621_0.jpg | GRAPHIC | 8154 |
|  | Complete submission text file | 0001193125-26-460888.txt |  | 676522 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13 2026, the Company issued a press release regarding its financial results for the three and nine months ended September 30, 2026.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No. Description 99.1 Press release dated November 13, 2026 104 Cover Page Interactive Data File (embedded within Inline XBRL document) SIGNATURE Pursuant to the requirements of the Securities Exchange Act of 1934, the Registrant has duly caused this report to be signed on its behalf by the undersigned hereunto duly authorized.

### 37. CERENOME, INC. — `0001193125-26-460887`

CIK 0001095981, form 8-K, feed items 2.02, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/0001193125-26-460887-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1095981/000119312526460887/cnsy-20261113.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | cnsy-20261113.htm iXBRL | 8-K | 52522 |
| 2 | EX-99.1 | cnsy-ex99_1.htm | EX-99.1 | 531409 |
|  | Complete submission text file | 0001193125-26-460887.txt |  | 722095 |

- Item 2.02 Results of Operations and Financial Condition. — On November 13, 2026, Cerenome, Inc. (the “Company”) reported financial results for the third quarter ended September 30, 2026 and other recent corporate updates.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits.

### 38. Apollo Global Management, Inc. — `0001193125-26-460879`

CIK 0001858681, form 8-K, feed items 1.01, 2.03, 8.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/0001193125-26-460879-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1858681/000119312526460879/d143669d8k.htm>.

Documents table:

| Seq | Description | Document | Type | Size |
|---|---|---|---|---:|
| 1 | 8-K | d143669d8k.htm iXBRL | 8-K | 33954 |
| 2 | EX-1.1 | d143669dex11.htm | EX-1.1 | 184116 |
| 3 | EX-4.1 | d143669dex41.htm | EX-4.1 | 537287 |
| 4 | EX-5.1 | d143669dex51.htm | EX-5.1 | 17167 |
| 9 | GRAPHIC | g143669dsp39.jpg | GRAPHIC | 6101 |
|  | Complete submission text file | 0001193125-26-460879.txt |  | 1094528 |

- Item 1.01 Entry into a Material Definitive Agreement. — On November 13, 2026, Apollo Global Management, Inc. (the “Company”) issued $600,000,000 aggregate principal amount of its 7.550% Fixed-Rate Resettable Junior Subordinated Notes due 2056 (the “Notes”), pursuant to a previously announced underwritten public offering (the “Offering”).
- Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 2.03.
- Item 8.01 Other Events. — The information contained in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 8.01.
- Item 9.01 Financial Statements and Exhibits. — The exhibits to this Current Report on Form 8-K (except Exhibit 104) are hereby incorporated by reference into the Registration Statement. (d) Exhibits.

### 39. American Strategic Investment Co. — `0001628280-26-073897`

CIK 0001595527, form 8-K, feed items 2.02, 7.01, 9.01. Index: <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/0001628280-26-073897-index.htm>. Document: <https://www.sec.gov/Archives/edgar/data/1595527/000162828026073897/nycr-20261113.htm>.

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

- Item 1.01 Entry into a Material Definitive Agreement. — On November 12, 2026, QUALCOMM Incorporated (the Company) executed an Officers’ Certificate (the Officers’ Certificate), in accordance with Sections 2.02, 2.03, 10.04 and 10.05 of the Indenture dated May 20, 2015 (the Base Indenture and, together with the Officers’ Certificate, the Indenture) between the Company and U.S. Bank Trust Company, National Association (as successor in interest to U.S. Bank National Association), as trustee (the Trustee), in connection with the sale of $750,000,000 in aggregate principal amount of the Company’s 5.000% Notes due 2028 (the 2028 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.150% Notes due 2029 (the 2029 Notes), $1,000,000,000 in aggregate principal amount of the Company’s 5.350% Notes due 2031 (the 2031 Notes), $750,000,000 in aggregate principal amount of the Company’s 5.600% Notes due 2033 (the 2033 Notes) and [...]
- Item 8.01 Other Events. — On November 9, 2026, the Company entered into an underwriting agreement (the Underwriting Agreement) with BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P.
- Item 9.01 Financial Statements and Exhibits. — (d) Exhibits Exhibit No Description 1.1 Underwriting Agreement, dated November 9, 2026, among QUALCOMM Incorporated, BNP Paribas Securities Corp., BofA Securities, Inc., Deutsche Bank Securities Inc., J.P.

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

- Assembly checks: 33/33 PASS (columns, row counts, key uniqueness, tallies recomputed from the final CSVs, SHA-256 recomputed, raw-feed agreement, review selection and item-code match, diff arithmetic).
- Per-pull verification: 20/20 checks PASS for PULL 1, PULL 2 and PULL 3 (re-run 2026-11-18, including a live spot-check that the first 5 review index pages per pull re-open with HTTP 200).
- Review verification: 40/40 filings PASS (re-run 2026-11-18): every summary found verbatim in the saved filing text, every heading found at its recorded line, every Documents-table row found in the saved index page, every raw file present.
- Live re-check 2026-11-18: all 40 reviewed index pages return HTTP 200 and contain their accession number.
- CSV SHA-256: PULL 1 `3a6ea568ee72b242e44dae52e70701d8b3cecc68b7666e20c71c6ea0b1e37d4a`, PULL 2 `b8d472f4d16305a887c648b5818fa06ff8d58b3d813b4785d8bc4806d705fbac`, PULL 3 `a4efa96674902edda72032412cd8f1052db8313a2a99813f1191b6e4f98ad19a`.

## Data files (Synmerco Rule 25)

The three pull CSVs are attached to this escrow as Synmerco data files (uploaded and verified before submission):

```synmerco-data
3a6ea568ee72b242e44dae52e70701d8b3cecc68b7666e20c71c6ea0b1e37d4a 8k-feed-pull1.csv
b8d472f4d16305a887c648b5818fa06ff8d58b3d813b4785d8bc4806d705fbac 8k-feed-pull2.csv
a4efa96674902edda72032412cd8f1052db8313a2a99813f1191b6e4f98ad19a 8k-feed-pull3.csv
```
