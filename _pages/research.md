---
layout: archive
title: "Publications & Research"
permalink: /research/
author_profile: true
menu:
  main:
    name: "Publications & Research"
    weight: 2
---

Below is an overview of my research programme, organised around three thematic pillars. You can also explore my full publication record on [Web of Science]({{ site.author.webofscience }}) and [Google Scholar]({{ site.author.googlescholar }}).

## First-Author Projects

<style>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1.5rem;
  margin: 1.5rem 0;
}
.project-card {
  border: 1px solid var(--global-border-color);
  border-radius: 6px;
  overflow: hidden;
  transition: box-shadow 0.2s ease;
  background: var(--global-bg-color);
}
.project-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
.project-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  display: block;
}
.project-card-body {
  padding: 1rem;
}
.project-card-body h4 {
  margin: 0 0 0.5rem 0;
  font-size: 1.05rem;
  line-height: 1.3;
}
.project-card-body p {
  margin: 0 0 0.75rem 0;
  font-size: 0.9rem;
  color: var(--global-text-color);
  line-height: 1.4;
}
.project-card-body a.project-link {
  font-size: 0.85rem;
  font-weight: 600;
  text-decoration: none;
}
</style>

<div class="project-grid">

  <div class="project-card">
    <a href="/publication/barretts_esophagus">
      <img src="/images/be.png" alt="Barrett's Esophagus Path-Omics">
    </a>
    <div class="project-card-body">
      <h4>Path-Omics on Barrett's Oesophagus</h4>
      <p>Weakly supervised deep learning predicts DNA content abnormalities directly from routine H&E biopsy images.</p>
      <a class="project-link" href="/publication/barretts_esophagus">View project &rarr;</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/publication/beacon">
      <img src="/images/be.png" alt="BEACON Framework">
    </a>
    <div class="project-card-body">
      <h4>BEACON: Spatial Immune-Molecular Profiling</h4>
      <p>Integrative framework for cancer risk stratification from routine Barrett's oesophagus histopathology.</p>
      <a class="project-link" href="/publication/beacon">View project &rarr;</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/publication/hcc_time">
      <img src="/images/ihc_time.png" alt="IHC-TIME">
    </a>
    <div class="project-card-body">
      <h4>IHC-TIME: HCC Immune Microenvironment</h4>
      <p>Computational characterisation of spatial immune phenotypes with prognostic significance in hepatocellular carcinoma.</p>
      <a class="project-link" href="/publication/hcc_time">View project &rarr;</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/publication/aih">
      <img src="/images/aih.png" alt="AI(H)">
    </a>
    <div class="project-card-body">
      <h4>AI(H): Autoimmune Hepatitis Assessment</h4>
      <p>Multi-task deep learning model for quantitative, reproducible grading and staging of autoimmune hepatitis from H&E slides.</p>
      <a class="project-link" href="/publication/aih">View project &rarr;</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/publication/ccr_fap">
      <img src="/images/fap.jpg" alt="FAP in CRC">
    </a>
    <div class="project-card-body">
      <h4>FAP Expression in Colorectal Cancer</h4>
      <p>Stromal FAP drives immune microenvironment remodelling toward an immunosuppressive state in colorectal cancer.</p>
      <a class="project-link" href="/publication/ccr_fap">View project &rarr;</a>
    </div>
  </div>

  <div class="project-card">
    <a href="/publication/fnh_hcc">
      <img src="/images/fnh.png" alt="FNH to HCC">
    </a>
    <div class="project-card-body">
      <h4>Malignant Potential of Focal Nodular Hyperplasia</h4>
      <p>First genomic evidence that a benign hepatic lesion can give rise to hepatocellular carcinoma through clonal selection.</p>
      <a class="project-link" href="/publication/fnh_hcc">View project &rarr;</a>
    </div>
  </div>

</div>

## Research Themes

### Spatially-Aware Deep Learning for Histopathological Tissue Characterisation

Combining pathology expertise with proficiency in machine learning and computational image analysis, I developed and led projects building quantitative, automated tools for histopathological tissue assessment that access biological information beyond the reach of manual review. My most significant contribution was a weakly supervised deep learning framework that predicts DNA content abnormalities, a key molecular marker of cancer progression, directly from routine H&E whole-slide images of Barrett's oesophagus biopsies, introducing a novel multi-instance learning augmentation strategy that substantially improved model performance. I further developed AI(H), a multi-task deep learning model for comprehensive histological assessment of autoimmune hepatitis that characterises multiple tissue compartments and pathological features from routine staining, providing spatially resolved, quantitative, and interpretable tissue profiles that improve reproducibility. Complementing these tools, I contributed to establishing an expert consensus morphological framework for standardised tumour-infiltrating lymphocyte assessment in gastro-oesophageal carcinomas, defining the evaluation criteria required for clinical validation of immune biomarkers in this cancer type.

1. **Ercan C**, Pan X, Paulson TG, et al. Predicting DNA content abnormalities in Barrett's oesophagus: a weakly supervised learning paradigm. *MIDL*. 2024. [Project page](/publication/barretts_esophagus) | [DOI](https://proceedings.mlr.press/v250/ercan24a.html)
2. **Ercan C**, Kordy K, Knuuttila A, et al. A deep-learning-based model for assessment of autoimmune hepatitis from histology: AI(H). *Virchows Arch*. 2024;485(6):1095-1105. [Project page](/publication/aih) | [DOI](https://doi.org/10.1007/s00428-024-03841-5)
3. Weeda YA, Salgado R, van Herpe F, ..., **Ercan C**, ..., Meijer SL. Making sense of TILs: recommendations for morphological assessment of tumour-infiltrating lymphocytes in gastro-oesophageal carcinoma. *Histopathology*. 2026. [DOI](https://doi.org/10.1111/his.70089)

### Spatial Profiling of Immune, Stromal, and Tissue Features for Cancer Progression Risk

I established a programme of work linking computational spatial profiling to cancer progression biology across multiple cancer and precancer systems. In my primary PhD project, I pioneered the computational characterisation of the spatial immune microenvironment in hepatocellular carcinoma, developing a deep learning pipeline that classifies tumour immunophenotypes from immunohistochemistry slides and demonstrating that computationally derived immunophenotypes carry prognostic significance. In a parallel project, I co-led a study establishing that stromal activation in colorectal cancer drives immune microenvironment remodelling toward an immunosuppressive state, linking stromal biology to immune tolerance and adverse prognosis. My most advanced contribution in this area is BEACON, a spatially aware integrative framework that jointly characterises molecular abnormality and spatial immune ecology from routine Barrett's oesophagus histopathology, enabling integrated cancer risk stratification from routine pathology images. I further contributed to identifying a morphometric tissue composition signature predicting freedom from invasive progression in ductal carcinoma in situ, demonstrating the generalisability of computational spatial profiling for precancer risk assessment.

1. **Ercan C**, Renne SL, Di Tommaso L, Ng CK, Piscuoglio S, Terracciano LM. Hepatocellular carcinoma immune microenvironment analysis: a comprehensive assessment with computational and classical pathology. *Clin Cancer Res*. 2024;30(22):5105-5115. [Project page](/publication/hcc_time) | [DOI](https://doi.org/10.1158/1078-0432.CCR-24-0960)
2. Coto-Llerena M\*, **Ercan C\***, Kancherla V, et al. High expression of FAP in colorectal cancer is associated with angiogenesis and immunoregulation processes. *Front Oncol*. 2020;10:979. [Project page](/publication/ccr_fap) | [DOI](https://doi.org/10.3389/fonc.2020.00979)
3. **Ercan C**, Pan X, Paulson TG, et al. Histopathology-based spatial profiling of immune and molecular features predicts cancer risk in Barrett's oesophagus. *medRxiv*. 2025. [Project page](/publication/beacon) | [DOI](https://doi.org/10.1101/2025.11.11.25339952)
4. Sobral-Leite M, Castillo SP, Vonk S, ..., **Ercan C**, ..., Wesseling J. A morphometric signature to identify ductal carcinoma in situ with a low risk of progression. *NPJ Precis Oncol*. 2025;9(1):25. [DOI](https://doi.org/10.1038/s41698-024-00769-6)

### Clonal Evolution, Tumour Heterogeneity, and Tissue Dynamics in Carcinogenesis

By integrating expertise in histopathology, molecular pathology, and translational research, I conducted and contributed to several studies investigating the molecular dynamics of tumour heterogeneity, clonal evolution, and tissue cell fate across carcinogenesis and organ regeneration. In the most conceptually significant of these contributions, I provided the first genomic demonstration that focal nodular hyperplasia, a hepatic lesion regarded as definitively benign, can give rise to hepatocellular carcinoma through clonal selection, establishing a shared genomic ancestry between the precursor lesion and the adjacent carcinoma. I further contributed to the molecular dissection of intra-tumoral heterogeneity in pulmonary pleomorphic carcinoma through multi-region profiling of histologically distinct tumour components, establishing the evolutionary relationships between tumour components and the molecular programs driving their divergent phenotypes. Extending this to regenerative biology, I contributed to the discovery of bipotent transitional liver progenitor cells, demonstrating through dual genetic lineage tracing that a biliary cell-derived progenitor population retains the capacity to adopt either hepatocyte or biliary fate during severe liver injury.

1. **Ercan C**, Coto-Llerena M, Gallon J, et al. Genomic analysis of focal nodular hyperplasia with associated hepatocellular carcinoma unveils its malignant potential: a case report. *Commun Med*. 2022;2(1):11. [Project page](/publication/fnh_hcc) | [DOI](https://doi.org/10.1038/s43856-022-00074-y)
2. Roma L, **Ercan C**, Conticelli F, et al. Tracing tumour heterogeneity of pleomorphic carcinoma of the lung. *J Thorac Oncol*. 2024;19(9):1284-1296. [DOI](https://doi.org/10.1016/j.jtho.2024.04.019)
3. Pu W, Zhu H, Zhang M, ..., **Ercan C**, ..., Zhou B. Bipotent transitional liver progenitor cells contribute to liver regeneration. *Nat Genet*. 2023;55(4):651-664. [DOI](https://doi.org/10.1038/s41588-023-01335-9)

## Collaborations & Selected Co-authored Work

### Postdoc Period (MD Anderson / CHUV)

- DeMixT 2.0: A deconvolution framework for sparse sequencing data using embedded negative binomial distribution. Submitted to AACR 2025.
- TMEseg: Tumour microenvironment segmentation from histology images for spatial transcriptomics spot annotation in lung cancer. Submitted to AACR 2025.
- AI-derived tumour-infiltrating lymphocytes enhance prediction of pathologic complete response in early-stage triple-negative breast cancer. Accepted to SABCS 2024.
- AI-derived tumour-infiltrating lymphocytes predict invasive breast cancer recurrence in ductal carcinoma in situ. Submitted to AACR 2025.
- AI-STORM: AI-guided sampling of tissues for optimal representative morphology. Accepted to USCAP 2025.

### PhD Period (University of Basel)

- GATA3 and MDM2 are synthetic lethal in estrogen receptor-positive breast cancers. *Commun Biol*. 2022;5(1):373. [PMC9018745](https://pmc.ncbi.nlm.nih.gov/articles/PMC9018745/)
- Integrative proteogenomic characterisation of hepatocellular carcinoma across etiologies and stages. *Nat Commun*. 2022;13(1):2436. [PMC9068765](https://pmc.ncbi.nlm.nih.gov/articles/PMC9068765/)
- Epigenetic priming in chronic liver disease impacts the transcriptional and genetic landscapes of hepatocellular carcinoma. *Mol Oncol*. 2022;16(3):665-682. [PMC8807355](https://pmc.ncbi.nlm.nih.gov/articles/PMC8807355/)
- TEAD4 exerts an oncogenic role in hepatocellular carcinoma by Hippo-independent regulation of HSP70 family members. *Hepatol Commun*. 2021;5(4):661-674. [PMC8034568](https://pmc.ncbi.nlm.nih.gov/articles/PMC8034568/)
- Bipotent transitional liver progenitor cells contribute to liver regeneration. *Nat Genet*. 2023;55(4):651-664. [PMC10101857](https://pmc.ncbi.nlm.nih.gov/articles/PMC10101857/)
- Live slow-frozen human tumour tissues viable for 2D, 3D, ex vivo cultures and single-cell RNA-seq. *Commun Biol*. 2022;5(1):1144. [PMC9616892](https://pmc.ncbi.nlm.nih.gov/articles/PMC9616892/)
- Transposon-activated POU5F1B promotes colorectal cancer growth and metastasis. *Nat Commun*. 2022;13(1):4913. [PMC9392749](https://pmc.ncbi.nlm.nih.gov/articles/PMC9392749/)
- YAP/TAZ and ATF4 drive resistance to sorafenib in hepatocellular carcinoma by preventing ferroptosis. *EMBO Mol Med*. 2021;13(12):e14351. [PMC8649869](https://pmc.ncbi.nlm.nih.gov/articles/PMC8649869/)
