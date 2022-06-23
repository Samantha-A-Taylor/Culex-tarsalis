# Local Adaptation and Range Exanpansion in *Culex* Mosquitoes

## Introduction & Motivation
*Culex tarsalis*, (also known as the Western Encephalitis Mosquito) is a North American mosquito species known for being the principal vector of the West Nile virus along with other arboviruses. This mosquito primarily inhabits the western U.S. and comprises of three genetically distinct genetic population clusters: the Pacific, Sonoran, and Midwest clusters. Due to *Cx. tarsalis* mosquitoes carrying dangerous diseases that infect both birds and livestock animals, questions arise pertaining to the possibility of them continuing to spread east of the Mississippi. Therefore, for this project, we will be examining:

     1. What environmental factors drive local adaptation and genetic divergence in different populations of Culex?
     2. Can we predict the spread of Culex in the near future to better inform management practices to mitigate disease risks?
     
<p align="center">
<img src="https://user-images.githubusercontent.com/97530809/155350986-35c19f43-21f5-4962-86a7-393d43c75888.png" width="400" height="350">
  </p>
 
## Part One of This Project: The Reference Genome
For this project, the first genome assembly of *Cx. tarsalis* by the UC Davis DNA Technologies Core [[1]](https://academic.oup.com/g3journal/article/11/2/jkaa063/6080661) from the Kern National Wildlife Refuge colony was used as the reference genome. Their team conducted a PacBio genome assembly, sequenced two Nextera libraries (Illumina), and used two pupae for 10X library preparation. To analyze and further investigate this genome, for the purposes of this project, we:

     - Masked the genome with MaskFasta to improve alignment
     - Determining reference genome mappability with GenMap
     - Found orthogroups and gene duplication events with OrthoFinder
     - Conducted gene ontology analysis with topGO
     - Collected protein function predictive information with InterProScan
     - Assigned orthogroups IDs to functional descriptions
     - Used Natural Language Processing via UniFunc to simplify protein function annotations

## Part Two of This Project: The Sample Data
In total, 884 (442 pairs) Illumina Next-Generation Sequencing files were recieved. Each file under-went quality control and was aligned as a pair to the reference genome. To ensure and improve sample quality, each file was run through:

     - Trimmomatic to trim the reads
     - FastQC to visually and quickly assess the data

To align the paired-end reads to the reference genome, each pair of files were run through:

     - BWA mem algorithm to perform a local alignment (due to its high speed and accuracy) both pre and post reference genome masking
