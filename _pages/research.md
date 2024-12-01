---
layout: archive
title: "Publications & Research"
permalink: /research/
date: 2024-11-23
type: page
author_profile: true
menu:
  main:
    name: "Publications & Research"
    weight: 2
---

Welcome to my Publications & Research page! Here, I highlight my authored and collaborative research contributions.
<div class="wordwrap">You can also explore my work on <a href="{{site.author.webofscience}}">Web of Science</a> and <a href="{{site.author.googlescholar}}">Google Scholar</a>.</div>

My primary focus is on leveraging advanced image analysis tools to extract quantifiable features from pathology images, aiming to discover prognostically relevant patterns directly from routine pathology slides. This includes studying molecular alterations and the tumor immune microenvironment.


<div style="display: flex; flex-direction: column; align-items: center;">

  <!-- Research Papers Flex -->
  <div style="display: flex; flex-direction: row; justify-content: space-evenly; flex-grow: 1;">

    <!-- Postdoc Section -->
    <div style="display: flex; flex-direction: column; gap: 1rem; justify-content: space-evenly; margin-bottom: 1rem; padding: 1rem;">
      <div style="flex: 1; text-align: center;">
        <h2>Postdoc</h2>
      </div>
      <div style="flex: 4; display: flex; justify-content: center;">
        <div style="text-align: center;">
          <a href="/publication/barretts_esophagus">
            <img src="/images/be.png" alt="" style="width: 350px; border: 1px solid #555;">
          </a>
          <p><strong onclick="updateInfo('postdoc1')">Path-Omics on Barrett's Esophagus</strong></p>
        </div>
      </div>
    </div>

    <!-- Vertical line -->
    <div style="display: flex; flex-direction: column; justify-content: space-evenly; margin-bottom: 1rem;">
      <div style="width: 1px; height: 100px; background-color: black;">
      </div>
    </div>

    <!-- PhD Section -->
    <div style="display: flex; flex-direction: column; gap: 1rem; justify-content: space-evenly; margin-bottom: 1rem; padding: 1rem;">
      <div style="flex: 1; text-align: center; padding-right: 1rem;">
        <h2>PhD</h2>
      </div>
      <div style="flex: 4; flex-direction: row; display: flex; gap: 1rem;">
        <div style="text-align: center;">
          <a href="/publication/hcc_time">
            <img src="/images/ihc_time.png" alt="IHC-TIME" style="width: 350px; border: 1px solid #555;">
          </a>
          <p><strong onclick="updateInfo('phd2')">IHC-TIME</strong></p>
        </div>
        <div style="text-align: center;">
          <a href="/publication/aih">
            <img src="/images/aih.png" alt="AI(H)" style="width: 350px; border: 1px solid #555;">
          </a>
          <p><strong onclick="updateInfo('phd3')">AI(H)</strong></p>
        </div>
        <div style="text-align: center;">
          <a href="/publication/ccr_fap">
            <img src="/images/fap.jpg" alt="FAP in CRC" style="width: 350px; border: 1px solid #555;">
          </a>
          <p><strong onclick="updateInfo('phd4')">FAP in CRC</strong></p>
        </div>
        <div style="text-align: center;">
          <a href="/publication/fnh_hcc">
            <img src="/images/fnh.png" alt="FNH to HCC" style="width: 350px; border: 1px solid #555;">
          </a>
          <p><strong onclick="updateInfo('phd5')">FNH to HCC</strong></p>
        </div>
      </div>
    </div>

  </div>

  <!-- Quick Info Box -->
  <div id="info-box" style="padding: 1rem; border: 1px solid #ccc; border-radius: 5px; width: 90%; background-color: #f9f9f9;">
    <p id="info-title" style="text-align: left; font-size: 1.5rem; font-weight: bold;">
    </p>
    <p id="info-text" style="text-align: left; font-size: 1rem;">
    <i>For a short summary, please click on a project title.</i>
    </p>
  </div>

</div>

<script>
  // Quick info descriptions
    const descriptions = {
      postdoc1: {
          title: "Path-Omics: Ecological Analysis of Barrett's Esophagus",
          text: "This project focuses on the spatially computational analysis of Barrett's Esophagus biopsy images to identify cancer progression-related changes. These include abnormalities in DNA content and alterations in the spatial immune microenvironment. This project has financed by SNF.",
          link: "/publication/barretts_esophagus"
      },
      phd2: {
          title: "IHC-TIME: Comprehensive Hepatocellular Carcinoma Immune Microenvironment Analysis",
          text: "As the main project of my PhD, this study investigated the tumor immune microenvironment in hepatocellular carcinoma (HCC) for the first time following the Immuno-Oncology Working Group’s recommendations. The project demonstrated the applicability and significance of microscopic evaluation of immune responses and their relationship with patient prognosis, histology, and tumor heterogeneity. Additionally, we developed a computational pathology tool to analyze slides with accuracy, interpretability, and reproducibility.",
          link: "/publication/hcc_time"
      },
      phd3: {
          title: "AI(H): A Deep-Learning Model for Assessing Autoimmune Hepatitis",
          text: "This study aimed to develop a computational pathology tool to analyze liver biopsies for autoimmune hepatitis. Current evaluations rely on semi-qualitative assessments by pathologists under a microscope. Our tool enhances reproducibility in these assessments while introducing fully quantitative evaluations for improved pathological insights.",
          link: "/publication/aih"
      },
      phd4: {
          title: "FAP Expression in Colorectal Cancer: Links to Angiogenesis and Immunoregulation",
          text: "This study highlights the significance of the tumor stroma in the tumor microenvironment, focusing on FAP protein expression in cancer-associated fibroblasts. We demonstrated its role in tumor progression, immunoregulatory processes, and patient prognosis.",
          link: "/publication/ccr_fap"
      },
      phd5: {
          title: "Genomic Insights Into the Malignant Potential of Focal Nodular Hyperplasia",
          text: "This project explored tumor heterogeneity in a liver carcinoma adjacent to a benign lesion (focal nodular hyperplasia). Spatial genomic analysis revealed a clonal relationship between the lesions, providing the first genomic evidence of malignant transformation from a lesion previously considered benign.",
          link: "/publication/fnh_hcc"
      }
  };

  // Function to update the info box
  function updateInfo(key) {
    const infoTitle = document.getElementById("info-title");
    const infoText = document.getElementById("info-text");

    const title = descriptions[key]?.title || "Title not found.";
    const description = descriptions[key]?.text || "Description not found.";
    const link = descriptions[key]?.link || "#";
    const finalText = `${title} </br> ${description} <br>For detailed info, please go to the project's page following <a href="${link}" target="_blank">this link</a>.`;
    

    infoTitle.textContent = title; // Update the title text
    infoText.innerHTML = `${description} <br>For detailed info, please go to the project's page following <a href="${link}" target="_blank">this link</a>.`;

    const infoBox = document.getElementById("info-box");

    infoBox.style.display = "block"; // Show the box
  }
</script>

<br>


# Research Summary

## 1. During Postdoc (MD Anderson Cancer Center)


<details> <summary style="font-weight: bold;"> Conducted Research </summary>


Here, I present the research projects I led as the first author.<br>


During my postdoctoral fellowship in the United States, I have been conducting research in computational pathology. My main project, "Deep learning-based whole-slide image analysis for immune ecology and cancer progression prediction in Barrett’s esophagus," aims to:

  1- Predict aneuploidy directly from endoscopic biopsy images.

  2- Investigate the spatial distribution of immune responses to uncover tumor-immune interactions.

  3- Identify features relevant to cancer progression.

  4- Develop a prognostic prediction tool.


This fellowship was funded by the <a href="https://data.snf.ch/grants/grant/214162">funded by SNF in postdoc.Mobility grant schema</a>. While this project is ongoing, key milestones have been presented at scientific conferences. For more details, visit <a href="/publication/barretts_esophagus">this page</a>.  <br>

</details>

<details> <summary style="font-weight: bold;"> Collaborations & Contributions </summary>

Besides my main project, I have been involved in multiple projects in my lab which I contribute with my expertise in pathology, morphology, immunemicroenvironment or pathologenesis, and also utilisation of softwares, algorithms in computarinal pathology research. THe collaborations which I involved and reached a milestone that could be published are listed below with brief desriptions. <br>

  - Spatial Transcriptomics Deconvolution: Developed an algorithm to deconvolve spatial transcriptomics data, submitted to AACR 2025.
    - DeMixT 2.0: A Deconvolution Framework for Sparse Sequencing Data Using Embedded Negative Binomial Distribution.<br>

  - Tumor Immune Microenvironment Segmentation: Developed a tool to annotate spatial transcriptomics spots for lung cancer, submitted to AACR 2025.
    - TMEseg: Tumor Microenvironment Segmentation from Histology Images.<br>

  - Breast Cancer Response Prediction: Built an AI-based tool to predict response to treatment in invasive breast carcinoma, accepted to SABCS 2024.
    - AI-Derived Tumor-Infiltrating Lymphocytes Enhance Prediction of Pathologic Complete Response in Early-Stage Triple-Negative Breast Cancer.<br>

  - Ductal Carcinoma Progression Prediction: Created a tool for progression prediction in ductal carcinoma in situ, submitted to AACR 2025.
    - AI-Derived Tumor-Infiltrating Lymphocytes Predict Invasive Breast Cancer Recurrence.<br>

  - Morphological Feature Analysis: Revealed cancer progression features in ductal carcinoma in situ, accepted to npj Precision Oncology.
    - A Morphometric Signature to Identify Ductal Carcinoma In Situ with Low Risk of Progression.<br>

  - Tumor Heterogeneity Sampling Tool: Developed a computational pathology tool for reproducible sampling of heterogeneous tumor regions, accepted to USCAP 2025.
    - AI-STORM: AI-Guided Sampling of Tissues for Optimal Representative Morphology.<br>

</details>

## 2. During PhD  (University of Basel)

<details>
    <summary style="font-weight: bold;">Conducted projects</summary>
During my PhD, I conducted two primary computational pathology projects:

  - Tumor Microenvironment Quantification in Hepatocellular Carcinoma:
Developed an AI-based model to quantify immune cells and classify tumors into inflamed, immune-excluded, and immune-desert phenotypes based on Nature's 2017 classification.

  - Autoimmune Hepatitis Biopsy Analysis:
Created the first computational pathology model to grade and stage autoimmune hepatitis biopsies from H&E slides while quantifying immune cells within the microenvironment.

Both projects were recognized with poster awards at international conferences.

Additionally, I led molecular and translational pathology studies on liver and colorectal carcinomas. These included:

  - Investigating the role of cancer-associated stroma in tumor progression.

  - Establishing a molecular link between focal nodular hyperplasia and hepatocellular carcinoma progression.

</details>


<details>
    <summary style="font-weight: bold;">Collaborations & Contributions</summary>

During my PhD, I worked in an interdisciplinary lab focusing on genomic changes in solid cancers. As the lab's pathologist, I contributed to experimental design, patient dataset creation, and microscopic evaluations of diverse samples, including biopsies, cell cultures, animal models, and organoids.

I also collaborated extensively with other labs in Basel’s vibrant biomedical research community, participating in studies using techniques like spatial transcriptomics, FISH, IHC, and RNA-seq. Below are selected publications from these collaborations:

  a.	GATA3 and MDM2 are synthetic lethal in estrogen receptor-positive breast cancers. Commun Biol. 2022 Apr 19;5(1):373. PubMed Central PMCID: PMC9018745. 

  b.	Integrative proteogenomic characterization of hepatocellular carcinoma across etiologies and stages. Nat Commun. 2022 May 4;13(1):2436. PubMed Central PMCID: PMC9068765. 

  c.	Epigenetic priming in chronic liver disease impacts the transcriptional and genetic landscapes of hepatocellular carcinoma. Mol Oncol. 2022 Feb;16(3):665-682. PubMed Central PMCID: PMC8807355. 

  d.	Transcriptional Enhancer Factor Domain Family member 4 Exerts an Oncogenic Role in Hepatocellular Carcinoma by Hippo-Independent Regulation of Heat Shock Protein 70 Family Members. Hepatol Commun. 2021 Apr;5(4):661-674. PubMed Central PMCID: PMC8034568. 

  e.	Bipotent transitional liver progenitor cells contribute to liver regeneration. Nat Genet. 2023 Apr;55(4):651-664. PubMed Central PMCID: PMC10101857. 

  f.	Live slow-frozen human tumor tissues viable for 2D, 3D, ex vivo cultures and single-cell RNAseq. Commun Biol. 2022 Oct 28;5(1):1144. PubMed Central PMCID: PMC9616892. 

  g.	Transposon-activated POU5F1B promotes colorectal cancer growth and metastasis. Nat Commun. 2022 Aug 20;13(1):4913. PubMed Central PMCID: PMC9392749. 

  h.	YAP/TAZ and ATF4 drive resistance to Sorafenib in hepatocellular carcinoma by preventing ferroptosis. EMBO Mol Med. 2021 Dec 7;13(12):e14351. PubMed Central PMCID: PMC8649869. 


</details>





