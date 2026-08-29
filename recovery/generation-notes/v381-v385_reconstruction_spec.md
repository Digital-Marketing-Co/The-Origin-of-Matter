# v381-v385 Reconstruction Specifications

This file preserves scientific reconstruction data for milestones v381-v385. Each was generated as a 12-page standalone milestone with eight mechanistic sections, rendered equation plates plus variable/operator tables, a six-level architecture page, a deeper hierarchy page, an evidence-firewall page, and a primary-source/next-frontier page.

---

## v381 — Mitochondria-ER Iron, Calcium and Lipid Contact-Site Atlas

Reported total after integration: 2,959 pages. SHA-256: `4bd6bd01b11735f9810e0fabc5cfbf531e49a3de7d2e7f7625b332f02677bd7c`.

### Core scientific sequence

1. Mitochondria-ER contacts are nanometre-scale material-exchange interfaces rather than fusion events. Flux relation: `J_k = P_contact k_k (C_ER - C_M)`.
2. MERCs can function as an iron-supply hub. 2026 evidence: MITOL/MARCH5 K63-linked ubiquitination of HMOX2 enhances haem-degrading activity and supports mitochondrial iron homeostasis/respiration. Relation: `J_Fe = k_HMOX2 [HMOX2*] [haem]`.
3. Ubiquitination is regulatory, not necessarily destructive. State tuple: `U = (S,K,L,n,F)` for substrate, modified residue, linkage, chain state, functional consequence.
4. STIM1-containing ER-mitochondria contacts promote direct calcium transfer through interactions including PTPIP51 and GRP75. Balance relation: `d[Ca2+]_M/dt = J_ER->M - J_efflux - J_buffer`.
5. Calcium transfer couples contact geometry to respiratory capacity. `J_OXPHOS = f([Ca2+]_M, S, Delta p, ADP)`.
6. Lipid-droplet-mitochondria contacts route fatty acids into oxidation through Rab8a/PLIN5-dependent tethering. `J_LCFA = P_LD-M k_FA C_LCFA`.
7. Contact sites are multiplexed rather than single-purpose. Typed adjacency representation: `A_ij^(k,s)=w_ij^(k,s)`.
8. Contact-site biology connects matter routing to energy conversion. Integrated state: `C_M(t)={J_Fe,J_Ca,J_lipid,G_contact,E_resp,U}`.

### Six-level architecture
contact geometry -> molecular tether/regulator state -> resource conversion -> directed interorganelle flux -> respiratory/metabolic integration -> provenance-aware spatial metabolism.

### Deeper hierarchy
organelle membrane -> contact distance -> tether protein -> post-translational modification -> MERC microdomain -> haem -> HMOX2 catalytic state -> iron liberation -> mitochondrial iron pool -> STIM1 calcium-sensing state -> GRP75/PTPIP51 interface -> ER calcium release -> mitochondrial calcium uptake -> TCA/OXPHOS regulation -> lipid-droplet tether -> Rab8a/PLIN5 state -> LCFA transfer -> beta-oxidation substrate supply -> respiratory/ATP output -> provenance-aware spatial resource-allocation network.

### Primary anchors
Oshio et al., Nature Cell Biology 28 (10 Jun 2026) 1464-1479; Orantos-Aguilera et al., EMBO Journal (7 Jul 2026); Tang et al., MedComm (6 Aug 2026), DOI `10.1002/mco2.70845`; Tian et al., Cell Reports 45 (24 Mar 2026) 117112; Menendez-Montes et al., Nature 654 (10 Jun 2026) 786-797; Gladkova et al., Science 393 (6 Aug 2026) 601-606.

---

## v382 — MIC10-Cardiolipin Cristae Curvature and MICOS Assembly Atlas

Reported total: 2,971 pages. SHA-256: `765e69b879b3604ef9451b5ad3849b60b6e30c3c84a2f19bf544bd01ccf9e5aa`.

### Core scientific sequence

1. Cristae curvature has a molecular mechanism: Mic10/Mic26/Mic27 positively charged loop motifs recruit cardiolipin. `Delta G_recruit = Delta G_elec + Delta G_lipid + Delta G_conf`.
2. Cardiolipin recruitment promotes MIC10 oligomerization. `K_olig=[M_n]/[M]^n`.
3. Oligomeric MIC10 machinery stabilizes high membrane curvature. Helfrich-like relation: `E_bend = (kappa/2) integral (2H-C0)^2 dA`.
4. Crista junctions are geometric necks and molecular filters. `J_CJ=P_CJ A_CJ (C_crista-C_IMS)`.
5. MICOS assembly can precede respiratory competence in T. brucei precursor cristae. Ordering constraint: `T_MICOS < T_resp` in that lineage/context.
6. MICOS connects inner-membrane shape to outer-membrane organization; human subassembly structural evidence was treated as provisional where preprint-level.
7. Cristae geometry changes the effective physics of respiration. `J_resp=A_IMM rho_ETC k_cat f(Delta p,S)`.
8. Membrane architecture is a protein-lipid-energy state. `C(t)={P,L,O,H,P_CJ,A_IMM,R,U}`.

### Six-level architecture
amino-acid electrostatics -> lipid microdomain formation -> protein oligomerization -> membrane geometry -> organelle bioenergetic architecture -> provenance-aware evolutionary architecture.

### 20-level hierarchy
MIC10-family amino acid -> positive loop motif -> electrostatic field -> cardiolipin headgroup -> local CL enrichment -> Mic10/Mic26/Mic27 membrane association -> oligomerization -> MIC10 subcomplex -> MICOS assembly -> crista-junction domain -> spontaneous curvature -> bending rigidity -> high-curvature neck -> intrinsically disordered region -> junction permeability -> crista lumen microenvironment -> inner-membrane surface area -> respiratory-complex organization -> oxidative-phosphorylation architecture -> provenance-aware protein-lipid-energy state.

### Primary anchors
Brown et al., Science Advances 12 (28 Aug 2026) eaee8657; Boudova et al., Molecular Microbiology (7 Aug 2026); Jindal et al., bioRxiv (Aug 2026); Horten et al., Protein Science (Jun 2026), DOI `10.1002/pro.70653`; Katti et al., Aging Cell (2026), DOI `10.1111/acel.70534`.

---

## v383 — ATP Synthase Dimer Rows, Cristae Tips and Bioenergetic Architecture Atlas

Reported total: 2,983 pages. SHA-256: `0ba0c37a17d27392a5b90ceea300bd1157a584d0d5f9a8c3919e74ef2163aeb2`.

### Core scientific sequence

1. ATP synthase is both enzyme and membrane-shaping machine. `J_ATP=N_act k_cat f(Delta p,[ADP],[Pi])`.
2. Dimerization creates a curvature-generating geometric unit. `C_local ~ C_lipid + C_dimer`.
3. Dimer rows reduce energetic cost of sustaining crista ridges. `E_row=E_bend-N_d epsilon_coop`.
4. Mammalian ATP synthase can form IF1-stabilized dimers/tetramers/rows. Assembly state: `{M,D,T,R;IF1,U}`.
5. A 2026 planar mammalian dimer reveals conformational plasticity; dimerization does not uniquely specify curvature. `P(C|D)=sum_s P(C|D,s)P(s|D)`.
6. Cardiolipin chemistry tunes ATP-synthase dimer conformation. `Delta G_dimer=Delta G_protein+Delta G_CL+Delta G_elastic`.
7. Senescence disrupts ATP-synthase spatial organization in hiPSC-derived cardiomyocytes, with reduced oligomerization, increased mobility, lower mitochondrial ATP and altered calcium/contractility. Simplified organization deficit: `D_org=1-O_sen/O_ref`.
8. Crista architecture couples catalysis, geometry and diffusion. `E_crista={J_ATP,Delta p,G_MICOS,G_ATP,L,D,U}`.

### 20-level hierarchy
ATP-synthase subunit -> Fo membrane sector -> F1 catalytic sector -> rotor-stator coupling -> monomer -> dimer interface -> V-shaped dimer -> planar dimer -> IF1 conformation -> tetramer -> lateral dimer association -> extended row -> bilayer deformation -> cardiolipin interaction -> crista-rim curvature -> crista-tip topology -> proton-motive microenvironment -> ATP-production flux -> cellular energetic phenotype -> provenance-aware crista bioenergetic architecture.

### Primary anchors
Nakano et al., Nature Communications (2026), DOI `10.1038/s41467-026-70578-x`; Yokoyama et al., Cell Death & Differentiation (2026); Morris et al., Aging Cell 25 (28 Jan 2026) e70388; Blum et al., PNAS (2019); Davies et al., PNAS (2012).

---

## v384 — Respirasome Assembly, Electron Flow and Cristae Supercomplex Atlas

Reported total: 2,995 pages. SHA-256: `b917e02bdb3101b5181b5e294f0856490f3e430866649be6a131e1036af75aee`.

### Core scientific sequence

1. Respiratory complexes form higher-order supercomplexes. Canonical respirasome: `R = CI_1 + CIII_2 + CIV_1`.
2. Human respirasome biogenesis can finish while Complex IV is still maturing. Late state: `{CI*,CIII2*,CIV_pre}`.
3. HIGD2A functions as a placeholder during CIV maturation and is replaced by NDUFA4 in the final step.
4. Native mammalian membranes contain multiple respiratory-supercomplex classes. `P(SC=s)=p_s; sum_s p_s=1`.
5. Electron transfer remains chemically mediated inside a supercomplex; Q/QH2 and cytochrome c remain explicit mobile carriers. `J_e=min(J_CI->Q,J_QH2->CIII,J_cytc->CIV)`.
6. Proton pumping converts electron free energy into membrane potential. `Delta p=Delta psi-(2.303RT/F)Delta pH`.
7. Supercomplexes can support metabolic flexibility without proving obligatory channeling; yeast architecture was explicitly distinguished from mammalian CI-CIII2-CIV.
8. Cristae are an integrated MICOS-supercomplex-ATP-synthase energetic landscape. `IMM={G_MICOS,G_SC,G_ATP,Q,cytc,Delta p,L,U}`.

### 20-level hierarchy
respiratory-chain subunit -> assembly factor -> CIV precursor -> HIGD2A placeholder -> NDUFA4 incorporation -> mature CIV -> mature CI -> CIII dimer -> late respirasome intermediate -> mature respirasome -> Q pool -> QH2 transfer -> cytochrome-c pool -> oxygen reduction -> proton translocation -> membrane potential -> pH gradient -> proton-motive force -> ATP-synthase utilization -> provenance-aware crista energy-conversion network.

### Primary anchors
Nguyen et al., Nature Communications 17 (10 Jan 2026) 1550; Nakano et al., Nature Communications 17 (17 Mar 2026) 4075; Eldeeb et al., Nature Communications 17 (21 Apr 2026) 5473; Gu et al., Nature 537 (2016) 639-643; Letts et al., eLife 5 (2016) e21290.

---

## v385 — Complex I Proton Gating, Cardiolipin and Respiratory-Chain Biogenesis Atlas

Reported total: 3,007 pages. SHA-256: `c8bb4ce2c19c3557d759b641e3a302853f509e6af2931a69c9353362686fc17f`.

### Core scientific sequence

1. Complex I converts redox free energy into long-range proton pumping. Idealized turnover relation: `NADH+Q+5H_N+ -> NAD+ + QH2 + 4H_P+`.
2. A conserved carboxylate can act as a kinetic proton gate. Transition-state estimate: `k_PT ~ (kBT/h) exp(-Delta G_dagger/RT)`.
3. Hydration is an active part of proton-transfer machinery. Water-wire probability: `P_wire=P(n_w >= n_c | q,chi)`.
4. D79 mutation separates structural integrity from functional competence. Coupling ratio: `eta_PCET=J_H+/J_e`.
5. The E-channel couples quinone chemistry to antiporter-like subunits. Graph representation: `G_E=(V_acid union V_water,E_Hbond)`.
6. Cardiolipin biogenesis controls respiratory-chain maturation in the neonatal heart. `d[CL]/dt=J_synth-J_remodel-J_loss`.
7. Lipid supply, crista density and respiratory-protein abundance are coupled but distinct. `R_mito=f([CL],A_crista,rho_ETC,M,U)`.
8. Complex-I proton physics links molecular water to organ-scale energy demand. `E_CI->tissue={q,W,G_E,J_e,J_H+,Delta p,CL,G_crista,R_tissue,U}`.

### Six-level architecture
internal protonic microstate -> E-channel kinetic gating -> redox-proton coupling -> PMF generation -> lipid/crista respiratory biogenesis -> provenance-aware multiscale energetics.

### 20-level hierarchy
internal water molecule -> hydrogen-bond orientation -> protonatable carboxylate -> D79/NuoA switch point -> E-channel water wire -> TM3 conformational gate -> quinone-binding state -> quinone reduction -> long-range protonic charge propagation -> antiporter-like membrane subunit -> pumped proton -> membrane potential -> pH gradient -> proton-motive force -> ATP-synthase driving force -> cardiolipin molecule -> cardiolipin biosynthetic flux -> crista-density expansion -> respiratory-protein accumulation -> provenance-aware cardiac energy-maturation state.

### Primary anchors
Beghiah et al., Nature Communications 17 (1 Jul 2026) 5737; Choi & Voth, JACS 148 (27 Mar 2026) 13954-13963; EMBO Reports (7 Jul 2026), DOI `10.1038/s44319-026-00864-8`; Nguyen et al., Nature Communications (10 Jan 2026); Nakano et al., Nature Communications 17 (2026) 4075; Brown et al., Science Advances 12 (28 Aug 2026) eaee8657.
