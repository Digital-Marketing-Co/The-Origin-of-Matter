# v396-v398 Reconstruction Specifications

These specifications preserve enough structured text, equations, hierarchy, evidence-firewall logic, and source anchors to regenerate the late lipid/biogenesis milestones whose temporary PDF delivery links may no longer be available.

---

# v396 — Cardiolipin Remodeling, Tafazzin, Respirasome and Membrane Bioenergetics Atlas

Reported standalone milestone: 12 pages. Reported reconstructible total: 3,139 pages. Reported SHA-256: `1aec9c4bf5b88eb29f604673f662f1383b3ca87bfc83f43ccca1957aad170eff`.

## Core sections

1. **Cardiolipin Is a Structural Lipid of the Energy-Transducing Inner Membrane.** Cardiolipin is an unusual dimeric phospholipid enriched in the inner mitochondrial membrane. Its small headgroup, four acyl chains and strong interactions with respiratory proteins make it a material component of oxidative phosphorylation rather than an inert solvent. Recent crista-junction modeling further shows preferential cardiolipin recruitment by MIC10-family proteins, directly connecting lipid chemistry to membrane curvature. State vector: `X_CL = {headgroup charge, acyl1..4, oxidation, local curvature, protein contacts}`.

2. **Tafazzin Remodels Cardiolipin Through Transacylation.** Tafazzin is a phospholipid-lysophospholipid transacylase whose loss causes Barth syndrome. It remodels acyl chains among phospholipid species rather than synthesizing cardiolipin de novo. Equation: `PL1-acyl + lyso-PL2 <-> lyso-PL1 + PL2-acyl`.

3. **Tafazzin Specificity Emerges from Membrane Context as Well as Enzyme Chemistry.** Mature cardiolipin composition is an emergent property of enzyme activity, substrate pools, membrane curvature and lipid phase behavior. Equation: `d[CL_i]/dt = sum_j k_ji[CL_j] - sum_j k_ij[CL_i] + S_i - D_i`.

4. **Cardiolipin Stabilizes Respiratory-Chain Protein Environments.** Bound phospholipids including cardiolipin can fill cavities, tune electrostatics and stabilize transmembrane contacts, but no single cardiolipin molecule is treated as a permanent glue for every respirasome. Equation: `Delta G_SC = Delta G_protein + sum_m theta_CL,m Delta g_CL,m + Delta G_membrane`.

5. **Lipid Remodeling Can Propagate from Molecules to Crista Mechanics.** Changing acyl-chain composition alters bilayer thickness, elasticity, spontaneous curvature and protein-lipid matching. Equation: `E_bilayer = integral [kappa/2(C-C0(CL))^2 + K_t/2(h-h0(CL))^2] dA`.

6. **Barth Syndrome Demonstrates the Physiological Cost of Failed Cardiolipin Remodeling.** Pathogenic TAZ variants disrupt tafazzin-dependent remodeling and produce mitochondrial dysfunction with prominent cardiac and skeletal-muscle phenotypes. Systems relation: `Phenotype_BTHS = f(TAZ, CL_species, MLCL/CL, cristae, OXPHOS, tissue, modifiers)`.

7. **Cardiolipin State Can Influence Both Electron and Proton Geography.** Respiratory complexes, ATP synthase and MICOS occupy different crista microdomains but interact with the same bilayer. Relation: `J_ATP(x) = F[SC(x,CL), H_s(x,CL), ATPase(x,CL), topology(CL)]`.

8. **A Lipid-Aware Digital Crista Completes the Current Inner-Membrane Framework.** State vector: `X_IMM(t) = {CL_i(x), TAZ, curvature(x), strain(x), SC(x), MICOS(x), ATPase(x), H+(x), e-(x), U}`.

### Six-level architecture
1. Cardiolipin molecular species.
2. Tafazzin remodeling network.
3. Membrane material state.
4. Protein-assembly state.
5. Crista bioenergetic state.
6. Provenance-aware tissue/disease state.

### 24-level lipid-to-bioenergetics hierarchy
fatty-acyl chain -> phospholipid donor -> lysophospholipid acceptor -> tafazzin active site -> transacylation event -> cardiolipin molecular species -> MLCL/CL balance -> local lipid packing -> bilayer thickness -> spontaneous curvature -> cardiolipin-protein binding site -> respiratory-complex interface -> supercomplex free-energy landscape -> MIC10 cardiolipin recruitment -> crista-junction curvature -> ATP-synthase lipid environment -> crista-tip architecture -> membrane strain field -> electron-carrier geography -> surface proton geography -> local ATP-production field -> whole-organelle OXPHOS -> tissue energetic phenotype -> provenance-aware cardiolipin state.

### Evidence firewall
Tafazzin is not described as the de novo cardiolipin synthase; one fixed cardiolipin species is not declared universally required; a bound cardiolipin is not interpreted as permanent supercomplex glue; MLCL/CL alone does not completely predict Barth-syndrome severity; cardiolipin effects on localized proton mobility are not claimed quantitatively known in intact mammalian cristae; membrane mechanics is not modeled independently of lipid composition; oxidation is not conflated with remodeling.

### Primary anchors
Brown et al., Science Advances 12 (2026) eaee8657; Xu et al., Nature Chemical Biology 2 (2006) 154-159, DOI `10.1038/nchembio771`; Schlame et al., JBC 287 (2012) 29425-29434; Letts, Fiedorczuk & Sazanov, Nature 537 (2016) 644-648; Pöverlein et al., eLife 13 (2026) e102104; Flegel et al., PNAS 123 (2026) e2510444123.

---

# v397 — Cardiolipin Synthesis, Saturation, Mitoregulin and Cardiac Maturation Atlas

Reported standalone milestone: 12 pages. Reported reconstructible total: 3,151 pages. Reported SHA-256: `9c5a176c33a6c200676b73a43763e63d6e554c58876ec31eb074af8562431a5b`.

## Core sections

1. **De Novo Cardiolipin Synthesis Is a Developmental Control Point.** A July 7, 2026 EMBO Reports study separated de novo cardiolipin synthesis from later acyl remodeling during postnatal mouse-heart maturation. Cardiomyocyte-restricted Crls1 deletion prevented the normal postnatal increase in cardiolipin concentration and blocked the rise in crista density and intramitochondrial respiratory-protein concentration. Equation: `d[CL]/dt = J_CRLS1 - J_turnover - J_export`.

2. **Cardiolipin Abundance and Acyl Remodeling Are Distinct Biological Variables.** State vector: `X_CL = {[CL]_total, p_1...p_n, MLCL/CL, oxidation}`.

3. **Respiratory-Chain Biogenesis Depends on the Lipid Scaffold.** Crls1-deficient neonatal cardiomyocytes fail to show the normal developmental increase in respiratory proteins. Equation: `dR_ETC/dt = k_bio f(CL,cristae) - k_deg R_ETC`.

4. **Saturated Cardiolipin Can Rigidify and Flatten the Inner-Membrane Material State.** 2026 JBC work found that saturated cardiolipin species can disrupt inner-mitochondrial-membrane structure and function; saturated cardiolipin reduced inner-membrane fluidity and ordered/rigidified membranes. Relation: `K_eff = K_0 + beta f_CL,sat ; C0 = C0(f_CL,sat)`.

5. **Saturation Adds a Second Pathogenic Axis Beyond Monolysocardiolipin.** Composite bookkeeping relation: `D_CL = w_M M + w_S S + w_O O` where M = MLCL-related perturbation, S = saturation perturbation, O = oxidation perturbation.

6. **Mitoregulin Couples a Microprotein to Cardiolipin and Membrane Integrity.** January 20, 2026 Cardiovascular Research work found that mitochondria from mitoregulin-knockout mice were more susceptible to membrane freeze damage and that acute re-expression rescued vulnerability. Equation: `E_mem = E_lipid(CL) + E_Mtln-CL + E_protein + E_stress`.

7. **Mitoregulin Loss Alters Lipidomes and Worsens Ischemia-Reperfusion Injury.** Relation: `Injury_IR = F(Mtln, CL_state, membrane_integrity, ROS, Ca2+, tissue_context)`.

8. **The Inner-Membrane Model Now Has Synthesis, Remodeling, Material and Protein-Stabilization Axes.** State vector: `X_lipid(t) = {J_synth, J_remodel, f_sat, oxidation, Mtln, K_eff, C0, ETC, cristae, U}`.

### Six-level architecture
1. Precursor/synthesis state.
2. Molecular-species state.
3. Membrane-material state.
4. Protein/lipid architecture.
5. Crista/respiratory maturation state.
6. Provenance-aware tissue state.

### 24-level synthesis-to-tissue hierarchy
phosphatidic-acid precursor -> CDP-diacylglycerol pathway -> phosphatidylglycerol precursor -> CRLS1 catalytic step -> nascent cardiolipin -> tafazzin remodeling -> mature cardiolipin species -> saturated cardiolipin fraction -> oxidized cardiolipin state -> MLCL/CL state -> local membrane fluidity -> bilayer elasticity -> spontaneous curvature -> mitoregulin-cardiolipin interaction -> MICOS lipid recruitment -> respiratory-complex lipid sites -> respiratory-supercomplex organization -> ATP-synthase lipid environment -> crista density -> respiratory-protein concentration -> maximal OXPHOS capacity -> stress resistance -> cardiac tissue phenotype -> provenance-aware lipid energetic state.

### Evidence firewall
CRLS1 synthesis is not conflated with tafazzin remodeling; total cardiolipin alone does not specify membrane function; MLCL is not the only TAZ-associated dysfunction axis; saturated-cardiolipin measurements are not universalized numerically to all tissues; mitoregulin protection is not claimed exclusively cardiolipin-mediated; respiratory maturation is not treated as lipid-independent.

### Primary anchors
EMBO Reports, 7 Jul 2026, DOI `10.1038/s44319-026-00864-8`; Venkatraman et al., JBC 302 (2026) 113306, DOI `10.1016/j.jbc.2026.113306`; Stein et al., Cardiovascular Research (20 Jan 2026), DOI `10.1093/cvr/cvag011`; Brown et al., Science Advances 12 (2026) eaee8657; Pöverlein et al., eLife 13 (2026) e102104.

---

# v398 — TOM-TIM22 Carrier Import and Inner-Membrane Proteome Biogenesis Atlas

Reported standalone milestone: 12 pages. Reported reconstructible total: 3,163 pages. Reported SHA-256: `34134f086de61df9025d69d76bf94e1dbfbbb04eda629161c551b04a49b0383a`.

## Core sections

1. **Most Mitochondrial Inner-Membrane Carriers Are Nuclear Encoded.** Multi-pass carriers exchanging ADP/ATP, phosphate and other metabolites are synthesized on cytosolic ribosomes and must cross the outer membrane before inner-membrane insertion. Equation: `J_carrier = k_syn P_cyt x eta_target x eta_import`.

2. **Fresh 2026 Structures Reveal Direct Human TOM-TIM22 Coupling.** A Nature Structural & Molecular Biology article published July 23, 2026 resolved a human TOM-TIM22 supercomplex and showed direct coupling between outer-membrane TOM and inner-membrane TIM22 carrier-insertion machinery. State vector: `X_import = {TOM, precursor, small-Tim, TIM22, Delta psi, lipid bilayer}`.

3. **Carrier Transmembrane Segments Traverse TOM Along a Hydrophobic Route.** Unpaired carrier transmembrane segments traverse TOM along a hydrophobic path and exit through an unexpected lateral groove. Equation: `Delta G_path = Delta G_hydrophobic exposure + Delta G_channel + Delta G_handoff`.

4. **Small Tim Proteins Form the Protected Intermembrane-Space Handoff.** Small Tim chaperones bind carrier segments and deliver them toward TIM22. Aggregation-risk model: `P_agg = 1 - exp[-k_agg C_free tau_IMS]`.

5. **TIM22 Provides a Membrane-Exposed Groove for Lateral Carrier Insertion.** Equation: `k_insert = k0 exp[-(Delta G_lateral - zFDelta psi)/(RT)]`.

6. **Membrane Potential Couples Existing Bioenergetics to Future Membrane Biogenesis.** Equation: `dN_carrier/dt = J_import(Delta psi) - k_turn N_carrier`.

7. **Carrier Import Determines the Metabolite Boundary Conditions of OXPHOS.** Relation: `J_ATP,cell <= min(J_synthase, J_ADP/ATP, J_Pi, J_substrate)`.

8. **Import Machinery Joins Lipid, Crista and Respiratory Biogenesis in One System.** State vector: `X_biogenesis = {lipid synthesis, TOM-TIM22, carrier flux, MICOS, ETC assembly, ATPase, Delta p, U}`.

### Six-level architecture
1. Precursor state.
2. Outer-membrane translocation state.
3. Intermembrane-space handoff.
4. Inner-membrane insertion state.
5. Metabolite/OXPHOS state.
6. Provenance-aware organelle biogenesis state.

### 24-level cytosol-to-OXPHOS hierarchy
nuclear carrier gene -> mRNA export/translation -> cytosolic precursor -> mitochondrial targeting recognition -> TOM receptor engagement -> TOM channel entry -> hydrophobic TOM path -> lateral TOM exit -> small-Tim capture -> intermembrane-space protection -> TIM22 substrate-entry site -> membrane-potential sensing -> TIM22 groove -> lateral transmembrane insertion -> carrier folding -> carrier oligomer/state maturation -> ADP/ATP exchange -> phosphate transport -> matrix substrate transport -> ATP-synthase substrate supply -> respiratory metabolic coupling -> whole-organelle ATP flux -> proteostasis/turnover -> provenance-aware import state.

### Evidence firewall
Human TOM/TIM22 are not represented as obligatorily separate; carrier precursors are not portrayed as freely exposed hydrophobic soluble proteins; TIM22 is not modeled as a completely enclosed aqueous pore; human architecture is not copied unchanged to yeast; membrane potential is recognized as a protein-biogenesis input; respiratory-chain abundance alone is not treated as sufficient for cellular ATP flux; static cryo-EM does not provide all kinetic rate constants.

### Primary anchors
Liu et al., Nature Structural & Molecular Biology 33 (23 Jul 2026) 1224-1235, DOI `10.1038/s41594-026-01849-w`; Nakano et al., Nature Communications 17 (2026) 4075; Colina-Tenorio et al., Cell Reports 45 (2026) 116727; Pöverlein et al., eLife 13 (2026) e102104; Brown et al., Science Advances 12 (2026) eaee8657.
