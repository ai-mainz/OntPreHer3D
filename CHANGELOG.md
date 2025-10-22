# Changelog

All notable changes to OntPreHer3D are documented in this file.

This changelog follows the format recommended by [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)  
and uses [Semantic Versioning](https://semver.org/).

## [2.1.1] – 2025-10-22

### Added
- Introduced new object property **R40 has phase**  
  (`https://www.ontscidoc3d.hs-mainz.de/OntPreHer3D/R40_has_phase`)
  - Establishes a relationship between **E22 Man-Made Object** and **M69 Phase**, enabling documentation of stylistic, chronological, or developmental stages (e.g., Romanesque, Gothic, Baroque).
  - **Quantification:** many to many (0,n:0,n)
  - Supports multi-phase cultural heritage documentation, allowing multiple objects to share a phase and one object to belong to several phases.
  - Added inverse property **R40i is phase of** for bidirectional reasoning consistency.
  - Property definition introduced and validated in both the **RDF ontology file** and the **PDF documentation**.

### Fixed
- Performed structural validation and namespace consistency check following the addition of R40.

### Version context
- This release expands OntPreHer3D’s conceptual coverage to better represent the temporal and stylistic evolution of physical heritage objects.
- No backward-incompatible or breaking changes introduced.

---

## [2.1.0] – 2025-10-20

### Added
- Introduced one new ontology **class** and one new **object property**, defined both in RDF and PDF documentation.
- Completed full **structural normalization** of ObjectProperties:
  - unified annotation order (`rdfs:label`, `skos:notation`, `skos:prefLabel`, `rdfs:comment`, `owl:inverseOf`);
  - ensured every property has either `rdfs:subPropertyOf` or both `domain` and `range`;
  - enforced consistent inverse definitions with `owl:inverseOf` in both directions.
- Grouped and alphabetically **sorted** all ontology elements for clarity.
- Added missing inverse and quantification metadata to several all properties.
- Introduced clean, human-readable comments and scope notes.

### Changed
- Merged all correction notes from *OntPreHer3D v2 Corrections* (CHANGES.md) into the canonical file.
- Converted 14 previously misdefined properties (previously in `rdf:Description` blocks) into valid `owl:ObjectProperty` definitions:
  - R7, R7i  
  - R12, R12i  
  - R13, R13i  
  - R15, R15i  
  - R22, R22i  
  - R27, R27i  
  - R34  
  - R9i (marked obsolete, replaced by `R10i_is_simulated_by`)
- Normalized indentation, line endings, and URI consistency across all elements.

### Fixed
- Resolved namespace consistency issues inherited from v2.0.0.
- Eliminated redundant or malformed annotation fragments.
- Verified all inverse relationships, comments, and quantifications are syntactically valid.

### Validation
- File validated using RDFLib: **no structural errors** detected.
- Verified all `skos:notation` codes unique and inverses mutually linked.

---

## [2.0.0] – 2025-07-25

### Added
- Major ontology refactor derived from v1.0.1:
  - Consolidated ObjectProperties into semantic groups.
  - Introduced new versioned file `OntPreHer3D_v.2.0.0.owl`.
- Extended CIDOC CRM / CRMDig / OntSciDoc3D alignment.
- Introduced several new properties for Digital Reconstruction workflows (R7–R18 family).

### Changed
- Replaced inconsistent RDF serialization with unified `.owl` file format.
- Simplified hierarchy and grouped by property domain (Reconstruction, Material, Source, Temporal).
- Removed deprecated intermediate versions.

---

## [1.0.2] – 2025-06-30

### Documentation
- Upload of graphical schemes (on the example of rexonstruction of Speyer Synagogue) to `docs/` folder, illustrating:
  - Classes hierarchy
  - Main documentation triple
  - Documentation scheme of Digital Reconstruction with shortcut property
  - Documentation scheme of Digital Reconstrcution through full path and simulation event
  - Documentation scheme of material creation and application to the 3D model
- No changes were made to classes, properties, or namespaces—this is a purely documentation-only update.

---

## [1.0.1] – 2025-06-13

### Added
- First formal public release of OntPreHer3D ontology version 1.0.1.
- Uploaded versioned ontology file (`OntPreHer3D 1.0.1.rdf`) and documentation (`OntPreHer3D 1.0.1.pdf`).


### Changed
- Applied semantic versioning to repository structure and filenames.
- Retrospectively documented previous ontology versions for transparency.

---

## [Repository Maintenance] – 2025-05-27
### Added
- Created `CHANGELOG.md`, `LICENSE`, and `CONTRIBUTING.md`
- Structured folders: `ontology/`, `docs/`
- Added CoVHer glossary alignment and EU funding acknowledgment to `README.md`
- Created full citation, contact, and acknowledgment sections

### Changed
- Rewrote `README.md` for clarity and completeness
- Renamed existing files to follow standardized semantic versioning scheme:
  - `OntPreHer3D_v1.owl` → `OntPreHer3D 0.9.0.owl`
  - `OntPreHer3D version 1.0.pdf` → `OntPreHer3D 0.9.0.pdf`
  - `OntPreHer3D version 2.1.pdf` → `OntPreHer3D 1.0.1.pdf`
  - `OntPreHer3D_v2.1.rdf` → `OntPreHer3D 1.0.1.rdf`
- These changes align repository structure with semantic versioning to improve clarity, usability, and consistency across releases.
- Clarified that version `0.9.0` was a draft with invalid namespace and never officially released.

---

## [1.0.1] – 2024-05-27 
### Removed
- Removed of LRMoo reference
  
### Added
- Minor ontology updates since version 1.0.0.

---

## [1.0.0] – 2024-05-03 
### Changed
- First stable non-public release of OntPreHer3D.
- RDF file with defined namespace.
- Project documentation in PDF format.
- Base structure of ontology and semantic alignment with CIDOC CRM, CRMinf, CRMdig, LRMoo, and OntSciDoc3D.

---

## [0.9.0] – 2024-04-23
### Known Issues
- Draft OWL version with invalid or unstable namespace.
- Draft of PDF documentation
- Not intended for reuse or citation.
