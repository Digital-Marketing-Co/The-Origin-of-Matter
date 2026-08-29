# The Origin of Matter v400 - Full Reconstruction Specification

This UTF-8 archival file preserves the complete searchable text extracted from the verified v400 PDF plus the rendered equation strings that are graphical in the PDF. It is intended to make the milestone scientifically reconstructible even if the binary PDF becomes unavailable.

## Rendered Equation Index

1. `J_import = k_cap H_free,TIM23 P_precursor ; H_tot = H_TIM23 + H_matrix + H_bound`
2. `f_bound = H_bound / H_tot ; reserve = 1 - f_bound`
3. `dH_TIM23/dt = k_on H_free T - k_off H_TIM23 - k_comp U H_TIM23`
4. `Control = F(U, H_TIM23, J_import, recovery, mitophagy)`
5. `d[D15]/dt = S_D15 - k_OMA1 A_OMA1[D15] - k_base[D15]`
6. `J_OXPHOS,bio = J0 g(DNAJC15, Delta psi, TIM23, precursor supply, stress)`
7. `dP_ER/dt = J_fail - k_clear P_ER ; UPR_ER = Phi(P_ER)`
8. `X_QC = {U_matrix, HSPA9 allocation, DNAJC15, OMA1, AFG3L2, J_import, J_OXPHOS,bio, ER stress, mitophagy, U}`

## Extracted Publication Text

### 1. mtHsp70 Is Both an Import Motor and a Matrix Proteostasis Chaperone
Matrix-destined precursors imported through TIM23 require the presequence translocase-associated motor (PAM). The central ATPase is mitochondrial Hsp70 (mtHsp70/HSPA9 in mammals; Ssc1 in yeast), which binds polypeptide segments as they emerge into the matrix. The same chaperone also folds newly imported proteins and suppresses aggregation. This dual allocation means protein import and matrix proteostasis compete for a finite chaperone pool. [1,3]

Variables: Jimport = productive matrix-import flux; Hfree,TIM23 = import-available mtHsp70; Htot = total mtHsp70 pool; Pprecursor = import-competent substrate concentration.

### 2. Single-Molecule Measurements Show mtHsp70 Operates Near Capacity
A 2026 PNAS study used single-molecule fluorescence methods in physiologically active mitochondria and found that the majority of mtHsp70 molecules were substrate bound. The result implies that the chaperone network normally operates with limited spare capacity rather than as a vast idle reserve. This makes mtHsp70 an intrinsic sensor of matrix protein-folding load. [1]

Variables: fbound = substrate-bound fraction; reserve = simplified spare capacity. Scope: the measured occupancy constrains physiology but is not a universal tissue-independent constant.

### 3. Matrix Unfolded Proteins Redistribute mtHsp70 Away from TIM23
When unfolded proteins were experimentally increased in the mitochondrial matrix, mtHsp70 association with TIM23 decreased and mtHsp70-dependent import was selectively impaired. This creates a direct mechanistic bridge from intramitochondrial proteostasis stress to reduced influx of new proteins: stressed mitochondria throttle the very pathway that would otherwise increase matrix folding burden. [1]

Variables: HTIM23 = translocase-associated mtHsp70; T = available TIM23 motor sites; U = unfolded-protein load; kcomp = stress-driven competition/redistribution term.

### 4. Import Throttling Is a Quality-Control Signal, Not Merely Mechanical Failure
The 2026 work interprets mtHsp70 redistribution as a mitochondrial quality-control sensor. Unfolded proteins do not simply jam TIM23; they alter allocation of the chaperone required to drive translocation. Reduced import can then help initiate cellular programs that rescue stressed mitochondria or promote their removal. The pathway is therefore modeled as regulated load shedding rather than passive collapse. [1]

### 5. OMA1 Adds a Proteolytic Import-Throttling Pathway Through DNAJC15
A February 27, 2026 Nature Structural & Molecular Biology study identified a second stress-adaptive mechanism. The inner-membrane stress protease OMA1 cleaves DNAJC15, a J-domain cochaperone associated with the TIM23 import motor, and this cleavage promotes DNAJC15 degradation by the m-AAA protease AFG3L2. Loss of DNAJC15 decreases mitochondrial protein import during dysfunction. [2]

Variables: D15 = DNAJC15 abundance; AOMA1 = activated OMA1; kOMA1 = stress cleavage rate; kbase = basal turnover.

### 6. DNAJC15 Loss Selectively Restricts OXPHOS Biogenesis During Stress
OMA1-dependent depletion of DNAJC15 impairs import and reduces OXPHOS-related protein accumulation under mitochondrial dysfunction. This is a protective resource-allocation strategy: when membrane/respiratory state is compromised, the organelle transiently limits construction of expensive oxidative-phosphorylation machinery until conditions improve or the mitochondrion is removed. [2]

### 7. Non-imported Precursors Couple Mitochondrial Stress to the Endoplasmic Reticulum
The DNAJC15 study further found that mitochondrial precursors failing to enter stressed mitochondria accumulate at the endoplasmic reticulum and induce an unfolded-protein response. Mitochondrial import stress is therefore not contained within one organelle: precursor rerouting creates cross-organelle proteostasis signaling. [2]

### 8. Stress-Adaptive Import Regulation Closes the Proteome-Energy-Quality Loop
v398 and v399 established carrier and presequence import as energy-dependent construction pathways. v400 adds quality-control feedback: proteostasis stress redistributes mtHsp70, while OMA1 proteolytically removes DNAJC15 to reduce import and OXPHOS biogenesis. The mitochondrion therefore controls not only what it imports, but when it should temporarily stop importing at full capacity.

## Six-Level Scientific Architecture
1. Precursor/chaperone molecular state - mtHsp70 ATPase/substrate-binding states and precursor segments define immediate import/folding chemistry.
2. Import-motor allocation state - mtHsp70, DNAJC15/DNAJC19, TIMM44 and PAM components set motor capacity at TIM23.
3. Matrix proteostasis state - unfolded-protein load competes for chaperones and changes import availability.
4. Proteolytic stress-control state - OMA1 and AFG3L2 remodel import capacity by regulating DNAJC15 abundance.
5. Organelle biogenesis/quality state - OXPHOS assembly, ER precursor stress, recovery and mitophagy emerge from regulated import flux.
6. Provenance-aware cellular state - species, stressor, tissue, assay and temporal stage remain explicit.

## Twenty-Four-Level Proteostasis-to-Quality-Control Hierarchy
1. cytosolic precursor synthesis
2. TOM entry
3. TIM23 engagement
4. presequence translocation
5. Tim17 cavity passage
6. PAM recruitment
7. mtHsp70 ATP binding
8. precursor capture
9. ATP hydrolysis
10. mtHsp70 substrate lock
11. matrix release/folding
12. matrix unfolded-protein load
13. chaperone-pool redistribution
14. reduced TIM23-associated mtHsp70
15. lower matrix-import flux
16. OMA1 stress activation
17. DNAJC15 cleavage
18. AFG3L2-dependent turnover
19. restricted OXPHOS import
20. reduced OXPHOS biogenesis
21. non-imported precursor rerouting
22. ER unfolded-protein response
23. recovery-versus-mitophagy decision
24. provenance-aware mitochondrial quality state

## Evidence Firewall
- Reject: mtHsp70 serves only as a protein-import motor. 2026 single-molecule work shows a large matrix substrate-bound pool involved in folding/proteostasis.
- Reject: proteostasis stress impairs import only because precursors physically clog TIM23. Unfolded proteins redistribute mtHsp70 away from TIM23 and selectively reduce mtHsp70-dependent import.
- Reject: the mtHsp70 network contains an unlimited inactive reserve. The majority of measured molecules were substrate bound in the 2026 study.
- Reject: OMA1 affects mitochondrial morphology but not protein import. 2026 work shows OMA1 cleavage of DNAJC15 decreases import and OXPHOS biogenesis under stress.
- Reject: DNAJC15 loss globally abolishes all mitochondrial import. The pathway acts as stress-adaptive throttling; basal import remains and substrate classes differ.
- Reject: failed mitochondrial import is entirely cell-autonomous within mitochondria. Non-imported precursors accumulate at the ER and induce an ER unfolded-protein response.
- Reject: reduced OXPHOS biogenesis under stress is necessarily pathological rather than adaptive. The data support regulated stress adaptation, although prolonged suppression may become detrimental.

## Cross-reference
v398 resolved TOM-TIM22 carrier insertion and v399 resolved TIM23 topogenic recognition. v400 adds the PAM/mtHsp70 motor-allocation layer and a stress-responsive OMA1-DNAJC15 proteolytic brake on import and OXPHOS biogenesis.

## Primary Sources
1. Banerjee R, Trauschke V, Bertram N, et al. *mtHsp70 chaperone converts mitochondrial proteostasis stress into impaired protein import.* PNAS. 2026;123(15):e2526136123. DOI: 10.1073/pnas.2526136123.
2. Kroczek L, Nolte H, Lasarzewski Y, et al. *Stress adaptation of mitochondrial protein import by OMA1-mediated degradation of DNAJC15.* Nature Structural & Molecular Biology. Published 27 February 2026. DOI: 10.1038/s41594-026-01756-0.
3. Schulz C, et al. *The mitochondrial Hsp70 controls the assembly of the F1FO-ATP synthase.* Nature Communications. 2022;13:7792. DOI: 10.1038/s41467-022-35720-5.
4. Sim et al. Nature 621 (2023) 620-626 - Tim17 translocation cavity and TIM23 architecture.
5. Chen et al. Nature Chemical Biology, published 26 August 2026. DOI: 10.1038/s41589-026-02304-z - topogenic recognition at Tim17/Tim22 cavities.

## Next Frontier
Measure absolute mtHsp70 occupancy and exchange rates in mammalian tissues; determine how matrix misfolding changes DNAJC15/DNAJC19 recruitment kinetics; resolve stressed human TIM23-PAM complexes structurally; quantify the threshold at which adaptive import throttling becomes irreversible bioenergetic failure; and incorporate precursor synthesis, import, folding, degradation and organelle turnover into one proteome-flux model.
