# The Origin of Matter v401 - Full Reconstruction Specification

## Milestone
- Version: **v401**
- Title: **mPOS, UPRam, mitoCPR, DELE1-HRI and Import-Stress Signaling Atlas**
- Standalone pages: **5**
- PDF filename: `The_Origin_of_Matter_mPOS_UPRam_mitoCPR_DELE1_HRI_Import_Stress_Atlas_v401.pdf`
- PDF SHA-256: `363ef0a7bb9f450702c88060bbba632301763d200586a04ea29b1edf43e09a58`
- Render verification: **5/5 pages at 200 DPI**
- Preflight: **passed**

## Scientific bridge from v400
v400 established intramitochondrial import throttling through mtHsp70/PAM redistribution and OMA1-DNAJC15 proteolysis. v401 follows the reduced import flux outward into cytosolic precursor accumulation, mitochondrial-surface surveillance, proteasomal disposal, and mammalian DELE1-HRI integrated stress signaling.

## Rendered Equation Index
1. `dP_cyt/dt = J_syn,mito - J_import - J_extract - k_deg P_cyt`
2. `Phi_import = J_syn,mito / (J_import + J_extract + k_deg P_cyt + epsilon)`
3. `d[Cis1]/dt = alpha_C S_import - k_C[Cis1] ; J_extract = k_Msp1[Cis1]P_stall`
4. `dD_cyt/dt = k_OMA1 A_OMA1 D_transit + k_arrest D_surface - k_clear D_cyt`
5. `A_HRI = D_cyt^n / (K_D^n + D_cyt^n)`
6. `dp_eIF2a/dt = k_HRI A_HRI(1-p_eIF2a) - k_deP p_eIF2a`
7. `J_translation = J0 T(p_eIF2a), with dT/dp_eIF2a < 0 for bulk translation`
8. `X_importStress = {P_cyt,P_stall,J_import,J_extract,DELE1,HRI,p-eIF2a,ATF4,proteasome,translation,recovery/death}`

## Six-Level Scientific Architecture
1. Precursor flux state.
2. Cytosolic precursor-proteostasis state.
3. Mitochondrial-surface stalled-import state.
4. Stress-relay state.
5. Integrated translation/transcription response.
6. Provenance-aware recovery-versus-death state.

## Evidence Firewall
- Do not equate yeast mitoCPR with mammalian DELE1-HRI.
- Do not claim all DELE1 signaling requires OMA1 cleavage.
- Do not equate OMA1-DNAJC15 with OMA1-DELE1 substrate pathways.
- Do not assume precursor overload requires permanent translocase damage.
- Do not label ATF4/CHOP signaling universally protective or apoptotic.

## Primary Sources
1. Wang & Chen, Nature 2015, DOI 10.1038/nature14859.
2. Wrobel et al., Nature 2015, DOI 10.1038/nature14951.
3. Weidberg & Amon, Science 2018, DOI 10.1126/science.aan4146.
4. Guo et al., Nature 2020, DOI 10.1038/s41586-020-2078-2.
5. Fessler et al., Nature 2020, DOI 10.1038/s41586-020-2076-4.
6. Fessler, Krumwiede & Jae, Nature Communications 2022, DOI 10.1038/s41467-022-29479-y.
7. Molecular Cell 2023, mitochondrial iron-responsive pathway regulated by DELE1.

## Next Frontier
Construct a quantitative precursor-load phase diagram linking v400 import throttling to v401 precursor accumulation, DELE1-HRI activation, translational attenuation, recovery, and cell death.
