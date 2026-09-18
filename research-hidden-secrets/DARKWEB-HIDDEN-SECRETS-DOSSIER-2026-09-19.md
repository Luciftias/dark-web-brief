# THE HIDDEN SECRETS LAYER — Research Dossier
### For: "THE DARK WEB — An Evidence-Based Technical Investigation" (luciftias.github.io/dark-web-brief/ — formerly scartheseller72-max.github.io/dark-web-brief/)
### Date: 2026-09-19 · Status: build-ready research · Labels: `LOGGED FACT` / `LEGEND` / `CORRECTION`

How to read this file: Sections A–D are the research bank. Section E is the shipped-product catalog (30 payloads + 3 unlock chains + Chapter 13 spec). Sections F–G are guardrails and code architecture. Every factual claim carries a URL. Anything labeled LEGEND is presented as folklore and must be labeled as such in the UI. Anything labeled CORRECTION fixes an error common in secondary sources — use it to strengthen the site's myth-busting brand.

Site map (from `index.html` on disk — use these real IDs for trigger wiring): `hero`, `intro`, `architecture`, `history`, `layers`, `use`, `market`, `opsec`, `crypto`, `zeroday`, section 10 (Censorship Resistance 2026), section 11 (Beyond Tor), section 12 (Future Directions), Key Figures. UI hooks available: `#topnav`, `.progress-bar/#pgfill`, `.btt` back-to-top button.

---

# SECTION A — TRUE-STORY SECRET BANK

**Master table (36 entries).** Ch = chapter mapping on your site. "Payload seed" = the easter-egg unit of content (full mechanics in Section E).

| # | Story / Artifact | Why it's surprising | Primary source(s) | Ch | Payload seed |
|---|---|---|---|---|---|
| A01 | **Ulbricht doxxed himself on Stack Overflow.** In March 2013 he asked "How can I connect to a Tor hidden service using cURL in PHP?" posting first as "Ross Ulbricht," renamed to "frosty" one minute later. The question is still live, and the Silk Road server's code matched his pasted snippet nearly line-for-line. | The mastermind's fatal leak was asking for help with his own homework — publicly, under his real name, mid-operation. | criminal complaint archived: archive.org/details/UlbrichtCriminalComplaint_201310 · live question: stackoverflow.com/questions/15445285 · Slate: slate.com/technology/2013/10/silk-road-s-dread-pirate-ross-ulbricht-asked-stack-overflow-question-under-real-name.html · BBC: bbc.com/news/technology-24371894 | 7 | Console line "frosty was here" + SO question card (E11/E12) |
| A02 | **The "Altoid" self-promotion posts.** In Jan 2011 "Altoid" posted Silk Road links on a magic-mushroom forum and BitcoinTalk ("kind of like an anonymous Amazon.com"), then 8 months later asked for "an IT pro in the Bitcoin community" to contact **rossulbricht@gmail.com**. | The trail that ended Silk Road began with a botched astroturf campaign by its own founder. | CNN: cnn.com/2013/10/04/world/americas/silk-road-ross-ulbricht · DOJ indictment: justice.gov/archive/usao/nys/pressreleases/February14/RossUlbrichtIndictmentPR.php | 7 | "Altoid" breadcrumb in hero comment chain (E01) |
| A03 | **The Glen Park library grab.** Ulbricht was arrested Oct 1, 2013 in the San Francisco Public Library (Glen Park branch). DHS agent Jared Der-Yeghiayan, posing as a DPR lieutenant in a live chat, asked him to check a flagged message; when Ulbricht logged in, an agent grabbed the open laptop before it could be locked. | Tor was never broken — persuasion + timing + an open laptop did it. | KQED 2025 (Der-Yeghiayan testimony recap): kqed.org/news/12023762 · FBI artifact page: fbi.gov/history/artifacts/ross-william-ulbrichts-laptop | 7 | "Laptop grab" timed card on Ch 7 |
| A04 | **"Dread Pirate Roberts" is a Princess Bride reference** — the character who runs a criminal enterprise under a stolen identity and passes the name on. Ulbricht's alias choice was accidentally self-describing. | The most feared name in dark web history is a 1973 Goldman novel / 1987 film joke. | DOJ filings use the alias throughout: justice.gov/usao-sdny (Ulbricht indictment PDF) · cultural origin: en.wikipedia.org/wiki/The_Princess_Bride | 3 | Onion-skin layers motif (E04) |
| A05 | **The bitcoin math.** FBI seized **173,991 BTC** total in 2013 (29,655 + 144,336 on Ulbricht's hardware; $33.6M at the time). The 144,336 laptop coins sold in 2017 for **$48,238,116**. In 2020 the DOJ seized **69,370 BTC** (~$1B) from hacker "Individual X" — worth up to **$4.4B** by 2024 when forfeiture finalized. | Everyone remembers "millions"; the real number crossed a billion while sitting still. | DOJ SDNY 2013: justice.gov/usao-sdny/pr/manhattan-us-attorney-announces-seizure-additional-28-million-worth-bitcoins-belonging · DOJ 2017 ($48M sale): justice.gov/usao-sdny/pr/acting-manhattan-us-attorney-announces-forfeiture-48-million-sale-silk-road-bitcoins · DOJ 2020: justice.gov/usao-ndca/pr/united-states-files-civil-action-forfeit-cryptocurrency-valued-over-one-billion-us · WIRED 2024: wired.com/story/4-4-billion-silk-road-bitcoin-tigran-gambaryan | 8 | "Follow the coins" counter (E15) |
| A06 | **CORRECTION — the "$13.4M seizure".** No single documented seizure is exactly $13.4M. Closest artifacts: the FBI states Silk Road generated "**more than $13 million**" in Bitcoin commissions (artifact page), and Individual X's stolen coins were worth ~$14M in 2013. Use the audited figures (A05) and note the confusion. | Correcting a circulating number is peak "evidence-first" branding. | fbi.gov/history/artifacts/ross-william-ulbrichts-laptop · CNN 2020: edition.cnn.com/2020/11/06/business/bitcoin-seized-silk-road-ulbricht/index.html | 8 | Myth-bust popup on hover of a footnote |
| A07 | **Ulbricht was sentenced to life (2015) and pardoned Jan 21, 2025.** The arc from library arrest to full pardon is 11 years, 3 months. | Same case, two eras of US policy — perfect Ch 12 "future/present" artifact. | KQED: kqed.org/news/12023762 · background: en.wikipedia.org/wiki/Ross_Ulbricht | 3/12 | Timeline node "2025" |
| A08 | **Hansa was a police honeypot for ~4 weeks.** Dutch police (NHTCU) secretly ran Hansa from **June 20 to July 20, 2017** after arresting its two German admins; they logged **27,000 transactions**, data on ~420,000 users, ~10,000 buyer addresses handed to Europol, and planted a malicious Excel file that revealed **64 sellers' IPs**. Hansa's traffic rose 1,000→8,000 transactions/day when AlphaBay users fled to it — straight into the trap. | The "safe" market everyone migrated to was literally the police. | WIRED: wired.com/story/hansa-dutch-police-sting-operation · WIRED AlphaBay series pt 6: wired.com/story/alphabay-series-part-6-endgame · Europol: europol.europa.eu/media-press/newsroom/news/massive-blow-to-criminal-dark-web-activities-after-globally-coordinated-operation | 6/7 | "Trust no admin" reveal (E14) |
| A09 | **CORRECTION — Hansa "27,000 IPs".** Secondary sources say "27,000 IPs"; WIRED's primary reporting says Dutch police **surveilled 27,000 transactions**, not IPs. IPs were obtained for specific sellers via the Excel trap (64) and other means. | A single-word error that flatters LE capabilities — exactly what your site debunks. | wired.com/story/hansa-dutch-police-sting-operation | 6 | Myth-vs-reality chip |
| A10 | **AlphaBay's fatal email.** Cazes ('DeSnake' persona claims aside) minted AlphaBay's password-reset emails from **Pimp_Alex_91@hotmail.com** — also used on a PayPal account. He was arrested in Bangkok July 5, 2017; found dead in custody July 12 (towel, suicide ruled). DOJ said $23M in assets, Lamborghinis, "economic citizenship" applications. | The king of OpSec was undone by a password-reset header. | DOJ indictment PDF: justice.gov/archives/opa/press-release/file/982826/dl?inline · ABC: abc.net.au/news/2017-07-21/who-was-alphabay-founder-alexandre-cazes/8730680 · CBC: cbc.ca/news/canada/montreal/jeff-sessions-alexandre-cazes-dark-web-alphabay-1.4215009 · DW: dw.com/en/alleged-operator-of-alphabay-alexandre-cazes-found-dead-in-thai-prison/a-39708095 | 7 | Reset-email "from:" header easter egg |
| A11 | **Operation Bayonet was a sequencing trick.** FBI/DEA took AlphaBay down first (July 5) knowing users would flee to Hansa — which Dutch police already controlled (since June 20) — then took Hansa down (July 20), netting the refugees. | LE didn't just seize markets; they ran a funnel with live traffic. | Europol press: europol.europa.eu (link above) · WIRED pt 6 | 6/10 | "The Trap" two-date timeline unlock |
| A12 | **The CMU Tor attack (2014) → subpoena (2016).** Carnegie Mellon's Software Engineering Institute ran ~100+ relays and exploited hidden-service flaws (Biryukov et al.-style) to deanonymize hidden services; their Black Hat 2014 talk was cancelled; court filings in 2016 confirmed CMU was subpoenaed over the attack. Tor's Roger Dingledine publicly accused the FBI of paying CMU "at least $1 million" (FBI denied the amount, didn't deny using it). | A university lab, not a hacker, breached Tor — and courts forced it into the record. | WIRED: wired.com/2015/11/tor-says-feds-paid-carnegie-mellon-1m-to-help-unmask-users · Vice: vice.com/en/article/carnegie-mellon-university-attacked-tor-was-subpoenaed-by-feds · background paper: ieeexplore.ieee.org/document/6547103 | 7/9 | "Blue.42" defense hint inside console |
| A13 | **"Trawling for Tor Hidden Services" (IEEE S&P 2013).** Biryukov, Pustogarov, Thill, Weinmann demonstrated detection, measurement and deanonymization of hidden services, including practical evaluation on Silk Road and DuckDuckGo's onion. One of the most-cited Tor attack papers (>350 citations). | The academic paper that taught a generation how to unpeel onions. | PDF: ieee-security.org/TC/SP2013/papers/4977a080.pdf · ACM record: dl.acm.org/doi/10.1109/SP.2013.15 | 7 | "Lecture hall" hidden card in Ch 9 |
| A14 | **Relay fingerprinting research (2015–2016).** Kwon et al. (USENIX Security '15) showed **circuit fingerprinting attacks** that passively deanonymize hidden services; Nithyanand et al. (NDSS '16) measured AS-level adversaries against Tor. Tor's response was design hardening (padding, v3 onions). | Tor's cat-and-mouse is documented, peer-reviewed, and public — not conspiracy. | USENIX: usenix.org/conference/usenixsecurity15/technical-sessions/presentation/kwon · NDSS 2016: ndss-symposium.org (paper listing) | 7/10 | "Fingerprint pattern" background easter egg |
| A15 | **Freedom Hosting / Eric Eoin Marques.** FBI controlled Freedom Hosting servers from July 2013; on Aug 4, 2013 every hosted site served a "Down for Maintenance" page carrying a Firefox 17 ESR exploit (CVE-2013-1680) that beaconed visitor IPs to a Virginia server. Snowden leak revealed the exploit codename **"EgotisticalGiraffe."** Marques was arrested Aug 1, 2013 in Dublin; extradited 2019; pleaded guilty 2020; sentenced to **27 years** (Sept 15, 2021); service had 200+ CSAM sites, 8.5M images. | The first mass "malware-as-CDP" operation in dark web history — and it rode a browser bug, not a Tor break. | WIRED: wired.com/2013/09/freedom-hosting-fbi · Ars: arstechnica.com/tech-policy/2013/09/fbi-admits-what-we-all-suspected-it-compromised-freedom-hostings-tor-servers · DOJ: justice.gov/usao-md/pr/dark-web-child-pornography-facilitator-sentenced-27-years-federal-prison-conspiracy · CVE: nvd.nist.gov/vuln/detail/CVE-2013-1680 · Wikipedia (EgotisticalGiraffe, sourced): en.wikipedia.org/wiki/Freedom_Hosting | 7/9 | "Down for maintenance" fake page → real card |
| A16 | **Playpen / Operation Pacifier.** FBI seized Playpen Jan 2015 and **ran it for ~2 weeks** with a court-approved NIT that extracted users' IPs, OS username, MAC address. By May 2017: 350+ US arrests, 548 international, 55 US + 296 international children identified/rescued; creator Steven Chase got 30 years. The NIT warrant violated Rule 41(b) venue rules (courts split; Rule 41 later amended in 2016). | The FBI ran a CSAM site longer than its owner did — and it changed federal procedure. | FBI: fbi.gov/news/stories/playpen-creator-sentenced-to-30-years · EFF FAQ: eff.org/pages/playpen-cases-frequently-asked-questions · court record: govinfo.gov (USCOURTS-ned-4_15-cr-03134) · 2nd Cir: govinfo.gov (USCOURTS-ca2-17-03367) | 7/9 | "2 weeks" counter in a hidden card |
| A17 | **Even a Harvard student using Tor was identified in hours.** Eldo Kim, Dec 16, 2013: sent bomb threats via Guerrilla Mail + Tor — but connected **through Harvard's Wi-Fi**. University network logs gave him up; he confessed same night. Charged federally; diversion program incl. 750 hrs community service + restitution. | Tor hides the destination, not the fact you're using Tor from a monitored network. | DOJ: justice.gov/usao-ma/pr/harvard-student-charged-making-hoax-bomb-threat · Verge: theverge.com/2013/12/18/5224130/fbi-agents-tracked-harvard-bomb-threats-across-tor · CNN: cnn.com/2013/12/17/justice/massachusetts-harvard-hoax | 7 | "Wi-Fi doesn't lie" micro-card (E24) |
| A18 | **The catch phrase that defines institutional Tor.** Tor Project statement, Apple/FBI era (2016): *"The Tor Project has never received a legal demand to place a backdoor in its programs or source code... we've been public about our 'no backdoors, ever' stance."* Developers publicly said they'd resign rather than backdoor Tor. | A cypherpunk culture statement with receipts — quotable, sourceable, nonconspiratorial. | Tor blog: blog.torproject.org/statement-tor-project-software-integrity-and-apple · social contract coverage: eff.org / Tor project press page | 10/12 | Console pledge line (E24) |
| A19 | **Onion v3 addresses are literally public keys.** v3 = Base32(ed25519 pubkey (32B) ‖ SHA3-256(".onion checksum"‖pk‖0x03)[:2] ‖ 0x03) → 56 chars + `.onion`. This is why you can verify you're talking to the right service cryptographically, and why vanity addresses are grindable. | Most visitors have never been told the address *is* the crypto — a perfect hidden teaching moment. | Tor spec/gist: gist.github.com/andris9/ee2eb15cb3f729bae69a84258caef1ff · academic breakdown: par.nsf.gov/servlets/purl/10485912 | 2 | "Decode the chapter" gadget (E21) |
| A20 | **CIA's official onion site (May 2019).** `ciadotgov4sjwlzihbbgxnqg3xiyrg7so2r2o3lt5wz5ypk4sxyjstad.onion` — everything on CIA.gov available via Tor. CIA's own announcement tells users to verify the Tor Browser package. | The agency whose onion you'd fear is the one safest to visit — with a verify-first lesson attached. | CIA: cia.gov/stories/story/cias-latest-layer-an-onion-site | 5/10 | "Which onions are real?" quiz (E26) |
| A21 | **Facebook brute-forced a human-readable onion.** `facebookcorewwwi.onion` = "**facebook**'s **core** **w**orld **w**ide **w**eb **i**nfrastructure" — found by generating many v2 addresses and picking the best ("We got lucky" — Alec Muffett; compute-farm grinding of vanity prefixes). Migrated to v3 `facebookwkhpilnemxj7asaniu7vnjjbiltxjqhye3mhbshg7kx5tfyd.onion` in 2021. First major onion with a CA-issued TLS cert. | Big Tech once treated Tor as a first-class deployment target; the vanity address was a flex. | PCWorld: pcworld.com/article/436147 · Wikipedia: en.wikipedia.org/wiki/Facebook_onion_address · Muffett: alecmuffett.com/article/15996 | 5 | Vanity-address card in Ch 2/5 |
| A22 | **Institutional onion mirrors are real and boring.** NYT ran `nytimesn7cgmftshazwhfgzm37qxb44r64ytbb2dj3x62d2lljsciiyd.onion`, BBC runs `bbcnewsd73hkzno2ini43t4gblxvycyac5aw4gnv7t2rccijh7745uqd.onion`, ProPublica's SecureDrop lives at `33xu4yhum2eiisxm6fntaslayop76fvaqgt3ak5dakdm3t7cub25cead.onion` (plus the meta-service `propublica.securedrop.tor.onion`). **The NYT shut its Tor site down in 2025** ("effective immediately") — a great "the experiment ended" artifact. | The institutions treated as "the establishment" were early adopters; one quietly quit. | NYT Open (updated Mar 2025): open.nytimes.com/the-new-york-times-is-now-available-as-a-tor-onion-service-e0d0b67b7482 · SecureDrop directory: securedrop.org/directory/new-york-times · securedrop.org/directory/propublica | 5/12 | "Mirror wall" with verify instructions |
| A23 | **Tor was born at the US Naval Research Lab.** Onion routing: Goldschlag, Reed, Syverson, mid-1990s; DARPA refinement; Navy patent 1998. Roger Dingledine (MIT) + Paul Syverson started the modern project in the early 2000s; "Tor" = **The Onion Routing**; Nick Mathewson joined; **EFF funded the work starting 2004**; nonprofit 2006. The design paper is public. | The anonymity network everyone calls a criminal tool is a Navy-funded, EFF-funded open-source project published at USENIX. | Tor history: torproject.org/about/history · paper: usenix.org/legacy/event/sec04/tech/full_papers/dingledine/dingledine.pdf · background: en.wikipedia.org/wiki/Onion_routing | 1/3 | "1986/1995/2004" timeline click zones |
| A24 | **Rendezvous points were invented to solve the meet-in-the-middle problem.** Hidden services exist because a server must not reveal its location while clients must reach it; the second-gen design introduced "location-hidden services via rendezvous points." The onion metaphor is literal: each hop peels one layer. | The architecture story is beautiful, teachable, and court-proof (it's in the USENIX paper). | usenix paper (above) | 2 | Onion-peel animation trigger (E04) |
| A25 | **Operation Onymous (Nov 5–6, 2014) was smaller than announced.** Europol announced 414 sites; later revised to **267**; independent analysis (Nik Cubrilovic) found **153 of those were clones/phishing/scam sites**, and several claimed seizures were clones of still-live originals. 17 arrests; ~$1M BTC. | The flagship "we cracked Tor" operation was partly a press-release inflation — the site's brand's perfect myth-bust. | Swansea paper archive: swansea.ac.uk/media/Operation-Onymous.pdf · Nik Cubrilovic analysis as cited therein · Guardian: theguardian.com/technology/2014/nov/07/silk-road-20-operation-onymous-dark-web-drugs-takedown · BBC: bbc.com/news/technology-29950946 | 6/10 | "414 → 267 → 153" counter (E19) |
| A26 | **Silk Road 2.0 fell to social engineering + a personal email, not a Tor break.** DHS had an undercover agent inside SR2's admin staff; Blake Benthall ("Defcon") used a personal email when registering servers. | Even after Silk Road 1, operators repeated the same class of mistake within a year. | Guardian (above) · NYT: nytimes.com/2014/11/08/world/europe/dark-market-websites-operation-onymous.html | 7 | "Same mistake twice" card |
| A27 | **Operation DisrupTor (Sept 2020): 179 arrests from one server.** Wall Street Market's backend (seized May 2019) gave Europol the intelligence packages that produced 179 arrests in 6 countries, >$6.5M, ~500 kg drugs, 63–64 firearms. | The most effective LE campaign began with forensic bookkeeping, not hacking. | Europol: europol.europa.eu/media-press/newsroom/news/international-sting-against-dark-web-vendors-leads-to-179-arrests · DOJ: justice.gov/archives/opa/pr/international-law-enforcement-operation-targeting-opioid-traffickers-darknet-results-over-170 · WIRED: wired.com/story/operation-disruptor-179-arrested-global-dark-web-takedown | 6/10 | "One server → 179" stat card |
| A28 | **Operation SaboTor (March 2019): 61 arrests**, preceding DisrupTor; part of JCODE's run of operations. | Shows the cumulative "intelligence recycling" pattern. | DOJ (cited in DisrupTor release above) | 6 | footnote chip |
| A29 | **Welcome to Video (2019): the blockchain case.** Son Jong-woo's site monetized CSAM in bitcoin (first of its kind at scale); IRS-CI used Chainalysis to trace payments, found the server IP **unconcealed in the site's own source code**, and located the server in his bedroom in South Korea. 8 TB, 250,000+ videos; 337 users arrested across 12 countries; 23 children rescued. | The takedown was pure financial forensics + one sloppy server — no Tor break. | DOJ: justice.gov/archives/opa/pr/south-korean-national-and-hundreds-others-charged-worldwide-takedown-largest-darknet-child · WIRED: wired.com/story/dark-web-welcome-to-video-takedown-bitcoin · CNN: edition.cnn.com/2019/10/19/asia/south-korea-child-exploitation-international-police-intl-hnk/index.html | 8 | "Trace the ledger" ledger card (E15) |
| A30 | **Dread Pirate Roberts' "sock puppets."** Beyond frosty/Altoid, DPR used other personas to shape Silk Road's image; prosecutors used post timestamps + writing style + login logs. (The specific "frosty" chat is the cleanest documented case.) | Persona management failed on metadata, not on cryptography. | complaint (A01 sources) · Slate (A01) | 7 | "Sock puppet theatre" hidden chat mock |
| A31 | **2025–2026: markets shrink, Telegram becomes the "office."** Chainalysis: DNM flows ~**$2.6B in 2025** (up YoY but a fraction of Hydra-era), TorZon rising after Abacus closed (July 2025), fraud shops contracting; DNM admins+vendors hold **>$40B** on-chain. Telegram blocked **43.5M+ channels/groups in 2025** (peaks >500k/day) yet criminal ecosystems adapted rather than left (gated joins, backup channels). Europol's line: "the golden age of the dark web marketplace is over" (2020). | The story visitors think is "dark web" has already migrated to where they least expect: mainstream apps. | Chainalysis: chainalysis.com/blog/crypto-drug-sales-darknet-markets-2026 · chainalysis.com/blog/darknet-markets-2025 · Check Point/Cybernews: cybernews.com/security/telegram-channels-takedown-criminal-activity · Hacker News (The Hacker News): thehackernews.com/expert-insights/2026/03/telegrams-crackdown-changed-how-threat | 6/12 | Future-chapter reality check (E25) |
| A32 | **Tor WebTunnel (March 12, 2024): "hiding in plain sight."** A bridge transport that wraps Tor in WebSocket-like HTTPS and can coexist with a normal website on the same domain/IP/port — a reverse proxy silently splits real visitors from Tor bridge traffic. | Censorship circumvention by camouflage is now standard tooling, not folklore. | Tor blog: blog.torproject.org/introducing-webtunnel-evading-censorship-by-hiding-in-plain-sight · Debian manpage: manpages.debian.org/testing/webtunnel/webtunnel-server.1.en.html | 10 | "Same port, two worlds" reveal (E18-adjacent) |
| A33 | **Research agrees Tor users are not who the myths say.** USENIX SOUPS 2024 "The Onion Unpeeled" surveys user perceptions vs realities; CSCW 2023 "Tor over VPN" found **5–6% of Tor connections come from VPNs (~140k daily users)** and no clear security benefit to the folklore combo; various studies measure ~2–8M daily users depending on methodology. | Survey data = the antidote to "dark web = criminals" — and a Ch 5 payload. | SOUPS poster: usenix.org/system/files/soups2024_poster7-berger_final.pdf · CSCW: usenix.org/system/files/soups2024_poster3-fassl_final.pdf · Tor metrics: metrics.torproject.org | 5/12 | "Who actually uses Tor" poll card |
| A34 | **Nth Room (2019–20) is the real-world "red room" analog — and it wasn't on Tor.** Korean Telegram-based paid extortion/CSAM rings; ~74 victims identified, hundreds of thousands of paying users across tiers; operators sentenced (Cho Ju-bin life-equivalent 40y + others). Documented reality is chat apps, not "Level 7" websites. | Gives the site a factual center for the red-room discussion: the harm was real, the mechanism was Telegram. | Reuters/BBC coverage of Nth room verdicts (e.g., bbc.com/news/world-asia-53831063) · review: dexpose.io/dark-web-red-rooms | 6/12 | "Where the myth points" card |
| A35 | **The Dread Pirate Roberts trial quotables.** DOJ release notes DPR solicited violence ("I'd like him beat up, then forced to send the bitcoins...") — and that a murder-for-hire victim named "FriendlyChemist" never existed; no homicide was recorded where he supposedly lived. | Court records include both the worst and the fake — your Ch 6/7 can be precise about both. | superseding indictment PDF: ice.gov/doclib/news/releases/2013/131002baltimore.pdf · DOJ 2013 release: archives.fbi.gov/archives/newyork/press-releases/2013 | 6/7 | "No body, no crime — except the site" card |
| A36 | **Onymous"/"DisrupTor" naming is a tell.** "DisrupTor" mashes "disrupt" + "Tor"; "Onymous" = anonymous → named. Even operation names carry the myth-busting irony. | Tiny literary easter egg the design team will love. | Europol releases (A27) · Guardian (A25) | 6 | Wordplay chip in nav |

## Expanded notes on the 10 highest-value entries

### A01 — The Stack Overflow post (full quote)
The question (still live, 319k views, locked): *"How can I connect to a Tor hidden service using cURL in PHP?"* posted March 16, 2013 by user `frosty` (Q571 score — the community later realized who it was; badges "Stellar Question" and "Famous Question" arrived in Oct 2013, days after the arrest). The complaint extracted the logging trail: post at 3:39, username edited one minute later. Identical lines to the Silk Road server code. **UI use:** show the literal code block `curl_setopt($ch, CURLOPT_PROXY, "http://127.0.0.1:9050/");` and the SO URL — readers can click through to history. Copy note: the irony line "He changed his username to hide his association — one minute too late."

### A03/A04 — Library + persona
Der-Yeghiayan's undercover account chatted with DPR while Ulbricht sat in the library; the arrest team waited for the login. The laptop was grabbed while unlocked — the FBI artifact page displays it today. The DPR name references *The Princess Bride*'s framing device: a name passed between men, each claiming the legend. **UI use:** a "laptop" SVG in Ch 7; clicking it shows the artifact page link.

### A05 — Bitcoin ledger facts (use these numbers, not vibes)
- 29,655 BTC seized from Silk Road server side (Oct 2013).
- 144,336 BTC recovered from Ulbricht's laptop (announced Oct 25, 2013) → sold 2017 for $48,238,116.
- 173,991 BTC total 2013 → $33.6M at announcement prices.
- 69,370 BTC from Individual X (Nov 3, 2020, ~$1B) → forfeiture upheld; by Oct 2024 worth ~$4.4B (WIRED).
- Individual X was located partly via a 2015 liquidation attempt: 101 BTC into BTC-e (Guardian/DOJ complaint).
**Payload idea:** a "vault dial" where each number is a clickable token.

### A08/A09 — Hansa: the numbers you can defend
- Takeover: June 20, 2017 (Dutch custody) → public takedown July 20, 2017 (Europol).
- Surveilled: **27,000 transactions**; ~420,000 users' data; ≥10,000 addresses to Europol; 64 sellers IPs via Excel file; 12 Hansa dealers later found reusing credentials on Dream Market.
- Traffic: 1,000 → 8,000 orders/day after AlphaBay shutdown.
- Operation: Bayonet, led by FBI/DEA with Dutch police, Europol support.
**Correction badge:** "27,000 IPs" → "27,000 transactions."

### A12 — CMU timeline (for a clean in-page timeline)
- 2013: Biryukov et al. paper.
- Early 2014: CMU SEI runs relays; attack executed.
- Aug 2014: Black Hat talk pulled.
- Nov 2014: Silk Road 2.0 taken down (Operation Onymous); Tor community suspects the CMU technique.
- Feb 2016: court records confirm subpoena of CMU; Tor says it refused collaboration earlier.
- Nov 2015: Dingledine: FBI paid "at least $1M" (FBI denies the figure, not the use).

### A15 — Freedom Hosting payload copy
The injected page said "Down for Maintenance" to *every* service on the host — including innocent ones (TorMail, HackBB, Hidden Wiki). CVE-2013-1680 (use-after-free in Firefox ESR 17, fixed 17.0.6/21). Codename `EgotisticalGiraffe` from Snowden training slides (per Wikipedia's sourced summary). Marques' outcome: 27 years, $87,000 restitution (Guardian). **UI use:** a fake "Down for Maintenance" modal that flips to a sourced explainer after 3 seconds — one of the best payoffs on the whole site.

### A16 — Playpen numbers (as of May 4, 2017)
350+ US arrests · 25 producers prosecuted · 51 hands-on abusers · 55 US children identified/rescued · 548 international arrests · 296 international children identified/rescued · ~1,500 unique users/day, 150,000+ registered · site ran ~2 weeks under FBI control (Feb 20–Mar 4, 2015). EFF: "most extensive use of government malware by a US law enforcement agency in a domestic criminal investigation."

### A23 — Tor origin quotes
USENIX 2004 abstract: "a circuit-based low-latency anonymous communication service... practical design for location-hidden services via rendezvous points." Tor history page: NRL 1995 question ("a way to create internet connections that don't reveal who is talking to whom"), DARPA, patent 1998, Dingledine + Syverson early 2000s, name expansion "The Onion Routing," Mathewson joins, EFF funding 2004, nonprofit 2006, ~a dozen volunteer nodes by end of 2003.

### A29 — Welcome to Video chain (court-verified)
Server IP in source code → South Korea → Son's bedroom server → 8 TB / 250,000+ unique videos → bitcoin addresses >1M capacity → payments traced through exchanges → 337 users arrested in 12 countries (and 23 children rescued). Quote from DOJ: "Through the sophisticated tracing of bitcoin transactions, IRS-CI special agents were able to determine the location of the Darknet server..."

### A31 — 2025–2026 numbers for Ch 12
- DNM on-chain inflows ~$2.6B (2025) per Chainalysis 2026 report; ~$2B (2024) in prior edition.
- DNM admin+vendor on-chain holdings >$40B (Chainalysis, Oct 2025).
- Telegram: 43.5M+ channels/groups blocked in 2025; daily takedowns 10–30k baseline → sustained 80–140k, peaks 500k+ (Check Point via Cybernews).
- Europol "golden age" quote (2020) — keep dated.
- TorZon rising post-Abacus (July 2025); inter-market resupply documented.


---

# SECTION B — MYTH vs. REALITY BANK

Presentation rules for the UI: every debunk card shows CLAIM → VERDICT (Myth / Exaggerated / Partially true / Outdated) → WHAT'S DOCUMENTED → SOURCE → and a one-line "why the myth survives." Link sources inline.

| # | Claim | Verdict | What's actually documented | Source |
|---|---|---|---|---|
| B01 | "96% of the web is the dark web." | **Myth (category error)** | The 96% number belongs to the **deep web** (unindexed content: logins, databases, intranets) and traces to the 2001 BrightPlanet white paper (550B deep-web docs vs ~1B surface). The **dark web is a sub-fraction of the deep web**: ISO puts it <1%; Recorded Future crawled 260k onion pages and found ~8,416 live domains vs ~200M surface domains (<0.005%). | MPI copy of Deep Web white paper: resources.mpi-inf.mpg.de/d5/teaching/ws01_02/proseminarliteratur/deepwebwhitepaper.pdf · WIRED 2015: wired.com/2015/06/dark-web-know-myth · Recorded Future via TechRadar: techradar.com/news/the-dark-web-represents-only-a-fraction-of-the-rest-of-the-internet · ISO: committee.iso.org (dark web explainer) |
| B02 | "Mariana's Web is a deeper layer below the dark web." | **Myth** | Urban legend; origin traced to a 2011 Imgur "levels of the internet" infographic. No technical layer exists below Tor/I2P/Freenet; the "quantum computer only" requirement is fiction. Academic treatment: Robert W. Gehl's paper on the phenomenon; Skeptics.SE answer documents the Imgur origin. | Engadget: engadget.com/2015-12-18-the-myth-of-marianas-web-the-darkest-corner-of-the-internet.html · Skeptics SE: skeptics.stackexchange.com/questions/42621 · Gehl paper cited therein |
| B03 | "The deep web has Levels 1–7+." | **Myth (fanfic)** | Infographic culture. The real "levels" that exist are engagement designs in puzzle games (Notpron's 140 levels), not network layers. | Notpron: en.wikipedia.org/wiki/Notpron · B02 sources |
| B04 | "Red rooms — pay-per-view live torture on Tor — exist." | **Myth (as described)** | No verified case in the entire documented history of Tor investigations. Tor is too slow for the livestreaming UX described; "red room" sites found in the wild are engagement-bait/scams. Closest real analogue: Nth Room (paid tiers, chat-app based, not live-streamed on Tor; ~74 victims; operators prosecuted). Also documented: "1 Lunatic 1 Ice Pick" was Luka Magnotta's uploaded murder video (arrested, convicted) — not a red room. | Vice: vice.com/en/article/the-real-dark-web-doesnt-exist · Metro: metro.co.uk/2017/02/27/what-is-a-red-room-dooh-darkweb-live-stream-murder-sites-really-exist-6476047 · dexpose review: dexpose.io/dark-web-red-rooms · BBC on Nth room verdicts |
| B05 | "Shadow Web / Shout rooms / Monkey rooms." | **Myth (internet folklore)** | Same family as B02/B04; no documented instances. These names function as creepypasta canons. | as B04 · SMH investigation: smh.com.au/technology/the-dark-web-uncovering-monsters-and-myths-in-the-net-s-evil-twin-20180307-p4z39d.html |
| B06 | "Tor makes you untraceable." | **Myth** | Documented deanonymizations and identifications: Eldo Kim (network logs), Playpen users (NIT malware), Freedom Hosting visitors (Firefox exploit), CMU/SEI attack on hidden services, plus endless OpSec errors (Ulbricht, Cazes). Tor protects traffic analysis, not users who leak identity through email, browsers, payments, or their own hands. | Verge (Kim): theverge.com/2013/12/18/5224130 · EFF Playpen FAQ: eff.org/pages/playpen-cases-frequently-asked-questions · WIRED CMU: wired.com/2015/11/tor-says-feds-paid-carnegie-mellon-1m-to-help-unmask-users |
| B07 | "The dark web is mostly drugs." | **Partially true / misleading** | Within *darknet markets*, drugs dominate wholesale flows (Chainalysis: 71–81% of 2024 DNM inflow share is wholesale drug purchasing). But "the dark web" as a whole includes dead mirrors, forums, fraud shops, CSAM (documented — handle carefully), journalism mirrors, and hobby sites. Markets are the loud minority of a small network. | Chainalysis 2025: chainalysis.com/blog/darknet-markets-2025 · WIRED 2015 (B01) |
| B08 | "Bitcoin is anonymous." | **Myth** | BTC is pseudonymous, permanently public, and clumped by analytics. Welcome to Video was unwound by chain analysis; the 2020 Individual X seizure was enabled by a 2015 partial liquidation; Chainalysis/TRM sell tracing to LE globally. Better statement: "bitcoin is a permanent public ledger with a PR team." | DOJ Welcome to Video: justice.gov (A29) · DOJ 2020 seizure: justice.gov/usao-ndca (A05) · MIT Tech Review: technologyreview.com/2019/10/16/132575 |
| B09 | "Delete your data and it's gone." | **Myth (in practice)** | Backups, logs, archives, mirrors, forensic images, and opposing parties retain copies. The Silk Road evidence lived on seized laptops; forums get mirrored; Wayback never forgets. Data minimization beats deletion. | FBI artifact (A03) · general: archive.org · your own site's Chapter 7 examples |
| B10 | "VPN + Tor = invincible." | **Exaggerated (folklore)** | CSCW 2023 study: 5–6% of connections to Tor come via VPN servers (~140k daily users), driven by social norm ("the cool kids do it"), with no clear security benefit; VPN can't patch browser exploits or self-doxxing, and can add a paid trail. | Fassl et al., USENIX SOUPS 2024 poster summarizing CSCW 2023: usenix.org/system/files/soups2024_poster3-fassl_final.pdf |
| B11 | "Silk Road was taken down by hackers." | **Myth (event conflation)** | SR1 fell to conventional investigation: forum posts, Gmail, VPN logs, an undercover admin, and an open laptop. The CMU/SEI relay attack came *after* SR1, in service of later targets (SR2/Onymous era). | BBC/CNN/Slate (A01–A03) · WIRED CMU (A12) |
| B12 | "All .onion sites are illegal." | **Myth** | CIA, BBC, NYT, ProPublica/SecureDrop, Facebook/Meta, Tor Project itself, and many libraries/universities operate onion services. Legit uses: whistleblowing, censorship circumvention, journalism, privacy. | CIA: cia.gov/stories/story/cias-latest-layer-an-onion-site · SecureDrop directory: securedrop.org/directory · Wikipedia: en.wikipedia.org/wiki/Facebook_onion_address |
| B13 | "The dark web is massive/hidden majority of the internet (iceberg)." | **Myth** | See B01. Live onion services are a rounding error next to the surface web (~8.4k live observed vs ~200M domains; 86% English-language per Recorded Future). | TechRadar (B01) |
| B14 | "Tor was made by the CIA/NSA as a honeypot." | **Partially true → distorted** | Origin = US Naval Research Lab (intelligence-adjacent by definition) + DARPA + Navy patent; but the code is open source, audited, and includes no backdoors by design; Tor Project's documented stance: "no backdoors, ever" (2016 statement). The nuance is honest and interesting — use it. | torproject.org/about/history · Tor blog: blog.torproject.org/statement-tor-project-software-integrity-and-apple · usenix design paper |
| B15 | "Tor is illegal to use." | **Myth in most jurisdictions** | Running/using Tor is legal in most countries; EFF's Tor legal FAQ addresses relay operators; Tor Project publishes guidance for law enforcement too. Some states restrict circumvention tools — the accurate statement is "legality varies by country/context." | EFF legal FAQ: community.torproject.org/relay/community-resources/eff-tor-legal-faq |
| B16 | "You can order a hitman on the dark web." | **Partially true only as scams/stings** | Documented cases are overwhelmingly scams or LE stings; DOJ's Silk Road materials note the supposed "FriendlyChemist" murder target didn't exist (no homicide recorded). The genre's real artifact is fraud. | DOJ/FBI releases (A35) |
| B17 | "Closing the laptop / smashing the drive defeats forensics." | **Exaggerated** | Live-memory states, backups, server-side mirrors, and cloud logs are the real exposure; Ulbricht's own case shows the server held what the laptop hid. In Cazes' arrest, his laptop was found logged into the server. | KQED (A03) · ABC (A10) |
| B18 | "Dark web takedowns ended the problem (post-Onymous, post-Hansa)." | **Outdated** | Markets regrew after every takedown (Onymous → SR3 clones; AlphaBay → Hansa; Wall Street → DisrupTor; Hydra → Kraken/TorZon). Chainalysis: 2025 flows rose YoY; ecosystem migrates to Telegram-first layers. | Swansea (A25) · WIRED DisrupTor (A27) · Chainalysis 2026: chainalysis.com/blog/crypto-drug-sales-darknet-markets-2026 |

**Copy pattern for debunk cards** (serious tone, no sneering):
> `MYTH` — "96% of the internet is the dark web."
> `WHAT PEOPLE MEAN` — the deep web (logins, databases) is enormous.
> `WHAT'S DOCUMENTED` — the dark web is a small sliver of the deep web; live onion services number in the thousands.
> `SOURCE` — BrightPlanet 2001 white paper; Recorded Future 2019 crawl; ISO briefing.

---

# SECTION C — HIDDEN-IN-PLAIN-SIGHT WEB TECHNIQUES

Implementation language: vanilla HTML/CSS/JS, single file, no dependencies. Each entry: difficulty (1 easy → 5 hard), sketch, real-world example links.

### C1. Console messages — difficulty 1
The classic. Developers' greeting, ASCII art, recruitment notes, and styled log lines using `%c` formatting. Real examples: Reddit's console job prompt; Slack prints its logo; Linear, Airbnb, Mozilla's fire-breathing dragon; Discord's `/humans.txt`. Best-practice copy is a legitimate warning + a hook (Facebook's famous "This is a browser feature intended for developers" self-XSS warning is a real defensive message worth emulating in spirit).
Sketch:
```js
console.log("%cTHE DARK WEB BRIEF", "font:700 22px Georgia;color:#e8e6e3;background:#030305;padding:6px 14px;border:1px solid #333");
console.log("You read the source. Good. Type `sauron.help()` for what the record actually shows.");
```
Sources: r/webdev thread collecting 12 real examples: reddit.com/r/webdev/comments/15ufv4d · Discord wiki: en.wikibooks.org/wiki/A_Guide_to_Discord/Easter_Eggs

### C2. Keyboard-sequence secrets — difficulty 1–2
- **Konami code**: ↑↑↓↓←→←→BA — invented by Kazuhisa Hashimoto for NES Gradius (1986), left in by accident, popularized by Contra (1988, +30 lives). Canonical web implementations: Discord 404 Snake; Bank of Canada site (plays anthem, drops $10 notes); Netflix reset variations.
- **Typed words**: buffer keystrokes; match "ONION", "TOR", "SILKROAD", "FROSTY", "3301". Case-insensitive; reset buffer on timeout (1.2s) and on non-letter keys.
- **Arrow sequences**: reuse the Konami listener shape; e.g., ←←→→↑↑↓↓ (reverse).
Sketch:
```js
const seq = [38,38,40,40,37,39,37,39,66,65]; let i=0;
addEventListener("keydown", e=>{ i = (e.keyCode===seq[i]) ? i+1 : 0;
  if(i===seq.length){ i=0; Sauron.unlock("konami"); }});
```
Sources: en.wikipedia.org/wiki/Konami_Code · atlasobscura.com/articles/cheating-wonders-a-brief-history-of-the-konami-code · Drupal module history: drupal.org/docs/contributed-modules/konami-code

### C3. Hidden routes & files — difficulty 2
- **`/robots.txt`**: standard for crawler rules; Disallow paths *reveal* hidden locations to humans (classic discovery vector). MDN warns it is not access control: "it does not secure websites... by adding sensitive page paths you show their locations." Perfect for a deliberate, safe breadcrumb.
- **`/.well-known/security.txt`**: RFC 9116 (April 2022) — machine-parsable vulnerability-disclosure contact file; fields: Contact, Expires, Canonical, Policy, Preferred-Languages, Acknowledgments. Educational payload: your site can host a *valid* security.txt, with one ROT13 line for humans.
- **`/humans.txt`**: informal credits file (web standards/team credits); Discord ships one with ASCII logo: `discord.com/humans.txt`.
- **Sitemap breadcrumbs / hash anchors / query params**: `#vault`, `?door=2`, `?found=3`. GitHub Pages serves static files; 404.html works for custom error pages.
Sources: RFC 9116: rfc-editor.org/rfc/rfc9116 · MDN robots.txt guide: developer.mozilla.org/en-US/docs/Web/Security/Practical_implementation_guides/Robots_txt · Discord humans.txt (via Wikibooks page above)

### C4. Source-level secrets — difficulty 2
- **HTML comments with ciphers.** Classic; keep signed/labeled ("This is an educational easter egg — decode: ROT13"). Notpron uses source comments as core mechanics ("what am I?").
- **`<noscript>` messages** for JS-off visitors; make it a real alternative, not a trap (a11y win).
- **Invisible Unicode**: zero-width space U+200B, ZWNJ U+200C, ZWJ U+200D, word-joiner U+2060, BOM U+FEFF; bidi controls (U+202A–U+202E) can visibly scramble text — use only in sandboxed toy contexts, never for real content. Encode bits as ZWSP/ZWJ pairs; detect on copy and decode with a JS utility.
- **White-on-white / color:transparent + `::selection` reveal**: text invisible until selected (or highlight-reveal on hover with `background-color` transition). Provide a non-visual alternative: `title` attr or a "reveal" button so screen readers aren't denied content.
- **Acrostics** in headings (first letters of chapter subtitles spell a word) — zero tech, maximum delight.
Sketch (ZW decode):
```js
const zwd = s => [...s].filter(c=>c==="\u200b"||c==="\u200d")
  .map(c=>c==="\u200b"?"0":"1").join("").replace(/.{8}/g,b=>String.fromCharCode(parseInt(b,2)));
```
Example study: zero-width stego is documented in academic watermarking literature and commonly used in "hidden message" web toys; test with a font that renders them invisibly (most do).

### C5. DevTools-reactive behavior — difficulty 3, ethics-gated
Detect that DevTools is likely open (window outer/inner size delta, `console.profile` timing, `toString` timing) and **reward** rather than block. Do NOT gate content. Honest note: detection is unreliable across browsers and can break accessibility tools; use `sauron` console API as the primary interface instead of spooky detection.
Sketch:
```js
let t=performance.now(); console.log("%c", "color:transparent"); // fires devtools render
if(performance.now()-t>120) Sauron.ping("devtools-likely-open");
```
Never: `debugger;` loops, cursor hiding, "you're being watched" fake threats — those are hostile and damage the educational brand. Also provide `sauron.help()` (`console.table` of secrets, redacted until found) — see Section G.

### C6. Steganography on the web — difficulty 3–5
- **Image payloads**: EXIF/metadata fields (JPEG/TIFF) can carry plaintext; LSB steganography can be done fully client-side with `<canvas>` (write bits into R/G/B LSBs; extraction reverses it). Keep the carrier image small.
- **Base64 in assets**: fake "corrupted" asset that is actually base64 text; `fetch(asset).then(r=>r.text())`.
- **Audio spectrogram**: canonical art examples — Aphex Twin's "Equation" hides Richard D. James' face at ~5:27 (MetaSynth); "Windowlicker" ends with a spiral; Nine Inch Nails' Year Zero ARG hid images in spectrograms; Venetian Snares' cat. Browser implementation: generate the audio with WebAudio (draw text as frequency bars over 2–4s), and draw the spectrogram in-page on canvas *after* a discoverable "ANALYZE" action. This teaches the real technique instead of hiding it behind an external tool.
- **SVG path puzzles**: geometry as data (circle counts, path lengths), `clip-path` reveals, or a "connect the nodes" mini-canvas.
Sources: Aphex Twin FAQ: aphextwin.nu/learn/99906995499023.shtml · Wikipedia Windowlicker: en.wikipedia.org/wiki/Windowlicker · Mixmag: mixmag.net/feature/spectrogram-art-music-aphex-twin · spectrogram tool: github.com/roukaour/spectrogram

### C7. Cipher stacks — difficulty 2–4
A "stack" (layered encodings) is more satisfying than any single cipher:
`plaintext → ROT13 → Base64 → hex → reversed string`.
Utilities in vanilla JS:
```js
const rot13 = s => s.replace(/[a-z]/gi, c => String.fromCharCode((c<="Z"?90:122) >= (c=c.toUpperCase().charCodeAt(0)) ? c+13 : c-13));
const b64d = s => atob(s); const hexd = s => s.match(/../g).map(h=>String.fromCharCode(parseInt(h,16))).join("");
```
Also use: **Vigenère** (key = "ONION"), **book cipher** pointing at your own chapters (e.g., "Ch2 ¶4 word 7" — the site becomes the codebook; self-referential and evidence-brand-safe), **Morse** (audio beeps or .-/ text), **Bacon's cipher** (A/B via bold/italic styling), **acrostics**, and **PGP "signed message" theater** — show a real PGP-style block and a *clearly labeled* counterfeit signature, then teach how verification actually works (Cicada's public key `7A35090F` is the canonical ARG example; fake keys are the cautionary tale).
Sources: Cicada archive with PGP details: github.com/cicada-solvers/The-Complete-Cicada3301-Archive · scream314 liber_primus notes: github.com/scream314/cicada3301 · Notpron ciphers: en.wikipedia.org/wiki/Notpron

### C8. Time / locale / date triggers — difficulty 1–2
- **Clock windows**: local 03:33–03:34 (atmospheric, clearly labeled ART), or "after midnight."
- **Anniversaries with documented dates** (use these!): Oct 1/2 (Ulbricht arrest/Silk Road seizure 2013; Cicada 3301 kickoff Jan 4, 2012); Nov 5–6 (Onymous 2014); July 5 & 20 (AlphaBay/Hansa 2017); March 12 (WebTunnel 2024); Jan 21 (Ulbricht pardon 2025); Oct 16 (Welcome to Video announcement 2019); Sept 15 (Marques sentencing 2021).
- **Day-of-week / timezone**: `new Date().getDay()`, `Intl.DateTimeFormat().resolvedOptions().timeZone`.
Sketch:
```js
const d = new Date(); if(d.getMonth()===10 && d.getDate()===5) Sauron.unlock("onymous");
```
Hard rule: time-gated content must be duplicated in the meta-page (Section F) so nobody is locked out of facts.

### C9. State-based unlocks — difficulty 2–3
- **localStorage progress**: `sauron.found = ["E01","E03",...]`; counter chip "3/7 fragments."
- **Multi-step**: each payload checks predecessors before revealing the deep layer ("you found the SO post — now find the man who posted it").
- **Referral paths**: `?via=hansa` from a shared link shows a context card ("You arrived from the Hansa trail").
- **visit counters**: `visits>=7` unlocks a curator note.
Sketch:
```js
const K="sauron.v1"; const S=JSON.parse(localStorage.getItem(K)||"{}");
S.found=[...new Set([...(S.found||[]),"E01"])]; localStorage.setItem(K,JSON.stringify(S));
```
Testing tip: add `?reset=1` to clear state; guard localStorage in try/catch (private mode).

### C10. Ambient UI secrets — difficulty 1–3
- **Custom 404** (GitHub Pages `404.html`): mini-game + trailhead (Discord's 404 Snake is the canonical example).
- **Favicon flip**: draw with canvas → `link[rel=icon].href = canvas.toDataURL()`; trigger on discovery or `visibilitychange` (tab hidden >60s).
- **Tab-title ROT13**: on 5s idle, set `document.title` to ROT13 of the page title; restore on interaction.
- **Cursor swap**: `body{cursor:url("data:image/svg+xml;...")}` — subtle onion cursor after first unlock; respect `prefers-reduced-motion`.
- **Scroll velocity / scroll-up triggers**: reveal a "CLASSIFIED" strip when user scrolls up mid-chapter (Hansa correction card), or when scroll velocity spikes (skip-detection joke: "you skipped the evidence — here's the summary").
- **Back-to-top easter egg**: `.btt` click 7× → "The record goes back further than you think" + link to Ch 3.
- **Text-selection**: `::selection` custom color that reveals hidden glyphs (C4).
Sketch (favicon):
```js
const c=document.createElement("canvas");c.width=c.height=64;const x=c.getContext("2d");
x.fillStyle="#0a0";x.beginPath();x.arc(32,32,28,0,7);x.fill();
document.querySelector("link[rel=icon]").href=c.toDataURL();
```
Sources (404/Discord): en.wikibooks.org/wiki/A_Guide_to_Discord/Easter_Eggs · Konami Code wiki (web easter eggs list).


---

# SECTION D — ARG / PUZZLE DESIGN LESSONS (case studies)

Case-study base: Cicada 3301 (2012/13/14/16, archive: github.com/cicada-solvers/The-Complete-Cicada3301-Archive), Notpron (2004; 140 levels; creator interview: fastcompany.com/3036599; wiki: en.wikipedia.org/wiki/Notpron), i love bees (Halo 2, 2004; 42 Entertainment; ACM writeup: dl.acm.org/doi/fullHtml/10.1145/1314215.1314222), The Beast (A.I., 2001; if50.substack.com/p/2001-the-beast), Discord's 404 Snake, Google's search eggs, Sad Satan cautionary tale (Kotaku: kotaku.com/a-horror-game-may-be-hidden-in-the-darkest-corners-of-the-inte-1714980337; Wikipedia: en.wikipedia.org/wiki/Sad_Satan).

**15 transferable principles**

| # | Principle | Evidence / how it played out |
|---|---|---|
| D1 | **First secret must be findable within 60 seconds.** | Notpron Level 1 = "click the door" (fastcompany). i love bees' trailhead was a URL at the end of a trailer. The Beast's first clue was hidden in a movie poster image. Your E01/E02/E03 are the 60-second layer. |
| D2 | **The rabbit hole must be safe.** | i love bees sent FedEx packages and ran payphones — strange but harmless. Cicada peaked at "download an image, run outguess" — never required dangerous acts. Your version: reading + thinking, never installing anything, never visiting real markets. |
| D3 | **Layer difficulty in tiers, and let casuals stop happily.** | Notpron: 20M+ visitors, ~100 completions (Wikipedia). Anyone can do L1; almost nobody finishes. Design so each tier is a complete experience (Casual gets 7 fragments; Dedicated gets dossiers; Obsessive gets the Vault). |
| D4 | **Secrets should reward, never gate core content.** | Cicada's community solved in parallel across wikis/IRC; latecomers could still read everything. Never hide a fact that the article needs to make sense. Every secret duplicates to the disclosed meta-page (Section F). |
| D5 | **Design for community solvability.** | Cicada 3301's 2012 wave was solved by 4chan/IRC collective effort; the archive is community-maintained. Include copy-pasteable artifacts (cipher strings, spectrogram instructions) so friends can share the hunt. |
| D6 | **Fairness: step 1 uses in-band knowledge only.** | Notpron's early levels teach its own grammar (URL editing at level 2 → source comments later). The mistake ARGs make: requiring obscure out-of-band lore to even start. Your step 1: "look at the console/source" — universal dev curiosity. |
| D7 | **Sign your canonical trail; expect fakes.** | Cicada: "There are many fake messages out there. Only messages signed with public key ID 7A35090F are valid" + the 2017 PGP warning "beware false paths" (archive README). Your site: one canonical meta-page + a versioned footer note ("secrets list v1.0") so copycat clones are detectable. |
| D8 | **Always ship a meta-hint eventually.** | Notpron has a hints/community culture and a certificates page; Cicada explicitly signed its messages over years. When in doubt, add a hint in the console help (`sauron.help()`) rather than letting visitors wander forever. |
| D9 | **Teach while you trick (museum pedagogy).** | Every payload in Section E carries a sourced fact. The secret's *payoff* is knowledge, not a jump-scare. This is what separates your layer from creepypasta. |
| D10 | **Keep the fiction diegetic and humble.** | i love bees looked like a hacked beekeeper site; the A.I. wrote in corrupted HTML. Your dark theme can host "corrupted archive cards" — but they must confess they're art (colophon), per D12. |
| D11 | **Time-boxed moments create lore — but never FOMO-block facts.** | i love bees' countdowns ("network throttling will erode") drove daily returns; Cicada always returned on Jan 4. Use anniversary cards (E19) that are *bonus* content, with the same facts available year-round in the meta-page. |
| D12 | **Cautionary: unverifiable provenance curdles into misinformation.** | Sad Satan was framed as a "deep web game"; Kotaku later walked back credence, and the legend now feeds the very myths your site debunks. Rule: any in-site fiction is labeled ART; any factual claim carries a source. Never blur them for effect. |
| D13 | **Plan for rot.** | Notpron needed old browsers/plugins and lost levels; many ARG sites die. Your countermeasures: single self-contained file, no external assets required for secrets, no time-limited *facts*, and a "How this layer works" meta-page preserved in the repo. |
| D14 | **Accessibility is a design constraint, not an afterthought.** | Keyboard-only paths for every trigger (typed words work for motor accessibility; avoid twitch-timing). Respect `prefers-reduced-motion` (no flicker, no shake). Secrets reachable by screen reader: hidden text must also be exposed via `aria-describedby` or a "reveal" control. Reduced-motion media query is one line. |
| D15 | **Never point to real harm.** | The ARG genre's worst failure mode is trafficking in real gore/illegal links. Your layer's rule set (Section F) forbids operational content, real market references, or unverified addresses — only public institutional onions with verification steps. |

Additional craft notes worth shipping as a design doc:
- **Rule of three artifacts**: every "truth" fact should appear at least three times (article text, hidden payload, meta-page bibliography) so meaning survives partial discovery.
- **Red herrings should be labeled as myths, not punishment**: if someone follows a false trail, the payoff is a debunk card — the site's whole thesis.
- **Naming matters**: Cicada's prime 3301, Notpron's misspelling, ilovebees' mundane URL — memorable, copyable, unambiguous. Yours: "The Vault" / "Sauron" / "The Record."

---

# SECTION E — THE CATALOG (core deliverable)

30 payloads. Tier: **C** Casual (60-second, no tools), **D** Dedicated (readers looking under the hood), **O** Obsessive (tools/ciphers/state chains). Ch = chapter/section ID in your `index.html`. Every payload is TRUE-sourced or explicitly labeled ART/LEGEND. Implementation is vanilla JS/CSS only.

### E01 — "The Comment in the Hero" (C · intro/hero · source A01)
- **Secret content:** An HTML comment in the hero: `<!-- FROSTY WAS HERE. He asked the internet for help with his own marketplace. Ctrl+U → this comment. Console has the rest. -->` Payoff text inside the vault entry: the actual SO question URL + the "one minute too late" username rename fact.
- **Discovery mechanic:** Right-click → View Source (or Ctrl+U) on the hero. Also hinted by E02 console output.
- **Payoff moment:** Console prints a highlighted line; fragment counter starts `1/7`.
- **Implementation:** literally one HTML comment; `Sauron.ping("source")` when `sauron.help` is called after a 5s delay (proxy for source-viewing — or simply count E01 as "found" when the user opens Sauron.help).
- **Chain:** → E02 (console) → E11 (FROSTY typed).

### E02 — Console Banner + `sauron.help()` (C · all · sources A18, A23, A33)
- **Secret content:** Styled ASCII banner, then: "You are reading the source of a museum, not a market. Type `sauron.help()` for the record." Help output: `console.table` of secret IDs (found ones titled, unfound ones `████`), plus three commands: `sauron.about()`, `sauron.pledge()`, `sauron.decode("...")`.
- **Discovery mechanic:** Open DevTools (F12) on any load.
- **Payoff:** Full help table; `sauron.pledge()` returns the Tor "no backdoors, ever" quote with link A18.
- **Implementation:** `console.log("%c...", styles)`; expose `window.sauron = {...}` with a small command dispatcher; keep it non-interactive (no eval).
- **Chain:** entry point for all; `sauron.decode` feeds E13.

### E03 — Konami Code → Onion Rain (C · all · source: Konami history)
- **Secret content:** ↑↑↓↓←→←→BA triggers a gentle "peeling onion" overlay (Canvas: concentric translucent rings shedding), then toast: "Kazuhisa Hashimoto built this in 1986 because he couldn't beat his own game. Cheat codes are older than the web." + fragment.
- **Discovery mechanic:** Standard Konami sequence anywhere.
- **Payoff:** Overlay + fragment `+1`; after 30s the overlay offers "I prefer reading: here's the fact."
- **Implementation:** keydown buffer (~10 lines). Respect `prefers-reduced-motion` (replace animation with a static diagram).
- **Chain:** → E17 counter; contributes key A.

### E04 — Type ONION (three times) (C→D · architecture · sources A19, A24)
- **Secret content:** Typing `ONION` anywhere peels a small corner overlay showing a live onion-layer animation and the line: "Each hop peels one layer. The address is the public key." Second time: the v3 formula `Base32(ed25519 pk ‖ SHA3-256('.onion checksum'‖pk‖03)[:2] ‖ 03)`. Third time: a mini-tool — paste any 56-char onion address, it checks the checksum in-browser (educational, no network).
- **Discovery mechanic:** Typed buffer; hint appears once in console help.
- **Payoff:** Onion-checksum validator + rendezvous explainer card sourced to the Tor design paper.
- **Implementation:** buffer + tiny SHA3 not required — checksum verification needs SHA3; either implement a compact SHA3-256 in JS (~60 lines) or accept a "format validator" (charset + length + version byte) with a note. Prefer format validator for ship speed; upgrade later.
- **Chain:** → E21 `#rv` → key B.

### E05 — Selection Reveal (C · crypto · source A05)
- **Secret content:** In the Ch 8 paragraph about the laptop, a span with `color:transparent` whose `::selection` style reveals: "144,336. $48,238,116 in 2017. Then $1,000,000,000+ in 2020." Hover alternative: a small "reveal" button (a11y).
- **Discovery mechanic:** Text selection (or the ⟳ button).
- **Payoff:** Numbers animate into a ledger strip; footnote links to DOJ releases.
- **Implementation:** `.whiteout{color:transparent} .whiteout::selection{color:#e8e6e3;background:#1a1a2e}` + button toggling a class.
- **Chain:** → E13 (zero-width) → key C.

### E06 — Favicon Flip (C · all · technique C10)
- **Secret content:** Leave the tab hidden for 60s → onion favicon for 10s; toast on return: "The network noticed you looked away. Here's what it does when you don't: [WebTunnel fact, A32]."
- **Discovery mechanic:** `visibilitychange` + timer.
- **Payoff:** Favicon + fact card + fragment.
- **Implementation:** canvas → dataURL swap; restore after 10s; no animation needed.
- **Chain:** → E17.

### E07 — 404: "Down for Maintenance" (C · 404.html · source A15)
- **Secret content:** Custom 404 styled as the Freedom Hosting fake maintenance page, but clearly labeled ART. After 3s it flips: "This page is a reconstruction. On Aug 4, 2013, a real maintenance page was the payload." Then the full EgotisticalGiraffe/CVE-2013-1680 sourced card.
- **Discovery mechanic:** Any broken URL.
- **Payoff:** The flip + fragment; link to A15 sources.
- **Implementation:** `404.html` with a 3s `setTimeout` class toggle. Must be a separate file — GitHub Pages serves it automatically.
- **Chain:** → E23 (codename console) → key A.

### E08 — robots.txt Breadcrumb (D · /robots.txt · technique C3)
- **Secret content:** Standard Disallow block plus a comment line: `# Door 2 is where the CAPTCHA used to be.` (references AlphaBay's password-reset email failure — "where the CAPTCHA used to be" is flavor; the real payload is the ROT13 line below it: "Gur zbfg frpher cneg bs gur vagrearg vf gur cneg lbh hcybnq lbhefrys" → decode: a sourced line about OpSec).
- **Discovery mechanic:** Visit `/robots.txt`.
- **Payoff:** Decoded line + pointer to E14. Meta-page records the decode.
- **Implementation:** static file next to `index.html`.
- **Chain:** → E14.

### E09 — security.txt, The Real RFC (D · /.well-known/security.txt · SOURCE: RFC 9116)
- **Secret content:** A *valid* RFC 9116 file (`Contact:`, `Expires:`, `Preferred-Languages: en, si`) plus `# NOTE:` lines explaining the spec, ending with: "The site has no vulnerabilities to report. The internet does. Policy: read Chapter 10."
- **Discovery mechanic:** Standard well-known path; also linked from the meta page and console help.
- **Payoff:** Teaches a real standard; unlocks a Ch 10 note card about vulnerability disclosure ethics.
- **Implementation:** static file; template from rfc-editor.org/rfc/rfc9116.
- **Chain:** → E02 (help table annotation).

### E10 — humans.txt (C · /humans.txt · technique C3)
- **Secret content:** ASCII art colophon + "Humans behind the record:" and a hidden NUL-separated line? Keep it simple: includes the line `/* TEAM: the people who lost their freedom so this page could be footnoted */` — respectful nod to primary sources, no glamorization.
- **Discovery mechanic:** Type `/humans.txt`.
- **Payoff:** Sourced colophon + a "titles" toggle that reveals curator notes on Key Figures.
- **Implementation:** static file (or a pre block in-file for GitHub Pages single-file constraint — a real file is better since the brief allows assets).
- **Chain:** → E30 meta page mention.

### E11 — Type FROSTY (D · opsec · source A01)
- **Secret content:** Full SO post reproduction (code block + link + timeline of the username edit) framed as "Exhibit A-01." Also the "sock puppet" note: Altoid → frosty → DPR naming trail.
- **Discovery mechanic:** Type `frosty` anywhere.
- **Payoff:** Exhibit drawer slides up; sourced; fragment +1.
- **Implementation:** buffer listener + a hidden `<article>`.
- **Chain:** → E12 → key A.

### E12 — Timeline Whisper (D · history · source A03/A05)
- **Secret content:** Click the "2013" node in the history timeline **7 times** → it flips to "Exhibit A-03: the arrest." Inside: three collapsible facts (SO post, Gmail, laptop grab) each with source links; ends with "Seven clicks. The FBI spent two years."
- **Discovery mechanic:** 7 clicks on the 2013 element (also mobile: long-press).
- **Payoff:** Exhibit panel + fragment.
- **Implementation:** click counter with a 1s decay; `aria-expanded` for the panel.
- **Chain:** → key A complete.

### E13 — Zero-Width Letter (D · opsec · source A02/A30)
- **Secret content:** A zero-width-encoded sentence embedded in a visible paragraph: "email addr + timestamps = indictment." Copying the paragraph and pasting into the site's decoder (or reading `sauron.decode` in console) reveals it. The meta-page explains the encoding and why invisible characters are a real forensic topic.
- **Discovery mechanic:** Select + copy a specific paragraph in Ch 7 and paste into the decoder input that appears after E05 is found.
- **Payoff:** Decoded line + ZWSP explainer card + fragment.
- **Implementation:** encoder used at authoring time (bits→ U+200B/U+200D); decoder ~6 lines (see C4).
- **Chain:** → E16 (spectrogram) → key C.

### E14 — The Hansa Correction (D · market · source A08/A09)
- **Secret content:** Scroll down past the market table then scroll **up** — a "CLASSIFIED" strip slides in: "Everyone says 27,000 IPs. The primary reporting says 27,000 transactions. One word, and the legend grows." Links to WIRED. Then the Hansa honeypot timeline (June 20 → July 20, Excel trap, 64 sellers).
- **Discovery mechanic:** Scroll-direction listener (deltaY < 0 after passing 60% of section).
- **Payoff:** Correction card + fragment; double-click the card unlocks the longer "Operation Bayonet" dossier.
- **Implementation:** `scroll` listener with threshold + throttling; `prefers-reduced-motion` → static reveal button.
- **Chain:** → E17 → key B.

### E15 — The Ledger (D · crypto · source A05/A29)
- **Secret content:** A "ledger terminal": user types wallet labels (fictional labels: `LAPTOP-144336`, `INDIVIDUAL-X`, `SERVER-29655`) to retrieve the documented totals and outcomes. Each entry reveals a sourced fact; entering `INDIVIDUAL-X` reveals the 101 BTC → BTC-e 2015 trace.
- **Discovery mechanic:** Terminal input at the end of Ch 8 (also `sauron.ledger` console command).
- **Payoff:** Ledger rows animate; fragment.
- **Implementation:** whitelist map + `<output>` element; no network.
- **Chain:** → E29 vault prerequisite.

### E16 — Spectrogram (O · crypto · source: Aphex Twin, Windowlicker)
- **Secret content:** A generated 3-second audio clip (WebAudio) described as "the noise from a seized hard drive." Press **ANALYZE** (a button that only appears after E13) to render the spectrogram on canvas: the frequency bars spell **RENDEZVOUS**. Educational card: Aphex Twin's face at 5:27 in "Equation" via MetaSynth; how to do this in Audacity.
- **Discovery mechanic:** E13 → analyze button; or `sauron.decode("spectro")`.
- **Payoff:** Visual message + method explainer + fragment.
- **Implementation:** WebAudio oscillator bank drawn from a bitmap font (letters drawn as frequency columns); spectrogram via `AnalyserNode` + canvas or direct fill (simpler: pre-computed bar data). ~80 lines. Ship as stretch goal.
- **Chain:** → key C complete.

### E17 — Fragment Counter (all tiers · all · meta)
- **Secret content:** A subtle HUD chip ("fragments 3/7") appears once the first fragment is found. Fragments: E01, E03, E07, E11, E14, E15, E19. At 7/7: "The Vault is open" (E29).
- **Discovery mechanic:** Just play; chip is visible bottom-right; click shows found/unknown hints.
- **Payoff:** Vault unlock.
- **Implementation:** localStorage state; `Sauron.fragment(id)`; aria-live polite announcements.
- **Chain:** hub of all chains.

### E18 — 03:33 (C · all · ART-labeled)
- **Secret content:** Visit between 03:33–03:34 local (or UTC toggle) → an atmospheric card, clearly labeled ART: "For one minute, the only traffic in the room is yours." Plus a TRUE footnote: what LE timestamps in the Playpen/AlphaBay cases show about time zones (link A16/A10).
- **Discovery mechanic:** Clock check on load + interval.
- **Payoff:** Card + fragment flag (counts as bonus, never required for Vault).
- **Implementation:** `Date` check; localStorage flag per day; reduced-motion safe.
- **Chain:** bonus.

### E19 — Anniversary Cards (C/D · all · sources: A03/A05/A08/A15/A25)
- **Secret content:** On documented anniversaries, a small museum placard appears in the relevant chapter: Oct 1 (arrest), Nov 5–6 (Onymous: "414 claimed → 267 documented → 153 clones"), July 5/20 (Bayonet funnel), Sept 15 (Marques sentencing), Jan 21 (pardon), March 12 (WebTunnel), Oct 16 (Welcome to Video), Jan 4 (Cicada homage — labeled HOMAGE).
- **Discovery mechanic:** Date match on load.
- **Payoff:** Placard + source links; the same cards are permanently available in the meta-page so nothing is FOMO-locked.
- **Implementation:** small date→card map; UTC+local dual display.
- **Chain:** feeds fragments/keys as bonus.

### E20 — Timeline 1986/1995/2004 (C · history · source A23)
- **Secret content:** Clicking the years in the "Origins" timeline reveals source cards: 1986 (Konami code! cross-link), 1995 (NRL question), 1998 (Navy patent), 2004 (EFF funds Tor + USENIX paper), 2006 (nonprofit).
- **Discovery mechanic:** Click year nodes.
- **Payoff:** Source drawer with the USENIX abstract quote.
- **Implementation:** buttons + details panel.
- **Chain:** → E03 cross-link.

### E21 — `#rv` Rendezvous Route (C→D · architecture · source A24)
- **Secret content:** Visiting `#rv` (hash route) scrolls to a hidden "Rendezvous" mini-section explaining why hidden services need meeting points. Contains a diagram and a line from the Tor design paper.
- **Discovery mechanic:** Hash in URL; also revealed by E04's third activation. Console help lists `sauron.route("rv")`.
- **Payoff:** Hidden subsection + fragment.
- **Implementation:** `hashchange` handler showing a hidden `<section>` (also directly navigable for a11y).
- **Chain:** → key B.

### E22 — Type SHISHKABOBS (D · opsec · source A16)
- **Secret content:** Playpen's most famous NIT case username. Typing it opens "The two weeks the government ran the site" — NIT facts (IP + OS username + MAC), Rule 41 split, rescue numbers.
- **Discovery mechanic:** Typed buffer (console hint hidden until E07 found).
- **Payoff:** Case card + fragment; cross-link to A16 court PDFs.
- **Implementation:** as E11.
- **Chain:** → key A.

### E23 — Codename Giraffe (D · zeroday · source A15/CVE-2013-1680)
- **Secret content:** In Ch 9's Freedom Hosting passage, a hidden line of JS comment: `/* the giraffe was egotistical */`. Typing `egotisticalgiraffe` in console (or the terminal) opens a card: CVE-2013-1680 explained, Firefox 17 ESR targeting, the Virginia beacon, Snowden-slide codename, Marques outcome.
- **Discovery mechanic:** Source comment + typed codename; unlocked fully after E07.
- **Payoff:** Exploit card with CVE link + fragment.
- **Implementation:** buffer + hidden article.
- **Chain:** → key A.

### E24 — `sauron.pledge()` / "Wi-Fi doesn't lie" (C · censorship · sources A18/A17)
- **Secret content:** Console command prints the Tor Project's "no backdoors, ever" line with link; second command `sauron.wifi()` prints the Eldo Kim fact: "Tor hides where you go. It doesn't hide that you went."
- **Discovery mechanic:** Console commands (list in help).
- **Payoff:** Two sourced quote cards.
- **Implementation:** command map in Sauron object.
- **Chain:** → E29 vault content seed.

### E25 — Logo ×7 → "The Office" (D · future · source A31)
- **Secret content:** Click the site logo 7 times → a Ch 12 sidecard: "The market moved. Telegram blocked 43.5M+ channels in 2025; the ecosystem re-created itself (gated joins, backups, bots). DNM flows ~$2.6B in 2025." Links to Chainalysis/Check Point.
- **Discovery mechanic:** 7 clicks on the logo (mobile: long-press).
- **Payoff:** Sidecard + fragment (bonus).
- **Implementation:** debounce counter.
- **Chain:** bonus → vault source list.

### E26 — "Which Onions Are Real?" Quiz (D · use · sources A20–A22)
- **Secret content:** A five-item quiz: match institutional onion services (CIA, BBC, NYT, ProPublica, Facebook v2 story) with facts; completing it shows the verification protocol (check official clearnet page → copy address → verify checksum) and a safety note. The NYT's 2025 shutdown is the twist answer ("this one quit").
- **Discovery mechanic:** Small interactive in Ch 5 (visible button "pop quiz").
- **Payoff:** Verification guide + fragment.
- **Implementation:** radio/drag-simple; no external links from quiz (meta page holds them).
- **Chain:** → E30 meta page.

### E27 — Binary Title (C · layers · technique C10)
- **Secret content:** 30s of no scroll in Ch 4 → the tab title becomes `01001111 01001110 01001001 01001111 01001110` for 3s; toast: "ONION. Now you know what binary looks like in the tab — here's why layered routing got the name."
- **Discovery mechanic:** Idle timer.
- **Payoff:** Title change + explainer card.
- **Implementation:** `setTimeout`/`scroll` debounce; restore.
- **Chain:** → E17.

### E28 — Garlic Comment (D · alt darknets · source: I2P architecture)
- **Secret content:** HTML comment in Ch 11: `<!-- i2p calls it garlic routing. layers within layers. some networks you can't peel. -->` + a small riddle whose answer ("garlic") typed in console opens a comparison card: Tor (onion, circuit-based, clearnet exits) vs I2P (garlic, packet-based, internal-only) vs Freenet (datastore). 
- **Discovery mechanic:** Source comment + typed answer.
- **Payoff:** Comparison card + fragment.
- **Implementation:** buffer + hidden article.
- **Chain:** bonus.

### E29 — CHAPTER 13: THE VAULT (O · finale · all sources)
- **Secret content:** A hidden chapter unlocked by **any 5 of 7 fragments** (or all three chain keys). Design: a museum vault door (CSS), opening into a bibliography-gallery: 7 "greatest hits" exhibits — (1) The Stack Overflow post; (2) $1B Individual X; (3) Hansa's Excel trap; (4) EgotisticalGiraffe; (5) Playpen NIT & Rule 41; (6) Welcome to Video's ledger; (7) "no backdoors, ever." Each exhibit: 120-word summary + 2 primary links + a "what it teaches" line. Ends with the curator colophon: how the hidden layer works, all secrets listed, and the ethics statement.
- **Discovery mechanic:** 5/7 fragments via E17.
- **Payoff:** Full-screen vault reveal; confetti? No — a quiet "You found the record" + the site's own name in ASCII + Sinhala line (see G).
- **Implementation:** hidden `<section id="vault">` shown by state; deep-linkable `#vault` once unlocked (store flag); focus trap; Esc closes; reduced-motion variant.
- **Chain:** terminal node.

### E30 — Meta Page: "About the Hidden Layer" (C · all · education/ethics)
- **Secret content:** Disclosed spoiler page: why secrets exist, the full list, all sources, accessibility notes, how to clear state (`?reset=1`), and a pledge that no payload contains operational/illegal content. Marked `noindex`, linked from the Vault and from `humans.txt`.
- **Discovery mechanic:** Direct link in Vault + `sauron.meta()` + humans.txt.
- **Payoff:** Transparency; the site's "art vs. fact" boundary made explicit.
- **Implementation:** hidden `<section>`; meta robots noindex applies to separate files only — for a hidden in-page section, add `<meta name="robots" content="noindex">` on any dedicated HTML files and keep the main page indexable.
- **Chain:** terminal node.

## Chains

**Chain 1 — "The Operator's Trail" (truth chain):**
E01 hero comment → E02 console help → E11 FROSTY exhibit → E12 timeline ×7 → **Key A** ("Operator"). Vault line: "He was caught by his own questions."

**Chain 2 — "The Layers" (architecture chain):**
E04 ONION ×3 → E06 favicon → E21 `#rv` → E14 Hansa correction → **Key B** ("Layers"). Vault line: "Every layer is a promise and a risk."

**Chain 3 — "The Cipher" (forensics chain):**
E05 selection → E13 zero-width decode → E16 spectrogram → E15 ledger → **Key C** ("Ledger"). Vault line: "The money never forgets, and neither does the record."

**Meta-chain:** E17 counter tracks 7 fragments (E01, E03, E07, E11, E14, E15, E19). Any 5 unlock the Vault (E29); all 7 add a curator's note. Three keys = the "perfect run" badge.

## Copy bank (tone: serious, sourced, never smug)

- Toast: `Fragment recovered. The record grows. 3/7.`
- Console: `You are reading the source of a museum. Nothing here is for sale. Everything here is footnoted. Type sauron.help().`
- Konami: `A cheat code from 1986, kept in by accident. History is full of kept-in accidents. (+1 fragment)`
- Hansa card: `Primary sources say 27,000 transactions. The legend says 27,000 IPs. One word makes the police look like wizards.`
- Vault welcome: `You found the record. Seven exhibits, every one of them verified in a courtroom, a federal filing, or a peer-reviewed paper. Read slowly.`
- Meta page intro: `These secrets exist to teach, not to tease. If you only take one thing: verification beats vibes.`


---

# SECTION F — SAFETY, ETHICS, LEGAL & ANTI-MISINFO

## F1. Keep the site unambiguously art/education
- **Colophon in the Vault** (E29/E30) stating: this hidden layer is an educational art project; facts are sourced; fiction is labeled; no illegal content or operational guidance exists anywhere in the layer.
- **Labels everywhere**: `LOGGED FACT` (court/DOJ/paper), `REPORTED` (journalism), `LEGEND` (folklore, presented as folklore), `ART` (atmospheric device by the site authors). Put the label in the UI chip, not just the prose.
- **Spoiler/meta page**: E30 lists every secret and its solution. Curiosity is rewarded; obscurity is never the only protection. This is also your anti-misinfo firewall: if someone claims "the site hides X," the meta-page is the canonical answer.

## F2. Must-avoid list (hard rules for shipped code)
1. **No real darknet market links** — historic or current; not even dead ones (mirrors and phishing clones still hurt people). Describe operations by name only (Silk Road, Hansa, AlphaBay), never by address.
2. **No operational guidance**: no OpSec "how to," no market discovery methods, no vendor tips, no evasion instructions. History and forensics only.
3. **No unverified onion addresses.** Institutional addresses are allowed *with verification instructions*, and only for persistently public organizations: CIA (A20), BBC/NYT/ProPublica SecureDrop (A22), Tor Project. Even then: link the clearnet announcement page and teach checksum verification rather than reproducing the address as a clickable target on its own. Note the NYT shut its service down in 2025 — a built-in lesson that addresses rot.
4. **CSAM handling**: refer to cases and statistics only. Never describe abuse content, never name victims, never link material. Keep the language clinical (the DOJ releases model this).
5. **No "spooky" scareware**: no fake threats, no fake malware warnings, no devtools-blocking, no fullscreen jumpscares, no audio auto-play.
6. **No glorification**: present convicts as case studies with outcomes (sentences, deaths in custody, rescues) — never as heroes; never reproduce racist/abusive language beyond what a court quote requires, and then only with a content note.
7. **No real PGP keys/signatures** pretending to be authentic. "Signed message theater" must show obviously-fake example keys and teach verification; never imitate a real signer (Cicada's key 7A35090F is a fact to discuss, not to spoof).

## F3. Footnote discipline for hidden facts
- Every payload fact gets: `source` (URL), `sourceType` (court/DOJ/paper/reporting), `date`, `confidence` (HIGH/MED/LOW). Store these as `data-*` attributes so the Vault can render an automatic bibliography.
- Two-source rule for the juicy claims; label single-source facts as `REPORTED` in the UI.
- Corrections are features: publish the "27,000 transactions, not IPs" fix and the "$13.4M doesn't exist" note. The site's brand is "verification beats vibes" — the hidden layer should model it.

## F4. Accessibility & reduced motion
- **Keyboard parity** for every trigger: typed words and buttons work for all; mouse-only mechanics get a keyboard equivalent (document it in console help).
- **Screen readers**: any content revealed by selection/zero-width has an explicit "Reveal" button with `aria-expanded`; zero-width payloads are re-stated in plain text in the meta page. Never make the *fact* available only through a trick.
- **`prefers-reduced-motion`**: disable flicker, rain, shake, scroll-jacking; replace with static diagrams. One media query + a `data-reduced` flag on `<html>`.
- **Focus management** for overlays/vault: focus trap, Esc closes, returns focus to trigger.
- **Contrast**: hidden text isn't "hidden" for low-vision users — keep the reveal mechanism visible (a small ⟳/Reveal control next to any concealment).
- **Timing**: no timed puzzles; typed buffers have generous windows; anniversary content is duplicated year-round (D11).

## F5. SEO / robots.txt interplay
- **Main page**: fully indexable; it's the product.
- **Hidden routes on the same page** (hash routes like `#rv`, `#vault`): hashes aren't crawlable as separate pages, so they stay human-findable and machine-invisible. Good.
- **Separate hidden files** (`vault.html`, `meta.html` if you split them): add `<meta name="robots" content="noindex,nofollow">` — this works on GitHub Pages where you can't set HTTP headers. Do **not** rely on `robots.txt` for secrecy (crawlers may ignore it; and Disallow lines reveal paths — use that effect deliberately, as in E08, but treat it as a breadcrumb, not a lock).
- **robots.txt design**: allow the public page; include one deliberate, harmless comment breadcrumb (E08). Never list real sensitive paths in it. Sitemap: include only public content.
- **GitHub Pages note**: `404.html` is served automatically; `/.well-known/security.txt` **cannot** be served as a directory-root dot-folder on GitHub Pages reliably (serve it as `/security.txt` and/or a `.nojekyll` + static path workaround — test it; RFC allows the legacy `/security.txt` location as well as `/.well-known/`). This is a real gotcha: GitHub Pages does not special-case `.well-known`; create the path as a folder with a file and verify. If it 404s, host the file at `/security.txt` and explain the legacy location in the copy.
- **Wayback**: expect the hidden pages to be archived eventually. That's fine — they contain no secrets worth hiding from history; the meta-page is public anyway.

## F6. Legal & content review checklist (ship-blockers)
- [ ] No illegal goods/services offered, described procedurally, or linked.
- [ ] Onion addresses only institutional + verification taught (F2.3).
- [ ] Quotes from court docs are accurate and attributed; fair-use amounts; no long copyrighted excerpts.
- [ ] Sensitive-case copy reviewed for victim-safety (no names, no identifying details of minors; the site covers CSAM topics in aggregate stats only).
- [ ] Sri Lanka context: the creator is Sri Lankan — the site is educational and hosted on GitHub Pages; keep the "no operational content" stance visible, since local law and platform policy both punish facilitation far more than documentation. (General guidance, not legal advice — for a public-facing product, a quick consult with a local lawyer familiar with cybercrime statutes is cheap insurance.)
- [ ] Donation/contact paths (if any) don't imply affiliation with any agency or market.

## F7. Anti-misinformation protocol (the layer's own quality bar)
1. Before shipping any hidden fact, run the **three-question test**: Is it sourced to a primary document? Does a second independent source agree? Does the UI label its confidence?
2. Keep a **corrections log** in the repo/meta-page; version the hidden layer (`secrets v1.0`) so screenshots circulating out of context remain checkable.
3. Myths get debunk cards, not silence (B01–B18 supply the copy).
4. Never let fiction share a visual container with fact without a label. Different chip, different color, explicit word: `LEGEND` vs `LOGGED FACT`.
5. If a claim can't be verified (Red Rooms, Mariana's Web, DeSnake's claims), say exactly that — "no verified instance is documented" — which is more interesting than a maybe.

---

# SECTION G — IMPLEMENTATION BLUEPRINT

## G1. Architecture inside the single self-contained HTML file

Namespacing: one global object, `window.SAURON`, plus a registry. Everything is additive — no build step, no dependencies.

```html
<!-- in <head> -->
<meta name="description" content="An evidence-based technical investigation of the dark web.">
<!-- hidden-layer state class flips here once anything is unlocked -->
```

```js
/* ============ SAURON: hidden layer core (vanilla JS) ============ */
const Sauron = (() => {
  const VERSION = "1.0";
  const KEY = "sauron.state.v1";
  const read = () => { try { return JSON.parse(localStorage.getItem(KEY)) || {}; }
                       catch(e){ return {}; } };
  const write = s => { try { localStorage.setItem(KEY, JSON.stringify(s)); } catch(e){} };

  const state = read();
  state.found = state.found || [];     // payload ids
  state.keys  = state.keys  || [];     // chain keys A/B/C
  state.flags = state.flags || {};     // misc booleans (devtools, konami...)

  const listeners = {};
  const on = (ev, fn) => (listeners[ev] = [...(listeners[ev]||[]), fn]);
  const emit = (ev, data) => (listeners[ev]||[]).forEach(fn => fn(data));

  function fragment(id, label) {
    if (state.found.includes(id)) return;
    state.found.push(id); write(state);
    emit("fragment", { id, label, count: state.found.length });
    Toast.show(`Fragment recovered — ${label}. ${state.found.length}/7.`);
  }
  function key(k, label) {
    if (state.keys.includes(k)) return;
    state.keys.push(k); write(state); emit("key", { k, label });
    Toast.show(`Key ${k} recovered — ${label}.`);
  }
  function unlock(id) { emit("unlock:" + id); fragment(id, LABELS[id] || id); }

  /* typed-word listener: call once */
  function words(map) {
    let buf = "";
    addEventListener("keydown", e => {
      if (/^[a-z]$/i.test(e.key)) buf = (buf + e.key.toLowerCase()).slice(-24);
      else if (e.key !== "Shift") buf = "";
      for (const [w, fn] of Object.entries(map))
        if (buf.endsWith(w)) { fn(); buf = ""; }
    });
  }

  /* console API */
  const api = {
    version: VERSION,
    help() { console.table((window.SECRETS || []).map(s => ({
        id: s.id, tier: s.tier, title: state.found.includes(s.id) ? s.title : "████" }))); },
    decode(s) {
      // base64 → rot13 → hex, in that order if applicable
      let t = s; try { t = atob(t); } catch(e){}
      t = t.replace(/[a-z]/gi, c => String.fromCharCode(
        (c.toUpperCase() >= "N" ? 90 : 122) >= c.toUpperCase().charCodeAt(0) + 13
          ? c.charCodeAt(0) + (c === c.toUpperCase() ? 13 : 13) : c.charCodeAt(0) - 13));
      console.log("%cdecoded","color:#7cf", t); return t;
    },
    about() { console.log("%cTHE DARK WEB BRIEF — hidden layer v" + VERSION, "font-weight:700",
      "\nEverything hidden here is sourced. See the meta page: #secrets"); },
    pledge() { console.log('%c"A backdoor is a vulnerability by another name."',
      "color:#e8e6e3", "\n— Tor Project statement, 2016: blog.torproject.org/statement-tor-project-software-integrity-and-apple"); }
  };
  return { VERSION, state, on, emit, fragment, key, unlock, words, api, write };
})();
window.sauron = Sauron.api;
```

**SecretRegistry** (data, not code — render the meta page from it):
```js
window.SECRETS = [
  { id:"E01", tier:"C", chapter:"hero",  title:"The Comment in the Hero",      source:"https://stackoverflow.com/questions/15445285" },
  { id:"E03", tier:"C", chapter:"all",   title:"Konami: 1986",                  source:"https://en.wikipedia.org/wiki/Konami_Code" },
  /* ... 30 entries ... */
];
```

**Wire-ups (each ~5–15 lines):**
```js
/* E01: source viewer proxy — count as found when help() is used after first visit */
if (!Sauron.state.flags.helped) Sauron.on("help-called", () => Sauron.unlock("E01"));

/* E03: Konami */
const KON = [38,38,40,40,37,39,37,39,66,65]; let ki = 0;
addEventListener("keydown", e => {
  ki = (e.keyCode === KON[ki]) ? ki+1 : 0;
  if (ki === KON.length) { ki = 0; Sauron.unlock("E03"); document.documentElement.classList.add("onion-rain"); }
});

/* E04: typed words */
Sauron.words({
  onion:    () => Sauron.state.flags.onion = (Sauron.state.flags.onion||0)+1,   // levels 1/2/3
  frosty:   () => Sauron.unlock("E11"),
  shishkabobs: () => Sauron.unlock("E22"),
  egotisticalgiraffe: () => Sauron.unlock("E23"),
  garlic:   () => Sauron.unlock("E28")
});

/* E06: favicon flip on tab-hidden 60s */
let hiddenAt = 0;
addEventListener("visibilitychange", () => {
  if (document.hidden) hiddenAt = Date.now();
  else if (hiddenAt && Date.now()-hiddenAt > 60000) { flipFavicon(); Sauron.unlock("E06"); }
});

/* E21: hash router */
addEventListener("hashchange", showFromHash); function showFromHash(){
  const id = location.hash.replace("#","");
  document.querySelectorAll("[data-route]").forEach(el =>
    el.hidden = el.dataset.route !== id);           // default hidden
}

/* E17: HUD */
Sauron.on("fragment", () => {
  const n = Sauron.state.found.length;
  document.getElementById("frag-count").textContent = n + "/7";
  if (n >= 5) document.getElementById("vault-link").hidden = false;
});
```

**CSS helper classes:**
```css
.whiteout { color: transparent; }
.whiteout::selection { color:#e8e6e3; background:#1a1a2e; }
.reveal-btn { /* visible affordance for a11y */ }
[hidden] { display:none !important; }                    /* keep explicit */
@media (prefers-reduced-motion: reduce) {
  .onion-rain, .peel { animation: none !important; }
}
.legend-chip::after { content:"LEGEND"; }
.fact-chip::after   { content:"LOGGED FACT"; }
```

**Toast component** (single DOM node, aria-live polite, 6s auto-dismiss, reduced-motion = fade only):
```js
const Toast = {
  show(msg){ const t = document.getElementById("toast");
    t.textContent = msg; t.dataset.on = "1";
    clearTimeout(Toast._t); Toast._t = setTimeout(() => delete t.dataset.on, 6000); }
};
```

**State reset**: `?reset=1` clears localStorage and reloads; also `sauron.reset()` — document in E30.

## G2. Priority build order (ship this week → later)

**First wave — 10 payloads, best payoff/effort (target: 2–3 evenings):**
1. E02 console banner + `sauron.help()` (core infrastructure for everything else).
2. E01 hero comment (one line, huge discovery moment).
3. E03 Konami (10 lines, universally loved).
4. E04 typed ONION + step-2 formula card (typed-words utility reused everywhere).
5. E05 selection reveal (3 lines CSS + reveal button).
6. E07 404 "Down for Maintenance" flip (single file, best theatrical payoff).
7. E08 robots.txt breadcrumb + decode utility (teaches `sauron.decode`).
8. E17 fragment HUD + storage (the meta-spine).
9. E29 Vault skeleton with 3 exhibits at launch (grow to 7).
10. E30 meta page (transparency + ethics; required for school-safe framing).

**Second wave (next weekend):** E11 FROSTY exhibit, E12 timeline ×7, E14 Hansa scroll-up, E15 ledger terminal, E19 anniversary cards, E21 #rv route, E24 pledge commands, E26 onions quiz, E27 binary title.

**Stretch (Obsessive tier):** E13 zero-width + decoder, E16 spectrogram (largest build), E18 03:33, E22/E23 typed cases, E25 logo ×7, E28 garlic.
**Never ship without:** the F2 hard rules audit + F4 a11y pass + E30 live.

## G3. Copy tone guide (serious brand)

Do:
- Speak like a museum placard: facts first, dates, sources.
- Let the dark theme carry atmosphere; copy stays calm.
- Addresses the reader as an investigator, not a "1337 hacker."
- Ends discoveries with a link, not a wink.

Don't:
- No leetspeak, no "you have been chosen," no fake threats, no "delete this message."
- No fake timers/urgency.
- No real agency logos or impersonation.
- No jokes that punch down at victims.

Sample strings (ship-ready):
- First console line: `THE DARK WEB BRIEF — the hidden layer. Nothing here is for sale. Everything here is footnoted. Type sauron.help().`
- Fragment toast: `Fragment recovered — "The Operator's Trail." 3/7.`
- Konami: `A cheat code from 1986, kept in by accident. History is full of kept-in accidents. (+1 fragment)`
- Vault door: `You found the record. Seven exhibits. Every one verified by a court, a federal filing, or a peer-reviewed paper. Read slowly.`
- Meta page: `These secrets exist to teach, not to tease. Claims carry sources; folklore carries labels. Verification beats vibes.`
- Sinhala release line (optional, for the creator's community): `මෙය රහසක් නොවේ. මෙය වාර්තාවක්.` ("This is not a secret. This is a record.")

## G4. QA checklist (pre-ship)
- [ ] Every trigger works with keyboard only (tab to controls; typed words tested in Chrome/Firefox/Safari/mobile).
- [ ] `prefers-reduced-motion` test pass on all animations.
- [ ] Private-mode localStorage failure doesn't break the site (try/catch verified).
- [ ] No console errors; `sauron.help()` table renders with 30 entries.
- [ ] All 30 payloads labeled with tier/chapter/source in `SECRETS`.
- [ ] Vault reachable via 5/7 and via `#vault` after unlock; `?reset=1` works.
- [ ] Meta page lists all secrets + sources + a11y statement.
- [ ] F2 audit: no market links, no operational content, only institutional onions with verification, no victim details.
- [ ] Wayback check after launch: `http://web.archive.org/save/` the meta page so the canonical version is archived.

---

# APPENDIX — MASTER SOURCE LIST (selected)

**Primary/court/DOJ:** archive.org/details/UlbrichtCriminalComplaint_201310 · justice.gov/archive/usao/nys/pressreleases/February14/RossUlbrichtIndictmentPR.php · ice.gov/doclib/news/releases/2013/131002baltimore.pdf · justice.gov/usao-sdny/pr/manhattan-us-attorney-announces-seizure-additional-28-million-worth-bitcoins-belonging · justice.gov/usao-sdny/pr/acting-manhattan-us-attorney-announces-forfeiture-48-million-sale-silk-road-bitcoins · justice.gov/usao-ndca/pr/united-states-files-civil-action-forfeit-cryptocurrency-valued-over-one-billion-us · justice.gov/archives/opa/press-release/file/982826/dl?inline (Cazes indictment) · justice.gov/usao-md/pr/dark-web-child-pornography-facilitator-sentenced-27-years-federal-prison-conspiracy · justice.gov/archives/opa/pr/south-korean-national-and-hundreds-others-charged-worldwide-takedown-largest-darknet-child · justice.gov/archives/opa/pr/international-law-enforcement-operation-targeting-opioid-traffickers-darknet-results-over-170 · justice.gov/usao-ma/pr/harvard-student-charged-making-hoax-bomb-threat · fbi.gov/newyork/press-releases/2014/manhattan-u.s.-attorney-announces-the-indictment-of-ross-ulbricht-the-creator-and-owner-of-the-silk-road-website · fbi.gov/news/stories/playpen-creator-sentenced-to-30-years · fbi.gov/history/artifacts/ross-william-ulbrichts-laptop · govinfo.gov (Playpen NIT court PDFs: USCOURTS-ned-4_15-cr-03134-6/-8, ca2-17-03367) · eff.org/pages/playpen-cases-frequently-asked-questions

**LE agency/EU:** europol.europa.eu (Bayonet 2017; DisrupTor 2020) · cia.gov/stories/story/cias-latest-layer-an-onion-site · dea.gov/press-releases/2020/09/22/... · fbi.gov/news/stories/operation-disruptor-jcode-shuts-down-darknet-drug-vendor-092220

**Academic:** ieee-security.org/TC/SP2013/papers/4977a080.pdf · usenix.org/legacy/event/sec04/tech/full_papers/dingledine/dingledine.pdf · usenix.org/conference/usenixsecurity15/technical-sessions/presentation/kwon · usenix.org/system/files/soups2024_poster7-berger_final.pdf · usenix.org/system/files/soups2024_poster3-fassl_final.pdf · par.nsf.gov/servlets/purl/10485912 (v3 onions) · resources.mpi-inf.mpg.de/d5/teaching/ws01_02/proseminarliteratur/deepwebwhitepaper.pdf (BrightPlanet) · dl.acm.org/doi/fullHtml/10.1145/1314215.1314222 (ARGs)

**Tor Project/standards:** torproject.org/about/history · blog.torproject.org/statement-tor-project-software-integrity-and-apple · blog.torproject.org/introducing-webtunnel-evading-censorship-by-hiding-in-plain-sight · community.torproject.org/relay/community-resources/eff-tor-legal-faq · rfc-editor.org/rfc/rfc9116 · developer.mozilla.org/en-US/docs/Web/Security/Practical_implementation_guides/Robots_txt

**Journalism:** wired.com (Hansa 2018; CMU 2015; Onymous 2014; DisrupTor 2020; Welcome to Video 2019/2022; Silk Road $4.4B 2024; AlphaBay series 2022; Freedom Hosting 2013; Dark Web myth 2015) · bbc.com (Silk Road 2013; Onymous 2014; Marques 2021) · theguardian.com (Onymous 2014; Individual X 2020; Marques 2021) · cnn.com (Ulbricht 2013; Kim 2013; Individual X 2020; Welcome to Video 2019) · vice.com (CMU 2016; red rooms 2024) · arstechnica.com (Freedom Hosting 2013) · krebsonsecurity.com (Freedom Hosting tag) · techradar.com (Recorded Future onion crawl 2019) · engadget.com (Mariana's Web 2015) · kotaku.com (Sad Satan) · fastcompany.com (Notpron) · atlasobscura.com (Konami) · mixmag.net (spectrogram art) · aphextwin.nu · wired.com/story/operation-onymous

**Industry reports:** chainalysis.com/blog/crypto-drug-sales-darknet-markets-2026 · chainalysis.com/blog/darknet-markets-2025 · chainalysis.com/blog/landscape-of-seizable-crypto-assets-2025 · chainalysis.com/blog (Individual X 2020) · cybernews.com/security/telegram-channels-takedown-criminal-activity · thehackernews.com/expert-insights/2026/03/telegrams-crackdown-changed-how-threat · committee.iso.org (dark web explainer) · congress.gov/crs-product/IF12172

**Cicada/ARG:** github.com/cicada-solvers/The-Complete-Cicada3301-Archive · github.com/scream314/cicada3301 · clevcode.org/cicada-3301 · connortumbleson.com (2014 solve) · dl.acm.org (ARG design) · en.wikipedia.org/wiki/Notpron · en.wikipedia.org/wiki/I_Love_Bees · if50.substack.com/p/2001-the-beast · 42entertainment.com/work/ilovebees


