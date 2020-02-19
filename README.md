# SNP-Classification
## Table of contents
* [General info](#general-info)
* [Data description](#data-description)
* [Technologies](#technologies)
* [Sources](#sources)
## General info 
Project made for the needs of the subject Data Analysis in college. I tried to predict invalid SNP (Single Nucleotide Polymorphism) in data I was given with Keras in Python. This was an inbalance data so I used some unusual methods. 
I shortly described what I was doing in every line, so I think everything is clear and understandable. 
If you don't know or don't understand methods I have used, I recommend referring to their documentation or try to google it.
## Data description 
I was given data with samples of SNP and calculeted which is wrong genotyped by my Professors.
Data comes from 4 "traditional Danish Red Dairy Cattle" bulls, sequenced by NGS (Illumina) and analyzed by WGS.
Wrong quality of prediction -> rare event data
In data is 12 variables. 
* Genotype - our binary variable, 0 - wrong SNP, 1 - good SNP,
* QUAL = −10 ∙ 𝑙𝑜𝑔10[𝑃(𝐴𝐿𝑇 is wrong)] - the higher the better classification,
* DP - coverage of the reference genome,
* DP2 - coverage of the reference genome on second level.
* 𝐺𝑄 = −10 ∙ 𝑙𝑜𝑔10[𝑃(genotype is wrong|SNP)] - the higher the better classification,
* BEFORE1,2,3 - Three nucleotides before SNPs,
* BEHIND1,2,3 - Three nucleotides after SNPs,
## Technologies 
* Python 3.7
* Keras 
* Tensorflow
* Scipy
* Sklearn
* Numpy
* Matplotlib
* pandas
* Pandas profiling
## Sources 
http://theta.edu.pl/
