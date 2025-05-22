# Hepatocyte-Dual-Omics

Dependencies:
--R (v4.4.1)
--R Studio (Version 2023.09.1+494)
--R Packages: biomaRt (2.60.1), dplyr (1.1.4), SummarizedExperiment (1.34.0), ggplot2 (3.5.1), tibble (3.2.1), tidyr (1.3.1), PerformanceAnalytics (2.0.4), MSnbase (2.30.1), reshape2 (1.4.4), limma (3.60.6), UpSetR (1.4.0), ggrepel (0.9.6), plyr (1.8.9), and data.table (1.17.0)
--Operating system: macOS Version 11.6.2 (Big Sur)

Versions the software has been tested on:
--R (v4.4.1)
--R Studio (Version 2023.09.1+494)
--R Packages: biomaRt (2.60.1), dplyr (1.1.4), SummarizedExperiment (1.34.0), ggplot2 (3.5.1), tibble (3.2.1), tidyr (1.3.1), PerformanceAnalytics (2.0.4), MSnbase (2.30.1), reshape2 (1.4.4), limma (3.60.6), UpSetR (1.4.0), ggrepel (0.9.6), plyr (1.8.9), and data.table (1.17.0)
--Operating system: macOS Version 11.6.2 (Big Sur)

Non-standard hardware:
--None required

Installation guide and Instructions for running: 
1.	Navigate to Hepatocyte-Dual-Omics GitHub repository: https://github.com/kosaku-san/Hepatocyte-Dual-Omics
2.	Under “Code” button, click “Download ZIP” to download all contents of the repository, which includes 3 scripts and 3 required files folders.  
3.	On local computer downloads page, double-click “Hepatocyte-Dual-Omics-main.zip” to open zipped folder. 
4.	Navigate to Script 1 Folder inside main folder. Do not change the location of the “Script_1.Rmd” file or “script1_required_files” folder. 
5.	Open “Script_1.Rmd” file in RStudio. 
6.	In RStudio, click “Run” and select “Run All”. 
7.	Repeat steps 4-6 for Script 2 and Script 3 Folders. 
8.	Results can be found in respective folders.

Demo:
No demo is necessary. The scripts can be directly run with the raw data included inside the “required_files” folders. 

Run time: 
1. Script_1 run time: 5 min; 36 sec 
2. Script_2 run time: 0 min; 6 sec
3. Script_3 run time: 0 min; 57 sec

Reproduction instructions: 
All data required for reproducing our analysis and results is found inside the three “required_files” folders. Running the scripts as outlined above will reproduce our results. The attached scripts can be adapted to analyze similar data. 



Expected results:

Script1:
The main output of this script is “differential_abundance_analysis.csv”, which contains log2 Fold Change and adjusted p-value results from limma proteomics analysis. Principle component analysis (PCA) plots are also produced here and found in the “PCA_publication” folder. 

Folder: normalization_log2_imputation
--histograms_after_log2.png
--histograms_before_log2.png
--log2_intensity_vs_rank_imputed_zoom.png
--log2_intensity_vs_rank_imputed.png
--missing_values_after_MinDet_imputation.png
--violin_after_log2.png
--violin_before_log2.png
--violin_plot_after_MinDet_imputation.png

Folder: PCA_publication
--proteomics_PC1_PC2_167_points.png
--proteomics_PC1_PC2_167.png
--proteomics_PC1_PC2_500.png
--proteomics_PC1_PC2_559.png
--proteomics_PC1_PC3_167_points.png
--proteomics_PC1_PC3_167.png
--proteomics_PC1_PC3_500.png
--proteomics_PC1_PC3_559.png
--RNAseq_PC1_PC2_500.png
--RNAseq_PC1_PC3_500.png

Folder: quality_control
--correlation_chart.png
--coefficient_of_variation.png
--missing_values_filtered.png
--missing_values.png
--precursor_number_average.png
--protein_per_category_average.png

Files:
differential_abundance_analysis.csv
Uniprot_and_gene_names_of_semicolon.csv
Protein_Barplots.pdf
uniprot_ids_for_uniprot.txt
data_filter.RDS
data.RDS



Script2:
The main output of this script is “mapped_data.csv” which contains all 1:1 protein mRNA mappings with uniport symbol, uniport accession number, ensemble symbol, and ensemble ID. 

Files:
mapped_data.csv
protein_only_df.csv


Script3:
This is the primary script used to make figures shown in the text.  

Folder: All_Combined_Comparisons
--combined_comp1.csv
--combined_comp2.csv
--combined_comp3.csv
--combined_comp4.csv
--combined_comp5.csv
--combined_comp6.csv
--combined_comp7.csv
--combined_comp8.csv
--combined_comp9.csv
--combined_comp10.csv
--combined_comp11.csv
--combined_comp12.csv
 
Folder: All_Combined_Comparisons_Classified
--classified_combined_comp_12.csv
--classified_combined_comp_1.csv
--classified_combined_comp_2.csv
--classified_combined_comp_3.csv
--classified_combined_comp_4.csv
--classified_combined_comp_5.csv
--classified_combined_comp_6.csv
--classified_combined_comp_7.csv
--classified_combined_comp_8.csv
--classified_combined_comp_9.csv
--classified_combined_comp_10.csv
--classified_combined_comp_11.csv

Folder: All_Protein_Comparisons
--F0hPCvsF0hPP.csv
--F0hPCvsF24hPC.csv
--F0hPCvsM0hPC.csv
--F0hPPvsF24hPP.csv
--F0hPPvsM0hPP.csv
--F24hPCvsF24hPP.csv
--F24hPCvsM24hPC.csv
--F24hPPvsM24hPP.csv
--M0hPCvsM0hPP.csv
--M0hPCvsM24hPC.csv
--M0hPPvsM24hPP.csv
--M24hPCvsM24hPP.csv

Folder: DESeq2
--DE_F0hPC_vs_F0hPP.csv
--DE_F0hPC_vs_F24hPC.csv
--DE_F0hPC_vs_M0hPC.csv
--DE_F0hPP_vs_F24hPP.csv
--DE_F0hPP_vs_M0hPP.csv
--DE_F24hPC_vs_F24hPP.csv
--DE_F24hPC_vs_M24hPC.csv
--DE_F24hPP_vs_M24hPP.csv
--DE_M0hPC_vs_M0hPP.csv
--DE_M0hPC_vs_M24hPC.csv
--DE_M0hPP_vs_M24hPP.csv
--DE_M24hPC_vs_M24hPP.csv

Folder: Figure4C-4D_data
--3_type3.csv
--1_concordant.csv
--1_type1.csv
--1_type2.csv
--1_type3.csv
--2_concordant.csv
--2_type1.csv
--2_type2.csv
--2_type3.csv
--3_concordant.csv
--3_type1.csv
--3_type2.csv
--4_concordant.csv
--4_type1.csv
--4_type2.csv
--4_type3.csv
--5_concordant.csv
--5_type1.csv
--5_type2.csv
--5_type3.csv
--6_concordant.csv
--6_type1.csv
--6_type2.csv
--6_type3.csv
--7_concordant.csv
--7_type1.csv
--7_type2.csv
--7_type3.csv
--8_concordant.csv
--8_type1.csv
--8_type2.csv
--8_type3.csv
--9_concordant.csv
--9_type1.csv
--9_type2.csv
--9_type3.csv
--10_concordant.csv
--10_type1.csv
--10_type2.csv
--10_type3.csv
--11_concordant.csv
--11_type1.csv
--11_type2.csv
--11_type3.csv
--12_concordant.csv
--12_type1.csv
--12_type2.csv
--12_type3.csv

Folder: System2_3out4
--metabolism_concordant_system2_3out4.csv
--metabolism_type1_system2_3out4.csv
--metabolism_type2_system2_3out4.csv
--sex_concordant_system2_3out4.csv
--sex_type1_system2_3out4.csv
--sex_type2_system2_3out4.csv
--zone_concordant_system2_3out4.csv
--zone_type1_system2_3out4.csv
--zone_type2_system2_3out4.csv

Files:
Figure5D_data_&_Suppl.Table_1.csv
SuppFigure2B_across-gene_data.csv
SuppFigure2B_within-gene_data.csv
SuppFigure2E_data_metabolism.csv
SuppFigure2E_data_sex.csv
SuppFigure2E_data_zone.csv
SuppFigure2F_data_metabolism.csv
SuppFigure2F_data_sex.csv
SuppFigure2F_data_zone.csv
SuppFigure3H_data.csv
Figure2A.jpg
Figure2C_metabolism.jpg
Figure2C_sex.jpg
Figure2C_zone.jpg
Figure3A.jpg
Figure3B.jpg
Figure3C.jpg
Figure4A.jpg
Figure4B_concordant.jpg
Figure4B_typeI.jpg
Figure4G.jpg
Figure5A.jpg
Figure5B.jpg
Figure5C.jpg
SuppFigure2C.jpg
SuppFigure2D.jpg
SuppFigure3A.jpg
SuppFigure3B.jpg
SuppFigure3C.jpg
SuppFigure3D.jpg
SuppFigure3E.jpg
SuppFigure3F.jpg



Trouble-shooting:
A recursive error (shown below) sometimes occurs when running Script 3. This problem can be fixed by quitting the R-studio session and re-opening the Script_3.Rmd file. 

Error: no more error handlers available (recursive errors?); invoking 'abort' restart
Warning: type 29 is unimplemented in 'type2char'
Error in scan(file = file, what = what, sep = sep, quote = quote, dec = dec,  : 
  INTEGER() can only be applied to a 'integer', not a 'unknown type #29'


