# translation-stats

This repository contains **aggregated statistics and error summaries** from a pipeline that translates **GA4GH VRS Alleles into the FHIR Allele profile**.

The pipeline primarily processes **ClinVar variation files**, extracting **VRS Allele objects** from each record’s members array. Extracted alleles are validated against the GA4GH VRS model, and valid alleles are translated into the **FHIR Allele profile** using the `VrsToFhirAlleleTranslator`.

The variant data processed by the pipeline is derived from the **ClinVar Genomic Knowledge Standards (GKS)** initiative, a ClinGen-supported effort to transform ClinVar releases into GA4GH-compliant representations. The source data is accessed via public URLs and is hosted in the official ClinVar GKS GitHub repository:
https://github.com/clingen-data-model/clinvar-gks
