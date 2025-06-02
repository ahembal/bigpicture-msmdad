# Bigpicture Mandatory Submission Metadata for Directly Accessible Datasets (MSMdad)

This repository provides **machine-readable XML files** specifying all mandatory CMMS Attributes and their value specifications for dataset submission, as defined by MSMdad v2.0.0.

## Structure

- `src/` — All XML files for each CMMS entity (see section 5.4 of the standard)
- `README.md` — This documentation
- `CHANGELOG.md` — Project changelog  
- `LICENSE` — License file

## What is MSMdad?

MSMdad defines the set of mandatory attributes required for every CMMS Entity when submitting datasets to the Bigpicture repository. Each XML file in this repository corresponds to a CMMS Entity or attribute group, following section 5.4 of the metadata standard.

**Version:** 2.0.0  
**Accepted:** 21.01.2025  
**Authors:** Maximilian C. Koeller, et al.

---

## Entity Definitions (section 4.3 of the metadata standard)

The CMMS comprises 16 entities, each described below:

| Entity Name       | Definition |
|-------------------|------------|
| **Dataset**       | A well-defined unit of data to be shared, with a stable identifier, data (e.g., WSI + Metadata), a controller (who holds rights), and terms of use. |
| **Policy**        | Contains information about Terms of Use (ToU) and relevant data sharing agreement provisions. |
| **Biological Being** | Represents a patient or animal from whom/which specimens are acquired for slides or data (genetics, labs, clinical history, etc.). |
| **Case**          | A collection of tissue specimens from one Biological Being collected at a single time point and processed in one pathological workup. |
| **Specimen**      | A removed part of a human or animal being. |
| **Block**         | A (part or collection of) specimen(s) sampled and processed for investigation. |
| **Slide**         | A physical slide created from one or more blocks. |
| **Image**         | A digital image of a slide. |
| **Annotation**    | A subset of image data (e.g., polygon coordinates), meaningful relative to a specific WSI, but may be stored separately. |
| **Staining**      | Encapsulates all information about a particular staining procedure. |
| **Observer**      | A human or machine performing observations on one of the following: Biological Being, Specimen, Block, Slide, Image, Annotation. |
| **Observation**   | A pathological statement about one of: Biological Being, Specimen, Block, Slide, Image, Case, or Annotation. |
| **REMS**          | Encapsulates all information needed to create a REMS catalog item for a dataset during submission. |
| **Organisation**  | Encapsulates all information about the submitting organisation, for administrative purposes. |
| **Landing Page**  | Encapsulates all information to be displayed on the landing page; used for landing page generation. |
| **Datacite**      | Defines attributes sent to DataCite to create a DOI for the dataset (if requested by the submitter). |

---

## Usage

- Use the XML files in `src/` as templates for preparing your own dataset submissions.
- Include all attributes specified as mandatory for your submission context (clinical, non-clinical, or everyone).
- For schema and metadata standard details, see the full Bigpicture metadata standard (contact the authors for access if needed).

## License

Apache 2.0

---

**Questions or contributions?**  
Open an issue or pull request!
