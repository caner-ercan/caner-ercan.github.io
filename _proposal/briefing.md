# Project Briefing — Editing Sessions
> For use in fine-tuning edit sessions only.
> Does not supersede summary.md for knowledge management purposes.

## What this project is

Precancers occupy a critical but poorly understood window in cancer
development. The transition from precursor lesion to invasive cancer
is governed not by genomic events in isolation but by the evolving
relationship between epithelial cells, the immune system, and the
stromal architecture that surrounds them — a tissue ecosystem under
selective pressure. Understanding which precancers progress, and why,
requires tools that can read this ecosystem directly from tissue.

This project develops a computational framework to do exactly that:
to quantify the spatial organisation of epithelial morphology, immune
ecology, and stromal architecture from routine histology images, and
to model how that organisation evolves toward malignancy. The central
claim is that progression is determined by the tissue ecosystem as an
integrated whole, and that this ecosystem is legible in standard
haematoxylin and eosin slides — without additional assay cost.

Barrett's oesophagus is the disease context in which the framework
is developed and validated. BE is uniquely suited to this purpose:
it is the only established precursor to oesophageal adenocarcinoma,
it progresses over years under endoscopic surveillance, and a unique
longitudinal natural history cohort provides the annotated dataset
that makes progression-relevant learning tractable. The biological
questions the framework addresses — how tissue architecture encodes
progression risk, how immune organisation shapes evolutionary
trajectories, how transcriptional programs shift across disease
stages — are not BE-specific. The framework is designed for BE;
the knowledge it generates applies to precancer biology broadly.

---

## What makes it distinctive

- **Dataset:** The project uses a unique, longitudinal, well-annotated
  BE natural history cohort with long-term clinical follow-up —
  a resource that makes progression-relevant learning tractable
  where most datasets cannot.

- **Biological grounding:** The computational models are designed
  around the known biology of BE tissue — its crypt architecture,
  compartment organisation, and immune ecology — rather than treating
  histology as generic image data. This grounding is what makes the
  representations biologically interpretable, not just predictive.

- **Integrated analysis:** The epithelial and immune models are
  trained independently and then structurally coupled. This
  separation prevents information leakage while preserving the
  ability to model their interaction — a design choice that reflects
  how the biology actually works.

- **Transcriptional resolution:** A spatial transcriptomics component
  applies whole-transcriptome profiling to paired BE and EAC tissue
  from the same resection specimen — a design that eliminates
  inter-patient confounding and provides the molecular ground truth
  that validates and extends the computational models.

---

## The three aims — current framing

Aim 1: Develops a self-supervised hierarchical graph model of
BE epithelial tissue, encoding cellular and tissue-level morphology
from H&E whole-slide images. It produces a tissue representation
model applicable to downstream pathological classification and
progression-relevant tasks.
The first hierarchycal graph autoencoder will trained to capture epithelial morphology. The layer 1 will be for individual crypt specific graphs. Here each epithelial cell will be one node. They will be classified for subtypes of metaplastic epithelium. In addition their texture, morphological features and CNN origined embeddings will lbe used to initiate the node. The graph embeddings will be carried to the next layer in the graph. The graph embeddings will be used to initiate the crypt super-nodes. The in-between stroma regions will be split into pieces and each piece will serve as stroma nodes. THey will be initiated using the CNN embeddings of the stroma images. The graph will be created. 
Following a graph autoencoder will be trainined for this using masked SSL training. This model will be finally utilized for pathology diagnostics. 

Aim 2: Extends the epithelial model with an immune ecology
layer, building a joint representation of epithelial architecture
and immune spatial organisation. It applies this integrated model
to study immune phenotypes, temporal immune evolution, and
progression-associated immune signatures.
The structure will be similar to the previous one. This time the model will incorporate the immune features. The crypt nodes from the previous frozen model will be used and stroma nodes will be removed. The immune graphs will be generated between immune cells. To capture the local interactions and reduce the weight of the model they will be pooled to generate the stroma supernodes. THey will be used to build tissue layer with crypt nodes. The model trained with masked ssl again. THe autoencoder wil lbe used for outcome relevant features, immune ecology discovery, model evolution and to stratify patients. 

Aim 3: Applies spatially-resolved transcriptomics to multi-
region EAC resection specimens to characterise the transcriptional
changes across the BE→EAC progression spectrum. Uses the
computational models from Aims 1 and 2 to guide region selection
and validates their outputs at the transcriptional level.
Resection samples will be used to discover transcriptomic changes in BE -> EAC progression. multi-region sampling will be done on resections to capture different stages of BE (dysplasia etc) and EAC locations. The previously trained models will be utilised to detect the ROI for xenium. I'll study for validation of the output of previous models and also discover transcriptomicly what are the important for the step-wise progression. 

## What the project is not

- Not solely a Barrett's oesophagus project. BE is the application
  domain and validation context. The framework, the representational
  approach, and the biological insights are intended to transfer to
  other epithelial precancers where similar tissue ecosystem dynamics
  operate.
- Not a diagnostic AI tool for clinical deployment. It is a
  research instrument for understanding progression biology.
- Not a genomics or molecular profiling project. The primary
  modality is histology; transcriptomics in Aim 3 provides
  validation and discovery, not the primary signal.
- Not a single-timepoint snapshot analysis. The longitudinal
  design and the paired resection sampling in Aim 3 are
  central to the scientific contribution.
- Not disease-agnostic. The models are deliberately designed
  for BE tissue biology. Generalisability to other precancers
  is a downstream consequence, not the primary aim.

## Register notes for editing

- Reviewers include computational pathology specialists,
  clinician-scientists, and cancer biologists. Assume no
  single reviewer covers all three domains.
- Every technical claim must be grounded in a biological
  motivation. Lead with the biological question; introduce
  the computational method as the means to answer it.
- The application targets both ground-breaking science and
  feasibility. Each section must carry both signals — neither
  alone is sufficient.
- First person is appropriate for achievement and background
  statements. Methods descriptions use "we will" or "the
  model will."
- No em-dashes. No bullet points in prose output.
- Citations inline: (Author et al., Year). Missing citations:
  [CITE: topic].

## PI expertise and collaborative network

### The dual competence

The project requires a combination of expertise rarely concentrated
in a single investigator: deep histological familiarity with BE
tissue at the cellular and architectural level, and the technical
capability to design hierarchical graph models, self-supervised
learning frameworks, and spatial transcriptomic pipelines. These
two competences are not interchangeable — the biological design
decisions (graph edge logic, node feature selection, attention
output validation) require pathological judgment; the computational
decisions (architecture, training objective, pipeline design)
require technical depth. The project is designed around both.

The PI's background spans clinical training in anatomic pathology
and an established research record in computational pathology,
cancer genomics, immune microenvironment analysis, and translational
research (Ercan, 2023, PhD thesis, University of Basel).

Prior work demonstrating this combination — use these inline when
editing feasibility and background passages:

| Topic | Citation | One-line description |
|---|---|---|
| Molecular-immune ecology integration in BE | Ercan et al., 2025, medRxiv | Spatially integrated molecular and immune features stratify BE progression risk from H&E |
| Computational spatial immunophenotyping | Ercan et al., 2024, Cancer Research | Spatial immune microenvironment model for solid tumour immunophenotyping |
| Spatial clonal analysis, precancer-malignancy | Ercan et al., 2022, Communications Medicine | Spatial genomic clonal analysis of precursor lesion and matched hepatocellular carcinoma |
| Weakly supervised molecular prediction | Ercan et al., 2024, PLMR | Weakly supervised learning for molecular predictions with spatial analysis |
| Tumour stroma and TME interactions | Coto-Llerena & Ercan et al., 2020, Frontiers in Oncology | Tumour stroma as a key TME element and its immune interactions |
| H&E morphology and immune integration | Ercan et al., 2024, Virchows Archiv | Deep learning H&E morphology integrated with immune features for pathological assessment |

### The interdisciplinary architecture

The project simultaneously requires expertise in four domains that
rarely converge: BE tissue histology at cell and crypt resolution;
hierarchical graph model design with self-supervised objectives;
landscape ecology spatial statistics applied to biological tissue;
and single-cell spatial transcriptomics in a multi-compartment
precancer system. The specific combination — ecological spatial
statistics as explicit node-level features within a deep learning
graph framework applied to a human precancer — has no prior
precedent in computational pathology.