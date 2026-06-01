# Site Edit Plan & Tracker

Session: 2025-06-01

---

## Completed

### About

- [x] **Rewrite about page**
  - Replaced outdated bio (MD Anderson as current) with CHUV position and dual pathologist/ML identity
  - Three research pillars with subheadings (ML for digital pathology, tumours as ecosystems, image-omics)
  - Added collaboration invitation closing
  - British English, no em-dashes

### Research

- [x] **Redesign research page**
  - Removed interactive JS/CSS card section and collapsible `<details>` summaries
  - New structure: First-Author Projects grid, three Research Themes with narrative + citations, Collaborations section
- [x] **Create BEACON publication page**
  - Created `_publications/beacon.md` for the medRxiv preprint
  - Needs image and expanded content later
- [x] **Fix project card dark/light mode**
  - Replaced hardcoded colours with CSS custom properties (`--global-bg-color`, `--global-border-color`, `--global-text-color`)

---

## Pending

### CV

- [x] **Redesign CV page**
  - [x] Modern, clean layout with consistent heading hierarchy
  - [x] Fix reversed residency dates ("11/2024 - 02/2019" → "02/2019 - 11/2024")
  - [x] Remove commented-out placeholder content
  - [x] Sections: Education, Academic Appointments, Grants & Fellowships, Awards & Honours, Professional Memberships
  - [ ] **Unresolved design issue**: Vertical line persists after cv-header entries despite converting to pure HTML (`_pages/cv.html`). Requires further debugging.

### Talks

- [x] **Create talks page and collection**
  - [x] Uncomment `talks` collection in `_config.yml`
  - [x] Delete 3 dummy talk files
  - [x] Create 13 proper collection entries (4 oral/short talks, 9 posters)
  - [x] Create `_pages/talks.md` listing page with categories: Invited & Oral Presentations, Posters (Postdoc / PhD)
  - [x] Add "Talks" link to `_data/navigation.yml`

### About (follow-up)

- [ ] **Add figures to research pillars on about page**
  - [ ] Insert one representative figure per research pillar (ML for digital pathology, tumours as ecosystems, image-omics)

### Research (follow-up)

- [ ] **Distribute collaborations into research themes**
  - [ ] Move relevant collaboration items into the three main research theme sections
  - [ ] Create separate categories for items that do not fit existing themes
- [ ] **Add BEACON project card image**
  - [ ] Replace placeholder image (currently reusing Barrett's oesophagus image)
- [ ] **Update `barretts_esophagus.md` project page**
  - [ ] Fix typos in body text
  - [ ] Align narrative with BEACON now being a separate project

### Publications

- [ ] **Add missing publications**
  - [ ] Identify publications not yet represented in the site
  - [ ] Create individual `_publications/*.md` entries following existing frontmatter pattern
  - [ ] Link them from the relevant research theme sections

### Cleanup

- [ ] **Fix typos in publication pages**
  - [ ] `barretts_esophagus.md`: "projecy" → "project", "projct" → "project", "aneuoploidy" → "aneuploidy", "microenviromental" → "microenvironmental", "heterogeniety" → "heterogeneity", "ging" → "going", "presentationss" → "presentations"
  - [ ] `ccr_fap.md`: broken markdown link syntax `(text)[url]` → `[text](url)`
- [ ] **Uncomment pubmed link** in `_config.yml` (currently commented out)
