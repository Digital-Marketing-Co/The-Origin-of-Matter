# v391-v395 Reconstruction Specifications

These notes preserve the scientific reconstruction layer for v391-v395 after temporary PDF-delivery failures. Each milestone was generated as a 12-page standalone addition with equation/variable plates, deep hierarchy, evidence firewall, source synthesis, illustrations, and render/preflight QA.

---

## v391 — ATP Synthase Assembly, IF1 Oligomerization and Cristae Energetics Atlas

Reported total after integration: 3,079 pages. SHA-256: `b8a8ba1de5cdd7797c2fcf6b88c7112911d42f3453a347bb2b05e51b32b31f16`.

### Core scientific sequence

1. Human ATP synthase is built as an ordered molecular construction project rather than a one-step self-assembly event. Assembly-competence relation: `A_mature = P(F1 assembled) x P(rotor assembled) x P(Fo coupled | precursors)`.
2. Catalytic-module assembly must preserve threefold F1 geometry. `N_beta=3; ATP/revolution=3`.
3. Mammalian c8 ring connects proton transfer to rotor mechanics. Ideal rotary ratio: `H+/ATP(rotor)=8/3=2.67` before transport/leak overhead.
4. IF1 is both inhibitory regulator and higher-order architectural element. State set: `{hydrolysis inhibition, dimer stabilization, oligomer bridging}`.
5. ATP-synthase oligomers help shape crista tips. Local-curvature dependence: `kappa_local=f(theta_dimer, oligomer spacing, lipid mechanics, IF1 state)`.
6. A newly resolved planar dimer expands ATP-synthase structural state space. `State_dimer in {V-shaped, planar, higher-order-associated}`.
7. IF1 conformation can reconfigure architecture without rebuilding the enzyme. `Delta G_IF1=G_kinked-G_straight`.
8. Assembly, catalysis and membrane geometry form one coupled ATP-synthase state. `X_ATPase(t)={A_F1,A_rotor,c8,IF1,theta,O,Delta p,J_ATP,U}`.

### Six-level architecture
subunit/cofactor state -> assembly-intermediate state -> mature rotary-catalytic state -> IF1 regulatory state -> dimer/tetramer/row architecture -> provenance-aware crista energetics.

### 24-level hierarchy
ATP5F1A/alpha -> ATP5F1B/beta -> alpha-beta pair -> alpha3-beta3 F1 head -> gamma central shaft -> epsilon/delta coupling -> c-subunit -> c8 rotor -> Fo proton half-channels -> peripheral stalk -> F1 assembly intermediate -> rotor assembly intermediate -> mature monomer -> IF1 binding -> reverse-hydrolysis inhibition -> canonical V-shaped dimer -> straight-IF1 planar dimer -> IF1-bridged dimer pair -> linear tetramer -> ATP-synthase row -> local crista-tip curvature -> PMF utilization -> ATP-production flux -> provenance-aware crista energetic state.

### Primary anchors
He et al., EMBO Journal 45 (2026) 5482-5513, DOI `10.1038/s44318-026-00842-9`; Nakano et al., Nature Communications 17 (2026) 4075, DOI `10.1038/s41467-026-70578-x`; Jiko et al., Cell Death & Differentiation (2026), DOI `10.1038/s41418-026-01797-4`; RCSB PDB 9VPB/EMD-65237; RCSB PDB 9VPC/EMD-65238; Watt et al., PNAS 107 (2010) 16823-16827.

---

## v392 — Mitochondrial Permeability Transition, Calcium, Swelling and ATP-Synthase Channel Atlas

Reported total: 3,091 pages. SHA-256: `ec5e7d095eb19299a487b127e82ef7ea113be1c922abcf29075185fd965038ff`.

### Core scientific sequence

1. Permeability transition is a catastrophic increase in inner-membrane conductance. PMF decay model: `Delta p(t)=Delta p0 exp[- integral g_PT(t)/C_m dt]`.
2. Calcium overload is a principal trigger but not a complete explanation. `P_open=sigmoid(a[Ca2+]m+b ROS+c Pi-d Delta psi+...)`.
3. Human genome-scale CRISPR screens identify NLRX1 as an essential activator, not necessarily the physical pore. `Phenotype_mPT=f(pore machinery,NLRX1,Ca2+,redox,membrane state)`.
4. ATP synthase and ANT remain central pore candidates. `G_PT=G_ATPase(state)+G_ANT(state)+G_other/uncertain`.
5. ATP-synthase c subunit is implicated in mitochondrial swelling. Osmotic relation: `dV_matrix/dt ~ Lp(Delta pi_osm-Delta P)` with Delta pi depending on K+ influx.
6. Potassium influx couples channel opening to organelle geometry. K+ flux treated as electrochemical and state dependent.
7. Permeability transition reverses the normal logic of OXPHOS. Energy ledger: `dE_pmf/dt=P_resp-P_ATP-P_leak-P_PT`.
8. Transition is modeled as a state ensemble: `X_mPT={G,Ca2+,ATPase_state,ANT_state,NLRX1,CypD,K+,Delta p,U}`.

### Six-level architecture
trigger state -> molecular gating state -> ion-conductance state -> bioenergetic collapse -> osmotic/structural response -> provenance-aware cell-fate state.

### 24-level hierarchy
cytosolic Ca2+ -> mitochondrial uptake -> matrix Ca2+ -> phosphate/redox context -> CypD -> NLRX1 -> ATP-synthase state -> ANT state -> candidate pore nucleation -> low-conductance event -> high-conductance transition -> ion permeability -> K+ influx -> osmotic solute accumulation -> water influx -> matrix expansion -> crista deformation -> Delta-psi collapse -> Delta-pH dissipation -> PMF collapse -> ATP-synthesis failure -> reverse-hydrolysis risk -> outer-membrane stress/cell-death signaling -> provenance-aware mPT phenotype.

### Primary anchors
Carraro, Gerle & Bernardi, Annual Review of Biophysics 55 (2026) 93-112, DOI `10.1146/annurev-biophys-030722-020832`; Valinsky et al., PNAS 123 (2026) e2535298123, DOI `10.1073/pnas.2535298123`; Jonas et al., Journal of General Physiology (12 Aug 2026), DOI `10.1085/jgp.202614066`; Pinke, Zhou & Sazanov, Nature Structural & Molecular Biology 27 (2020) 1077-1085; Nakano et al., Nature Communications 17 (2026) 4075; He et al., EMBO Journal 45 (2026) 5482-5513.

---

## v393 — MICOS, MIC10, Cardiolipin and Crista-Junction Biogenesis Atlas

Reported total: 3,103 pages. SHA-256: `b61a5a5d5b2702f95bb3e9c0f135b6ff73241ac4965f44fa1ca3576424bbf114`.

### Core scientific sequence

1. MICOS defines narrow gateways of mitochondrial cristae. Curvature relation: `kappa_CJ=1/R_CJ`.
2. Fresh August 28, 2026 work provides a molecular model for MIC10-driven curvature. `Delta G_olig=Delta G_protein+Delta G_CL-recruit+Delta G_bend`.
3. Cardiolipin recruitment couples lipid chemistry to protein architecture. `P(CL|loop) proportional exp[-Delta G_bind(CL,loop)/(RT)]`.
4. Intrinsically disordered regions may help form a crista-junction permeability barrier. `J_CJ=-D_eff A_CJ (Delta C/L_CJ)`.
5. MICOS assembly can precede respiratory competence in T. brucei. `P(MICOS assembled | respiration off)>0`.
6. MICOS is also a respiratory-complex biogenesis platform. `J_CIV,assembly=f(MICOS,MIMAS,Cox1-module,Cox3-module,import)`.
7. MIC60 and MIC10 subcomplexes divide labor across junction formation and lamellar cristae. `G_crista=G_MIC60+G_MIC10+G_OPA1+G_ATPase+G_lipid+interactions`.
8. MICOS links geometry, lipid selection, protein assembly and respiration. `X_crista={kappa_tip,kappa_CJ,MICOS,OPA1,ATPase,CL,MIMAS,ETC,U}`.

### Six-level architecture
lipid/electrostatic state -> MIC10 oligomer state -> crista-junction architecture -> organelle membrane topology -> respiratory biogenesis/function -> evolutionary/provenance state.

### 24-level hierarchy
cardiolipin molecule -> MIC10 positive loop -> local lipid enrichment -> Mic10 monomer -> Mic26/Mic27 -> MIC10 oligomer -> membrane-bending stress -> junction curvature stabilization -> IDR -> junction permeability barrier -> MIC60 subcomplex -> CJ nucleation -> OPA1 stabilization -> lamellar remodeling -> ATP-synthase tip curvature -> crista compartmentation -> inner-boundary-membrane import zone -> MIMAS -> Cox1 module -> Cox3 module -> CIV maturation -> respiratory-chain organization -> OXPHOS competence -> provenance-aware crista energetic state.

### Primary anchors
Brown, Wassenaar, Freyberg & Marrink, Science Advances 12 (28 Aug 2026) eaee8657, DOI `10.1126/sciadv.aee8657`; Boudova et al., Molecular Microbiology (7 Aug 2026), DOI `10.1111/mmi.70105`; Colina-Tenorio et al., Cell Reports 45 (27 Jan 2026) 116727, DOI `10.1016/j.celrep.2025.116727`; Stephan et al., EMBO Journal 39 (2020) e104105; Horten et al., Protein Science (Jun 2026), DOI `10.1002/pro.70653`.

---

## v394 — Localized Proton Coupling, OPA1 Crista Connectivity and Spatial OXPHOS Atlas

Reported total: 3,115 pages. SHA-256: `8ab475e7cbb35d9a549b233dc496a7e7d3a59666645f3feddaf063fc46314879`.

### Core scientific sequence

1. Membrane surface can participate directly in proton delivery. Reaction-diffusion relation: `dC_H,s/dt=D_s nabla_s^2 C_H,s-k_cons C_H,s+S_pump`.
2. Localized coupling does not abolish chemiosmosis. `Delta mu_H=F Delta psi+2.303RT Delta pH; J_local=-D_s grad_s C_H,s`.
3. Active ATP synthase can alter proton-accepting behavior of the interface. `D_s,eff=D_s,0[1+alpha A_ATPase]`.
4. Crista geometry matters for both protein packing and proton transport. `tau_surface ~ L_surface^2/(4D_s)`.
5. Aging hearts show crista remodeling before wholesale OXPHOS machinery loss. `J_OXPHOS,max=f(A_crista,connectivity,OPA1,ETC abundance,substrate)`.
6. OPA1 downregulation connects molecular remodeling to network topology. `T_crista={rho_crista,w_crista,C_connect,A_fen,OPA1}`.
7. ATP-synthase organization deteriorates in senescent cardiomyocytes. `E_cell=f(O_ATPase,M_ATPase,T_crista,Ca2+,mPT,J_ATP)`.
8. Spatial OXPHOS must join thermodynamics, surface kinetics and crista topology. `X_spatial={Delta p,C_H,s(x),D_s,pumps(x),ATPase(x),MICOS(x),OPA1,topology,U}`.

### Six-level architecture
electrochemical state -> membrane-interface proton state -> source-sink geography -> crista architecture -> organellar functional state -> provenance-aware tissue state.

### 24-level hierarchy
respiratory redox reaction -> vectorial proton pumping -> membrane-surface proton acceptance -> interfacial proton population -> lateral surface diffusion -> local pump-to-sink distance -> ATP-synthase proton capture -> Fo rotation -> F1 catalysis -> ATP production -> ATP-synthase row -> crista-tip curvature -> MICOS junction -> cardiolipin curvature -> OPA1 -> crista width -> crista density -> connectivity -> fenestration topology -> maximal OXPHOS -> calcium handling -> mPT susceptibility -> cardiomyocyte contractile phenotype -> provenance-aware tissue energetics.

### Primary anchors
Flegel, Variyam, Amdursky & Steinem, PNAS 123 (2026) e2510444123, DOI `10.1073/pnas.2510444123`; Molina-Riquelme et al., PNAS 123 (2026) e2508911123, DOI `10.1073/pnas.2508911123`; Morris et al., Aging Cell 25 (2026) e70388, DOI `10.1111/acel.70388`; Brown et al., Science Advances 12 (2026) eaee8657; He et al., EMBO Journal 45 (2026) 5482-5513.

---

## v395 — Membrane Strain, Respiratory Supercomplex Assembly and Crista Mechanics Atlas

Reported total: 3,127 pages. SHA-256: `180440c4ad448f9d89cbd7924bdedd16a427b603f2bfddd181ee36c494be363b`.

### Core scientific sequence

1. Respiratory supercomplexes can be driven partly by membrane mechanics. `Delta G_assoc=Delta G_contact+Delta G_membrane+Delta G_lipid+Delta G_entropy`.
2. Hydrophobic mismatch creates a long-range membrane interaction field. `E_mem=integral[K_t/2(h-h0)^2+kappa/2(C-C0)^2]dA`.
3. Supercomplex formation need not imply permanent substrate channeling. `J_e=J_SC+J_pool; f_SC=J_SC/(J_SC+J_pool)`.
4. Native-membrane cryo-EM confirms coexisting respiratory and ATP-synthase assemblies. `X_IMM={SC_I-III-IV,FoF1_dimer,FoF1_tetramer,lipids,curvature,IF1}`.
5. Crista mechanics is an energetic coupling layer between protein systems. `E_crista=E_bend+E_thickness+E_SC+E_ATPase+E_MICOS+E_lipid`.
6. Membrane strain can bias assembly without making it deterministic. `P(S_i) proportional exp[-G_i/(RT)] x Phi_assembly,i`.
7. Spatial organization can change carrier search times without creating a molecular wire. `tau_encounter ~ L_eff^2/(4D_eff)+tau_bind+tau_cat`.
8. Digital crista must couple mechanics to bioenergetics. `X_crista(t)={shape(x),strain(x),lipids(x),SC(x),ATPase(x),MICOS(x),H+(x),e-(x),U}`.

### Six-level architecture
protein/lipid molecular state -> membrane deformation field -> supercomplex state -> crista architectural state -> spatial bioenergetic state -> provenance-aware organelle state.

### 24-level hierarchy
transmembrane helix -> hydrophobic mismatch -> local lipid packing -> cardiolipin interaction -> bilayer thickness deformation -> local spontaneous curvature -> membrane strain field -> strain overlap -> direct protein interface -> respiratory-complex association -> supercomplex state distribution -> Q-pool geography -> cytochrome-c geography -> carrier encounter distance -> electron-transfer throughput -> respiratory proton pumping -> surface proton field -> ATP-synthase sink -> ATP-synthase dimer/tetramer -> crista-tip curvature -> MICOS junction constraint -> OPA1/topology -> spatial ATP-production field -> provenance-aware crista mechanics.

### Primary anchors
Pöverlein, Jussupow, Kim & Kaila, eLife 13 (23 Feb 2026), DOI `10.7554/eLife.102104`; Nakano et al., Nature Communications 17 (17 Mar 2026) 4075, DOI `10.1038/s41467-026-70578-x`; Brown et al., Science Advances 12 (28 Aug 2026) eaee8657; He et al., EMBO Journal 45 (2026) 5482-5513; Flegel et al., PNAS 123 (2026) e2510444123.
