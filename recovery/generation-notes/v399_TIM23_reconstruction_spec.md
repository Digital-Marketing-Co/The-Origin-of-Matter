# v399 Reconstruction Specification — TIM23 Topogenic Recognition, Stendomycin and Metabolic Import Control

Status: reconstructible text/specification preserved after temporary PDF-link failure.
Reported milestone size: 12 pages.
Reported reconstructible total after integration: 3,175 pages.
Reported PDF SHA-256: `71f59531cbee5e4c461d59cc57920e36917639137ae4f47ca7fb1b7dec4bef5d`.

## 1. TIM23 Extends the Import Atlas from Carriers to Matrix and Stop-Transfer Proteins

v398 resolved the human TOM-TIM22 carrier pathway. The complementary TIM23 pathway handles presequence-containing proteins destined for the matrix or selected inner-membrane positions. Most mitochondrial proteins originate in the cytosol; N-terminal amphipathic, positively charged targeting helices guide a major fraction through TOM and into TIM23. The pathway therefore links nuclear gene expression to construction of the matrix proteome and inner-membrane machinery.

Equation plate: `J_TIM23 = J_TOM x eta_presequence x eta_Tim17 x eta_motor`.

Variables: J_TIM23 = productive TIM23 import flux; J_TOM = outer-membrane entry flux; eta_presequence = targeting/recognition efficiency; eta_Tim17 = translocation efficiency; eta_motor = ATP-dependent completion efficiency for matrix cargo.

## 2. August 26, 2026 Structures Reveal the Shape Logic of Topogenic Recognition

A Nature Chemical Biology study published August 26, 2026 used cryo-EM and functional experiments to determine how the natural product stendomycin occupies the yeast Tim17 translocation cavity. Stendomycin adopts an alpha-helical shape that mimics topogenic sequences and plugs the same concave, lipid-exposed surface used by precursor proteins. This provides direct structural evidence that TIM recognition is partly a shape-and-surface problem rather than a simple linear sequence code.

Equation plate: `Delta G_rec = Delta G_shape + Delta G_hydrophobic + Delta G_electrostatic + Delta G_membrane`.

## 3. Tim17 Is Better Modeled as a Lipid-Exposed Translocation Cavity Than a Classical Water Pore

The 2023 TIM23 structure overturned the older picture in which Tim23 itself formed the central aqueous pore. Tim17 contains the principal protein-conducting cavity, open toward the surrounding membrane; the 2026 stendomycin structure visualizes a helical ligand occupying that cavity. The precursor is therefore modeled as moving along a protein-lipid interface whose accessibility can be dynamically regulated.

State vector: `X_Tim17 = {cavity geometry, acidic sites, lipid exposure, substrate helix, Mgr2 state}`.

## 4. Tim17 and Tim22 Share a Deep Mechanistic Core Despite Different Client Classes

The August 2026 study found that the cavities of Tim17 and Tim22 are largely interchangeable while retaining substantial function. A single Tim22 cavity mutation could confer stendomycin sensitivity, and broader cavity swaps preserved important activity. Substrate-class specificity is therefore not encoded solely by the core cavity; accessory subunits, targeting signals and pathway architecture make major contributions.

Specification relation: `Specificity = F(core cavity, accessory subunits, signal class, handoff geometry, kinetics)`.

## 5. Mgr2 Functions as a Dynamic Lateral Gate Rather Than a Permanent Wall

Stendomycin sterically conflicts with modeled Mgr2 binding, and biochemical experiments show reduced Mgr2 association after stendomycin treatment. Together with prior structural work, this supports a dynamic gate model in which Mgr2 can seal or regulate the lipid-facing Tim17 opening during translocation and sorting. For stop-transfer substrates, controlled lateral release converts a translocation intermediate into an inner-membrane protein.

Equation plate: `P_lateral = sigmoid[a(H_TM-H*) + b G_Mgr2 + c Delta psi]`.

## 6. Stendomycin Couples Import Blockade to Membrane-Potential Collapse

The 2026 work found that stendomycin not only inhibits TIM23 but also depletes mitochondrial membrane potential, likely through Tim17- or Tim22-dependent translocation across the inner membrane. This creates an experimentally useful separation between direct occupancy of the import machinery and secondary energetic failure. The encyclopedia avoids attributing every downstream phenotype solely to stalled precursor traffic.

Equation plate: `d(Delta psi)/dt = J_pump/C_m - J_leak/C_m - J_import-coupled/C_m`.

## 7. Fresh 2026 Evidence Adds Metabolic Control of TIM23 Through Succinate and Sfc1

An August 14, 2026 Cell Reports study identifies succinate and its mitochondrial carrier Sfc1 as regulators of TIM23-dependent protein import. This connects the metabolic state of the matrix and carrier-mediated metabolite exchange to the efficiency of presequence import. The import system is therefore not merely a constitutive conveyor: mitochondrial metabolism can feed back onto organelle protein biogenesis.

Equation plate: `J_import = J0 F(Delta psi, ATP, succinate, Sfc1, precursor, TIM23)`.

## 8. Protein Import Is a Closed Feedback Loop with Respiration and Metabolism

v398 established voltage-dependent carrier insertion; v399 adds TIM23 recognition, matrix import and succinate/Sfc1 metabolic regulation. Imported proteins build respiratory enzymes, metabolic pathways and import machinery; respiration creates membrane potential; metabolism generates the state variables that regulate import. The mitochondrial proteome is therefore maintained by a coupled feedback network rather than a one-way nuclear supply chain.

State vector: `X_feedback = {precursor supply, TOM, TIM23, TIM22, Delta psi, ATP, succinate, carriers, ETC, matrix enzymes, U}`.

## Six-Level Scientific Architecture

1. Topogenic-signal state — amphipathic presequences and hydrophobic sorting segments encode destination-relevant physical information.
2. Tim17 recognition state — lipid-exposed concave cavity recognizes helical topogenic features and supports translocation.
3. Gate/sorting state — Mgr2 and hydrophobic sorting signals regulate continued matrix translocation versus lateral membrane release.
4. Motor/energetic state — membrane potential and ATP-dependent PAM activity drive productive import.
5. Metabolic feedback state — succinate/Sfc1 and respiratory metabolism feed back onto TIM23-dependent biogenesis.
6. Provenance-aware proteome state — species, precursor class, inhibitor, energetic condition and structural/functional evidence remain explicit.

## Twenty-Four-Level Presequence-to-Proteome Hierarchy

1. nuclear mitochondrial gene
2. cytosolic translation
3. unfolded precursor
4. N-terminal presequence
5. TOM receptor recognition
6. Tom40 translocation
7. Tom22 trans-site handoff
8. Tim50 recognition
9. Tim23 receptor/scaffold state
10. Tim17 cavity engagement
11. alpha-helical topogenic recognition
12. Mgr2 lateral-gate state
13. membrane-potential driving
14. stop-transfer decision
15. lateral inner-membrane insertion
16. PAM motor engagement
17. mtHsp70 ATP cycle
18. matrix translocation
19. presequence cleavage
20. matrix folding/assembly
21. succinate/Sfc1 metabolic regulation
22. respiratory feedback
23. mitochondrial proteome maintenance
24. provenance-aware biogenesis state

## Evidence Firewall

- Reject: Tim23 itself is the principal aqueous protein-conducting pore. Structural evidence identifies the lipid-exposed Tim17 cavity as the main translocation path.
- Reject: TIM23 and TIM22 use completely unrelated core mechanisms. 2026 cavity-swap experiments reveal substantial functional interchangeability of Tim17/Tim22 cores.
- Reject: Core-cavity identity alone determines all substrate specificity. Accessory machinery, signal class and handoff architecture contribute strongly.
- Reject: Mgr2 is a permanently fixed wall around Tim17. Structural/biochemical evidence supports dynamic, translocation-dependent association and gating.
- Reject: Stendomycin phenotypes report only precursor-import blockade. The compound also causes membrane-potential collapse through an import-machinery-dependent mechanism.
- Reject: TIM23 import depends only on membrane potential and ATP. 2026 evidence adds succinate/Sfc1-dependent metabolic regulation.
- Reject: A yeast inhibitor structure automatically defines every human TIM23 kinetic constant. The mechanistic scaffold is informative, but species and kinetic provenance remain explicit.

## Primary-Source Synthesis

1. Chen et al., Nature Chemical Biology, published 26 Aug 2026, DOI `10.1038/s41589-026-02304-z` — stendomycin-bound Tim17 cavity; alpha-helical topogenic mimicry; Tim17/Tim22 cavity interchangeability; Mgr2 competition; membrane-potential collapse.
2. Sim et al., Nature 621 (2023) 620-626, DOI `10.1038/s41586-023-06239-6` — Tim17 lipid-exposed cavity as principal TIM23 translocation path; revised TIM23 architecture.
3. Das et al., Cell Reports 45 (14 Aug 2026) 117857, DOI `10.1016/j.celrep.2026.117857` — succinate and carrier Sfc1 mediate metabolic control of TIM23 protein import.
4. Liu et al., Nature Structural & Molecular Biology 33 (2026) 1224-1235 — direct human TOM-TIM22 carrier-import coupling; v398 cross-reference.
5. Flegel et al., PNAS 123 (2026) e2510444123 — localized proton transfer and energetic membrane state; bioenergetic cross-reference.

## Next Frontier

Solve human TIM23 with native precursor and PAM motor states; time-resolve Mgr2 opening during stop-transfer sorting; quantify succinate/Sfc1 effects on individual import steps; simultaneously measure import flux, membrane potential and ATP in intact mitochondria; integrate TIM23/TIM22 traffic with turnover to predict the complete mitochondrial proteome from nuclear precursor supply and organelle energetic state.
