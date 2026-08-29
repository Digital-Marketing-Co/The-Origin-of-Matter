# v386-v390 Reconstruction Specifications

Each milestone was generated as a 12-page standalone addition with mechanistic sections, equation/variable plates, deeper hierarchy, evidence firewall, primary-source synthesis, original scientific illustrations, and render/preflight QA.

---

## v386 — Complex I Quinol Post-Catalysis and Histidine Gating Atlas

Reported total after integration: 3,019 pages. SHA-256: `287c61959013e37a4e401553401758d25cba5c83b57774666fad41451de73c6d`.

### Core scientific sequence

1. Post-catalysis mammalian Complex I captures reduced ubiquinol in the active channel. June 12, 2026 cryo-EM structures in phospholipid nanodiscs with Q10 reported approximately 2.0-2.6 A global resolution and two reduced Q10H2 conformations. Reaction: `NADH + Q10 + H+ -> NAD+ + Q10H2`.
2. Reduced Q10H2 occupies more than one product-side conformation. Pose occupancy model: `P(q_i|red)=exp(-G_i/RT)/sum_j exp(-G_j/RT)`.
3. Highly hydrated structures reveal near-continuous proton connections; connectivity is distinguished from flux. `Gamma_PT = product_i p_i^HB`.
4. Histidine junctions provide a candidate directionality mechanism. Provisional ND5 H248 and ND4 H220 gating assignments from an August 2026 bioRxiv preprint are stored as states `S_H in {U,L,O}` for uptake-, lateral-, and output-connected geometry.
5. Conformational gating can impose direction without a macroscopic valve. `J_H+ = sum_s P(s) k_s Delta mu_s`.
6. Histidine-switch energetics have an independent 2026 peer-reviewed computational foundation. `Delta G_switch = G_state2 - G_state1`.
7. Product chemistry and proton gating must be joined in a time-ordered cycle: `Q -> QH2 -> H_inj+ -> G_mem -> 4H_pump+`.
8. Complex I is a dynamic redox-hydration-conformation machine. `X_CI(t)={Q(t),W(t),pKa(t),R(t),H(t),psi(t),J_e(t),J_H(t),U}`.

### Six-level architecture
quinone chemical state -> hydration/protonation microstate -> carboxylate and histidine gating -> antiporter-like subunit coupling -> PMF production -> provenance-aware catalytic ensemble.

### 22-level hierarchy
NADH hydride equivalent -> FMN/FeS relay -> oxidized Q10 -> Q-channel entry pose -> reactive quinone pose -> Q10H2 product pose A -> product pose B -> local protonation -> internal water -> H-bond wire -> D79/NuoA kinetic gate -> ND1/ND3/ND4L lateral pathway -> antiporter-like module -> ND4 H220 junction -> ND5 H248 junction -> helix rearrangement -> proton-uptake connection -> lateral connection -> proton-output connection -> four-proton pumping cycle -> PMF -> provenance-aware dynamic Complex-I ensemble.

### Primary anchors
Chung et al., Nature Communications (12 Jun 2026); Fisher et al., bioRxiv (13 Aug 2026), DOI `10.64898/2026.08.12.744383`; Endres et al., Protein Science 35(8) (Aug 2026) e70720; Beghiah et al., Nature Communications (1 Jul 2026); Choi & Voth, JACS 148 (2026) 13954-13963; Badolato et al., JACS (8 May 2026), DOI `10.1021/jacs.6c05956`.

---

## v387 — Complex II Loss, Respiratory-Chain Remodeling and Cristae Ultrastructure Atlas

Reported total: 3,031 pages. SHA-256: `9fef9ac8d7b1661e977b87708b7fb6d442513498ed43a2fb798c207d230c380e`.

### Core scientific sequence

1. Complex II is both a TCA-cycle enzyme and respiratory-chain entry point. `succinate + Q -> fumarate + QH2`; no direct proton pumping by CII.
2. SDHA and SDHB deficiency create distinct assembly contexts but a shared loss of CII activity. `A_CII=k_cat[CII_active]`; SDHB deficiency can permit an inactive CII-low assembly intermediate containing flavinated SDHA.
3. Complex-II loss propagates beyond its own enzyme. Network response: `Delta R_ETC = J_matrix Delta x_CII`.
4. Complex I is a major secondary target of CII deficiency. `CI_obs=f(Q_redox,SC,L,P,Delta p,U)`.
5. Respiratory loss produces measurable ATP-production deficit. `J_ATP <= J_H+,pump / n_H+/ATP`.
6. Complex-II deficiency reaches the ultrastructural level with reduced crista density. `rho_crista=A_crista/V_mito` as an idealized metric.
7. CII-low is an assembly marker, not a functional substitute. `F_rescue=A_intermediate/A_holo`.
8. Respiratory architecture is a coupled network rather than five independent machines. `N_IMM={CI,CII,CIII,CIV,CV,Q,cytc,L,G,Delta p,U}`.

### Six-level architecture
Complex-II molecular state -> assembly-state competence -> respiratory-network remodeling -> bioenergetic output -> crista ultrastructure -> provenance-aware systems energetics.

### 22-level hierarchy
succinate -> SDHA active site -> FAD -> SDHB FeS relay -> SDHC/SDHD membrane module -> Q-binding site -> QH2 reduction -> active holo-CII -> CII-low -> Q-pool redox state -> respiratory cross-talk -> Complex-I abundance/assembly -> supercomplex organization -> oxygen-consumption capacity -> respiratory proton pumping -> PMF -> ATP-synthase driving force -> ATP production -> inner-membrane material state -> crista density -> mitochondrial ultrastructure -> provenance-aware respiratory-network phenotype.

### Primary anchors
Esteban-Amo et al., Scientific Reports (27 Aug 2026), DOI `10.1038/s41598-026-68904-w`; Beghiah et al., Nature Communications 17 (1 Jul 2026) 5737; Choi & Voth, JACS 148 (2026) 13954-13963; Fisher et al., bioRxiv (13 Aug 2026); Nguyen et al., Nature Communications 17 (2026) 1550; Brown et al., Science Advances 12 (28 Aug 2026) eaee8657.

---

## v388 — Complex IV Oxygen Reduction, Proton Pumping and Cytochrome-c Diffusion Atlas

Reported total: 3,043 pages. SHA-256: `7ccb99153983cb87817ac2cd1c42cebf144eb884d3856cc246ad78770bca9074`.

### Core scientific sequence

1. Complex IV terminates the respiratory electron-transfer chain. Idealized full O2 reaction: `O2 + 4e- + 8H_N+ -> 2H2O + 4H_P+`.
2. Electron transfer proceeds through cytochrome c -> CuA -> heme a -> heme a3/CuB.
3. Catalytic protons and pumped protons are functionally distinct. `N_H+,in=N_chem+N_pump`.
4. D, K and H pathways encode competing/complementary mechanistic models. Pathway-state set: `{D,K,H;M,U}`.
5. H-pathway model contains gate, water cluster and proton-loading region. Leak proxy: `P_leak ~ P(open|cycle) P(path connected)`.
6. Cytochrome-c transfer between III and IV is context dependent. Saturating carrier relation: `J=J_max[cyt c]/(K_1/2+[cyt c])`.
7. Membrane embedding changes the meaning of diffusion limitation. Turnover time: `tau_cycle=tau_diff+tau_bind+tau_ET+tau_cat`.
8. Complex IV closes the electron-proton-oxygen conservation loop. `B_resp={J_e,J_O2,J_H,chem,J_H,pump,J_H2O,Delta p,U}`.

### Six-level architecture
redox-cofactor state -> proton-pathway state -> catalytic-cycle coupling -> carrier-transfer kinetics -> PMF contribution -> provenance-aware terminal respiration.

### 22-level hierarchy
reduced cytochrome c -> productive docking -> CuA reduction -> heme-a reduction -> binuclear-center state -> oxygen binding -> O-O chemistry -> chemical-proton uptake -> water formation -> D state -> K state -> H state -> water-channel gate -> proton-storage cluster -> proton-loading site -> P-side release -> pumped-proton output -> membrane-potential contribution -> Delta-pH contribution -> PMF -> ATP-synthase coupling -> provenance-aware terminal respiratory state.

### Primary anchors
Shimada, Tsukihara & Yoshikawa, Frontiers in Chemistry (30 Jan 2026), DOI `10.3389/fchem.2025.1645343`; Lobez, Oliveberg & Brzezinski, FEBS Letters (16 Jun 2026), DOI `10.1002/1873-3468.70382`; Baserga et al., ChemPhysChem 26 (2025) e202500539; Nguyen et al., Nature Communications 17 (10 Jan 2026) 1550; Nakano et al., Nature Communications 17 (2026) 4075; Padavannil, Liu & Letts, JoVE (21 Aug 2026), DOI `10.3791/72243`.

---

## v389 — Respiratory Chain Stoichiometry, Proton-Motive Force and ATP Yield Atlas

Reported total: 3,055 pages. SHA-256: `acdb716d25420d102c46c36448fc4b6ceffb2b739effb1c7e142db1591724413`.

### Core scientific sequence

1. Respiratory stoichiometry is a conservation problem, not a single magic number. Idealized NADH-linked bookkeeping: `n_H(NADH) ~ n_I+n_III+n_IV ~ 4+4+2=10`.
2. Succinate-linked electrons enter downstream of CI. `n_H(succinate) ~ n_III+n_IV ~ 4+2=6`.
3. PMF has electrical and chemical components. `Delta p=Delta psi-(2.303RT/F)Delta pH`.
4. ATP-synthase stoichiometry depends on rotor architecture. `H+/ATP(rotor)=n_c/3`; mammalian c8 gives idealized 8/3 before overhead.
5. Cellular ATP cost includes more than the rotary motor. `g_eff=g_rotor+g_transport+g_leak`.
6. P/O is an emergent ratio. `P/O=J_ATP/(2J_O2)` under the specified normalization.
7. Free-energy sufficiency must be checked. `Delta G_H=F Delta p; n Delta G_H >= Delta G_ATP,eff`.
8. Complete OXPHOS ledger: `{J_e,J_H,pump,Delta p,g_eff,J_ATP,J_O2,U}`.

### Six-level architecture
electron-entry state -> complex-specific proton pumping -> electrochemical storage -> rotary conversion -> transport-adjusted ATP output -> provenance-aware P/O.

### 20-level hierarchy
reducing equivalent -> CI/CII entry -> Q pool -> CIII -> cytochrome c -> CIV -> oxygen reduction -> chemical-proton consumption -> respiratory proton pumping -> membrane voltage -> Delta-pH -> PMF -> Fo proton binding -> c-ring rotation -> gamma-shaft torque -> F1 state cycling -> matrix ATP -> phosphate/ADP-ATP transport -> effective P/O -> provenance-aware cellular ATP yield.

### Primary foundations
Mitchell, Nature 191 (1961) 144-148; Hinkle, BBA 1706 (2005) 1-11; Watt et al., PNAS 107 (2010) 16823-16827; Gu et al., Nature 537 (2016) 639-643; Beghiah et al., Nature Communications 17 (2026) 5737; Esteban-Amo et al., Scientific Reports (27 Aug 2026).

---

## v390 — Complex III Q Cycle, Electron Bifurcation and Cytochrome-c Reduction Atlas

Reported total: 3,067 pages. SHA-256: `3acf131bbef9b0ce2db68346a331c0b65919ba067364ef12217379340fff6eb6`.

### Core scientific sequence

1. Complex III couples quinol oxidation to cytochrome-c reduction. Net idealized Q-cycle relation: `QH2 + 2 cyt c(ox) + 2 H_N+ -> Q + 2 cyt c(red) + 4 H_P+`.
2. Electron bifurcation separates high- and low-potential branches: `e1: QH2 -> Rieske -> c1 -> cyt c`; `e2: QH2 -> bL -> bH -> Qi`.
3. Two Qo turnovers complete the canonical Q cycle. `2 QH2(Qo)+Q(Qi)+2H_N+ -> 2Q(Qo)+QH2(Qi)+4H_P+`.
4. Semiquinone is a necessary intermediate and potential hazard. `Q+e- <-> Q.- ; Q.-+e-+2H+ -> QH2`.
5. Rieske-domain motion couples chemistry to ET. Ensemble representation: `P_ET=sum_s P(s) k_ET(s) dt`.
6. Complex III contributes approximately four proton equivalents per two cytochrome-c reductions. `n_H,CIII/2e- ~ 4`.
7. Q-cycle control limits wasteful short circuits. `J_e,total=J_productive+J_short+J_ROS`.
8. Integrated CIII state: `{Qo,Qi,Rieske,c1,bL,bH,Q.-,cytc,H+,U}`.

### Six-level architecture
Qo chemical state -> branch-specific electron state -> Qi quinone state -> cytochrome-c output -> vectorial proton contribution -> provenance-aware Q-cycle ensemble.

### 22-level hierarchy
QH2 membrane pool -> Qo binding -> first proton release -> first bifurcation -> Rieske reduction -> Rieske movement -> c1 reduction -> cytochrome-c reduction -> bL -> bH -> Qi quinone -> Qi semiquinone -> second Qo turnover -> second high-potential electron -> second cytochrome-c reduction -> second low-potential electron -> Qi QH2 formation -> N-side proton uptake -> P-side proton appearance -> PMF contribution -> CIV electron delivery -> provenance-aware respiratory-network state.

### Primary foundations
Mitchell, J. Theor. Biol. 62 (1976) 327-367; Crofts et al., BBA 1827 (2013) 1362-1377; Xia et al., Science 277 (1997) 60-66; Iwata et al., Science 281 (1998) 64-71; Lobez, Oliveberg & Brzezinski, FEBS Letters (16 Jun 2026); Esteban-Amo et al., Scientific Reports (27 Aug 2026).
