# Tracing the Pattern of Positive Selection and Structural Conservation in the Genome Guardian Gene (TP53) during Vertebrate Evolution

This repository contains the data, analysis settings, and results for an in-silico evolutionary study of the TP53 gene across seven vertebrate species.

## Project Overview
The TP53 gene, encoding the p53 protein, is known as the "Guardian of the Genome." This study investigates the evolutionary patterns of TP53 by analyzing:
- Pairwise genetic distances
- Phylogenetic relationships (Maximum Likelihood)
- Natural selection pressure at the codon level (FEL method)

## Study Species
- *Homo sapiens* (Human)
- *Macaca mulatta* (Rhesus macaque)
- *Mus musculus* (House mouse)
- *Rattus norvegicus* (Norway rat)
- *Bos taurus* (Cattle)
- *Canis lupus familiaris* (Dog)
- *Danio rerio* (Zebrafish) - Outgroup

## Methods
- **Sequence Retrieval:** NCBI database
- **Multiple Sequence Alignment (MSA):** MUSCLE algorithm (MEGA 12)
- **Genetic Distance:** Tamura-Nei (TN93) model (MEGA 12)
- **Phylogenetic Tree:** Maximum Likelihood (ML) with 1000 bootstrap replicates (MEGA 12)
- **Selection Pressure Analysis:** Fixed Effects Likelihood (FEL) on the Datamonkey server

## Key Results
- **Genetic Distance:** The lowest divergence was observed between *Homo sapiens* and *Macaca mulatta* (3.66%), while *Danio rerio* showed the greatest divergence from mammals (52.7% – 57.6%).
- **Phylogenetics:** High bootstrap support for primate (99%) and rodent (100%) clades. *Danio rerio* formed the basal outgroup.
- **Selection Analysis:** Out of 389 non-invariant codon sites, 12 sites were under purifying selection and 4 sites (codons 14, 174, 318, 380) showed evidence of positive/diversifying selection at p ≤ 0.05.

## Repository Structure
- `data/`: NCBI accession numbers and raw sequence information.
- `results/`: Output files including genetic distance matrix, phylogenetic tree, and FEL analysis plot.
- `docs/`: Full project report in Markdown format.

## Tools Used
- MEGA 12
- Datamonkey Server (FEL method)
- MUSCLE
- NCBI Database

## License
This project is licensed under the MIT License.
