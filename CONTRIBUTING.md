# Contributing to OntPreHer3D

Thank you for your interest in contributing to **OntPreHer3D** – an ontology for the documentation of hypothetical 3D reconstructions of lost or never-built architectural heritage.

We welcome feedback, bug reports, use cases, and technical contributions!

---

## 📥 How to Contribute

### 🐞 Report an Issue
If you encounter a problem, inconsistency, or error in the ontology or documentation:
- Open an [Issue](https://github.com/igorbajena/OntPreHer3D/issues)
- Clearly describe the problem and steps to reproduce it
- Link to relevant files or classes if possible

### 💡 Suggest a Change or Feature
Have an idea to improve the ontology? Please:
- Open an issue first to discuss your suggestion
- Provide reasoning and, if applicable, references to standards or vocabularies

### 📘 Improve Documentation
You can help by:
- Fixing typos or unclear sections in the `README.md` or documentation files
- Suggesting or writing examples or SPARQL queries
- Adding diagrams or usage guides

---

## 🧠 Ontology Contribution Guidelines

If you want to contribute directly to the ontology:

### Preferred Formats
- **RDF/XML (`.rdf`)** or **OWL/XML (`.owl`)**  
  Both formats are equally accepted and should comply with OWL 2 DL standards.
  Maintain semantic alignment with CIDOC CRM, CRMinf, CRMdig, LRMoo, and OntSciDoc3D

### Tooling
- Use [Protégé](https://protege.stanford.edu/) for editing, if possible
- Avoid making structural changes without prior discussion

### Best Practices
- Reuse existing concepts where appropriate
- Add `rdfs:label` and `rdfs:comment` for new classes and properties
- Document uncertainties or interpretative decisions

---

## 🛠️ Repository Structure
ontology/ → Versioned ontology files (.rdf/.ttl)
docs/ → Documentation, diagrams, examples
README.md → Project overview
CHANGELOG.md → Release history

---

## ✅ Submitting a Contribution

1. Fork the repository
2. Create a new branch:  
   `git checkout -b my-contribution-name`
3. Make your changes (include comments in the ontology if relevant)
4. Commit with a clear message
5. Open a Pull Request (PR) and describe your changes

---

## 📜 Licensing

All contributions must be compatible with the repository's license:  
**Creative Commons Attribution 4.0 International (CC BY 4.0)**

By contributing, you agree that your work will be published under this license.

---

## 📬 Questions?

Reach out by opening an issue or contacting the maintainer directly.

