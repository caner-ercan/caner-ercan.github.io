# Predicting DNA Content Abnormalities in Barrett’s Esophagus: A Weakly Supervised Learning Paradigm 
#### Abstract

Barrett’s esophagus (BE) is the sole precursor to esophageal adenocarcinoma (EAC), and is an opportunity for developing biomarkers for cancer risk assessment. DNA content abnormalities, including aneuploidy, have been implicated in the progression to EAC in BE patients, but molecular assays require valuable tissue for its detection. We propose utilizing images from routine histology to detect ploidy status using deep learning.Employing a weakly supervised deep learning approach, multi-instance learning (MIL), we trained a model to predict ploidy using hematoxylin and eosin-stained whole slide images of endoscopic biopsies and flow cytometry results. The study introduces a novel data augmentation method for MIL, sequentially altering features from original and augmented images during training loops. This method improved the average area under curve (AUC) from 0.43, 0.64 and 0.81 for ResNet50, DenseNet121 and REMEDIS foundation model, respectively (training without any augmentation), to 0.61, 0.87 and 0.91 with the proposed augmentation strategy.The top-performing model, using REMEDIS foundation model as the backbone, achieved 0.93 AUC and 0.83 balanced accuracy to predict aneuploidy in the test cohort biopsies (n=279). Across all the patients (n=123), predicted aneuploidy status was correlated with progression to EAC (p=6.55e-06), similar to correlation with ploidy status based on flow cytometry results (p=2.84e-7). Supporting the findings, histologic nuclear features typically associated with dysplasia and DNA content abnormalities such as enlarged, hyperchromatic nuclei and loss of nuclear polarity, were seen in the samples called abnormal compared to the control diploid samples.In conclusion, our deep learning model efficiently predicts aneuploidy, a mechanism that has been shown to underpin BE progression to EAC. This method, preserving precious biopsy tissues, complements routine histology, offering potential for identifying individuals at high risk of progression through molecular-based advancements.


# A deep-learning-based model for assessment of autoimmune hepatitis from histology: AI(H)

## Abstract

Histological assessment of autoimmune hepatitis (AIH) is challenging. As one of the possible results of these challenges, nonclassical features such as bile-duct injury stays understudied in AIH. We aim to develop a deep learning tool (artificial intelligence for autoimmune hepatitis [AI(H)]) that analyzes the liver biopsies and provides reproducible, quantifiable, and interpretable results directly from routine pathology slides. A total of 123 pre-treatment liver biopsies, whole-slide images with confirmed AIH diagnosis from the archives of the Institute of Pathology at University Hospital Basel, were used to train several convolutional neural network models in the Aiforia artificial intelligence (AI) platform. The performance of AI models was evaluated on independent test set slides against pathologist’s manual annotations. The AI models were 99.4%, 88.0%, 83.9%, 81.7%, and 79.2% accurate (ratios of correct predictions) for tissue detection, liver microanatomy, necroinflammation features, bile duct damage detection, and portal inflammation detection, respectively, on hematoxylin and eosin-stained slides. Additionally, the immune cells model could detect and classify different immune cells (lymphocyte, plasma cell, macrophage, eosinophil, and neutrophil) with 72.4% accuracy. On Sirius red-stained slides, the test accuracies were 99.4%, 94.0%, and 87.6% for tissue detection, liver microanatomy, and fibrosis detection, respectively. Additionally, AI(H) showed bile duct injury in 81 AIH cases (68.6%). The AI models were found to be accurate and efficient in predicting various morphological components of AIH biopsies. The computational analysis of biopsy slides provides detailed spatial and density data of immune cells in AIH landscape, which is difficult by manual counting. AI(H) can aid in improving the reproducibility of AIH biopsy assessment and bring new descriptive and quantitative aspects to AIH histology.


# Making sense of TILs: recommendations for morphological assessment of tumour-infiltrating lymphocytes in gastro-oesophageal carcinoma
## Abstract

In the era of immune checkpoint inhibitors for cancers, the need for prognostic biomarkers to identify patients most likely to achieve a durable response has become increasingly more relevant. Tumour-infiltrating lymphocytes (TILs) have gained significant interest, as they can be evaluated using standard haematoxylin and eosin-stained slides, making it a widely accessible and cost-effective biomarker. In addition to their practicality, TILs provide prognostic insights into the interplay between the immune system and tumour cells. While the morphological assessment of TILs has been standardised in breast cancer, comprehensive guidelines for their evaluation in gastro-oesophageal carcinomas (GEC) are still lacking. This narrative review examines the current literature on the composition, clinical implications and therapeutic utility of TILs in GEC. These insights are used to propose a framework with recommendations for standardised evaluation and reporting of TILs in GEC, while also highlighting pitfalls specific to GEC pathology. These recommendations serve as a vital first step towards the widespread use and validation of TILs as a biomarker.

This review examines the role of tumour-infiltrating lymphocytes (TILs) in gastro-oesophageal carcinoma (GEC), focusing on their composition, clinical relevance and therapeutic utility. It proposes a framework for standardised evaluation and reporting of TILs, addressing GEC-specific pathology challenges to support the widespread use and validation of TILs as a predictive biomarker.
# Histopathology-based Spatial Profiling of Immune and Molecular Features Predicts Cancer risk in Barrett’s Esophagus
## Abstract

**Background** Improved cancer risk stratification is needed to differentiate high-risk individuals with Barrett’s esophagus (BE) from low-risk populations to reduce overtreatment and improve outcome. The evolution of BE towards adenocarcinoma is likely driven by a combination of genomic and microenvironmental factors, yet existing predictive models rarely integrate both using routine specimens.

**Method** We developed BEACON (Barrett Esophagus DNA content Abnormality and immune ecology for Cancer Outcome), a spatially aware framework predicting DNA content abnormalities and characterizing immune spatial ecology from routine histopathology. First, using 777 BE biopsies with flow cytometry-based DNA content data scanned at two institutions, we trained and tested DACOR (DNA content abnormality recognition), a multi-instance learning model that predicts DNA content abnormalities from histopathology. Next, complementary models for cell classification and tissue segmentation enabled spatial immune ecology metric computations. Lastly, a logistic regression model integrated molecular immune ecological features and epithelial morphology for cancer risk stratification.

**Results** DACOR achieved 0.825 AUC in the test cohort for DNA content abnormality prediction. DNA content abnormal regions exhibited increased lymphoplasma cellular inflammation versus normal regions (p=0.006). Patients classified as DNA content abnormal by DACOR demonstrated increased cancer progression (p=0.0001). Among patients with DNA content abnormality, cancer progressors exhibited increased plasma cell clustering adjacent to abnormal epithelium compared to non-progressors. The integrated risk classification model stratified DNA content abnormal patients into high- and low-risk groups with 0.817 AUC.

**Conclusion** BEACON spatially integrates molecular abnormality with immune spatial ecology to stratify BE patients by cancer progression risk using routine pathology images. This scalable, explainable approach could improve clinical decision-making and reduce unnecessary surveillance in low-risk patients.


# High Expression of FAP in Colorectal Cancer Is Associated With Angiogenesis and Immunoregulation Processes
## Abstract

Fibroblast activation protein α (FAP) plays an important role in tissue remodeling and helps tumor cells invade surrounding tissue. We sought to investigate FAP as a prognostic molecular marker in colorectal cancer (CRC) using immunohistochemical and transcriptomic data. _FAP_ expression and clinicopathological information were obtained from The Cancer Genome Atlas data set. The association of _FAP_ expression and tissue cellular heterogeneity landscape was explored using the xCell method. We evaluated FAP protein expression in a cohort of 92 CRCs and 19 non-tumoral tissues. We observed that _FAP_ was upregulated in tumors both at the mRNA and protein levels, and its expression was associated with advanced stages, poor survival, and consensus molecular subtype 4. _FAP_ expression was also associated with angiogenesis and collagen degradation. We observed an enrichment in immune-cell process–related genes associated with _FAP_ overexpression. Colorectal cancers with high _FAP_ expression display an inflamed phenotype enriched for macrophages and monocytes. Those tumors showed enrichment for regulatory T cell populations and depletion of TH1 and natural killer T cells, pointing to an immunosuppressive environment. Colorectal cancers with high levels of stromal FAP are associated with aggressive disease progression and survival. Our results suggest that FAP plays additional roles in tumor progression such as modulation of angiogenesis and immunoregulation in the tumor microenvironment.

# Hepatocellular Carcinoma Immune Microenvironment Analysis: A Comprehensive Assessment with Computational and Classical Pathology

## Abstract

Purpose:

The spatial variability and clinical relevance of the tumor immune microenvironment (TIME) are still poorly understood for hepatocellular carcinoma (HCC). In this study, we aim to develop a deep learning (DL)–based image analysis model for the spatial analysis of immune cell biomarkers and microscopically evaluate the distribution of immune infiltration.

Experimental Design:

Ninety-two HCC surgical liver resections and 51 matched needle biopsies were histologically classified according to their immunophenotypes: inflamed, immune-excluded, and immune-desert. To characterize the TIME on immunohistochemistry (IHC)-stained slides, we designed a multistage DL algorithm, IHC-TIME, to automatically detect immune cells and their localization in the TIME in tumor–stroma and center–border segments.

Results:

Two models were trained to detect and localize the immune cells on IHC-stained slides. The framework models (i.e., immune cell detection models and tumor–stroma segmentation) reached 98% and 91% accuracy, respectively. Patients with inflamed tumors showed better recurrence-free survival than those with immune-excluded or immune-desert tumors. Needle biopsies were found to be 75% accurate in representing the immunophenotypes of the main tumor. Finally, we developed an algorithm that defines immunophenotypes automatically based on the IHC-TIME analysis, achieving an accuracy of 80%.

Conclusions:

Our DL-based tool can accurately analyze and quantify immune cells on IHC-stained slides of HCC. Microscopic classification of the TIME can stratify HCC according to the patient prognosis. Needle biopsies can provide valuable insights for TIME-related prognostic prediction, albeit with specific constraints. The computational pathology tool provides a new way to study the HCC TIME.


# A morphometric signature to identify ductal carcinoma in situ with a low risk of progression
## Abstract

Ductal carcinoma in situ (DCIS) may progress to ipsilateral invasive breast cancer (iIBC), but often never will. Because DCIS is treated as early breast cancer, many women with harmless DCIS face overtreatment. To identify features associated with progression, we developed an artificial intelligence-based DCIS morphometric analysis pipeline (AIDmap) on hematoxylin-eosin-stained (H&E) tissue sections. We analyzed 689 digitized H&Es of pure primary DCIS of which 226 were diagnosed with subsequent iIBC and 463 were not. The distribution of 15 duct morphological measurements was summarized in 55 morphometric variables. A ridge regression classifier with cross validation predicted 5-years-free of iIBC with an area-under the curve of 0.67 (95% CI 0.57–0.77). A combined clinical-morphometric signature, characterized by small-sized ducts, a low number of cells and a low DCIS/stroma ratio, was associated with outcome (HR = 0.56; 95% CI 0.28–0.78). AIDmap has potential to identify harmless DCIS that may not need treatment.

# Genomic analysis of focal nodular hyperplasia with associated hepatocellular carcinoma unveils its malignant potential: a case report

## Abstract

### Background

Focal nodular hyperplasia (FNH) is typically considered a benign tumor of the liver without malignant potential. The co-occurrence of FNH and hepatocellular carcinoma (HCC) has been reported in rare cases. In this study we sought to investigate the clonal relationship between these lesions in a patient with FNH-HCC co-occurrence.

### Methods

A 74-year-old female patient underwent liver tumor resection. The resected nodule was subjected to histologic analyses using hematoxylin and eosin stain and immunohistochemistry. DNA extracted from microdissected FNH and HCC regions was subjected to whole exome sequencing. Clonality analysis were performed using PyClone.

### Results

Histologic analysis reveals that the nodule consists of an FNH and two adjoining HCC components with distinct histopathological features. Immunophenotypic characterization and genomic analyses suggest that the FNH is clonally related to the HCC components, and is composed of multiple clones at diagnosis, that are likely to have progressed to HCC through clonal selection and/or the acquisition of additional genetic events.

### Conclusion

To the best of our knowledge, our work is the first study showing a clonal relationship between FNH and HCC. We show that FNH may possess the capability to undergo malignant transformation and to progress to HCC in very rare cases.

## Plain language summary

Focal nodular hyperplasia (FNH) is a lesion resulting from the abnormal growth of liver cells. It is typically considered a benign tumor that does not become malignant. In rare cases, FNH may occur alongside malignant hepatocellular carcinoma (HCC). In these cases, it is not known whether the malignant HCC may derive from the benign FNH. In this study, we reported on the analysis of a 74-year-old female patient with co-occurring FNH and HCC. We found that the FNH and HCC lesions were in fact genetically related, suggesting that the FNH gave rise to the HCC lesions. Furthermore, we found multiple cell populations within the FHN lesion that may be precursors to the HCC lesions suggesting that, in rare cases, FNH may be capable of progressing to malignant HCC. These findings may help to refine the surveillance strategy for these lesions.


# Tracing Tumor Heterogeneity of Pleomorphic Carcinoma of the Lung

## Abstract

### Introduction

Pulmonary pleomorphic carcinoma (PPC) is an aggressive and highly heterogeneous NSCLC whose underlying biology is still poorly understood.

### Methods

A total of 42 tumor areas from 20 patients with PPC were microdissected, including 39 primary tumors and three metastases, and the histologically distinct components were subjected to whole exome sequencing separately. We further performed in silico analysis of microdissected bulk RNA sequencing and methylation data of 28 samples from 14 patients with PPC. We validated our findings using immunohistochemistry.

### Results

The epithelial and the sarcomatoid components of PPCs shared a large number of genomic alterations. Most mutations in cancer driver genes were clonal and truncal between the two components of PPCs suggesting a common ancestor. The high number of alterations in the RTK-RAS pathway suggests that it plays an important role in the evolution of PPC. The metastases morphologically and genetically resembled the epithelial or the sarcomatoid components of the tumor.

The transcriptomic and epigenetic profiles of the sarcomatoid components of PPCs with matched squamous-like or adenocarcinoma-like components differed from each other, and they shared more similarities to their matched epithelial components. NCAM1/CD56 was preferentially expressed in the sarcomatoid component of squamous-like PPCs, whereas _CDH1_/E-Cadherin expression was down-regulated in the sarcomatoid component of most PPCs.

### Conclusion

Lung adenocarcinoma-like PPCs are mainly driven by RTK-RAS signaling, whereas epithelial-mesenchymal transition programs as highlighted by increased _NCAM1_ and decreased _CDH1_ expression govern the epithelial-sarcomatoid transition between the clonally related tumor components. Several alterations in PPCs pinpoint therapeutic opportunities.



# Bipotent transitional liver progenitor cells contribute to liver regeneration

## Abstract

Following severe liver injury, when hepatocyte-mediated regeneration is impaired, biliary epithelial cells (BECs) can transdifferentiate into functional hepatocytes. However, the subset of BECs with such facultative tissue stem cell potential, as well as the mechanisms enabling transdifferentiation, remains elusive. Here we identify a transitional liver progenitor cell (TLPC), which originates from BECs and differentiates into hepatocytes during regeneration from severe liver injury. By applying a dual genetic lineage tracing approach, we specifically labeled TLPCs and found that they are bipotent, as they either differentiate into hepatocytes or re-adopt BEC fate. Mechanistically, Notch and Wnt/β-catenin signaling orchestrate BEC-to-TLPC and TLPC-to-hepatocyte conversions, respectively. Together, our study provides functional and mechanistic insights into transdifferentiation-assisted liver regeneration.
