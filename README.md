# InsightOfFAIR-OpenPracticesInMicrobialBiotechnology

Dataset for "How well is Microbial Biotechnology research sharing FAIR and Open research data and why?"

Author:
George Strevens

General Information

1. Abstract:

Within the scientific ecosystem there has been growing emphasis on the adoption of FAIR and Open data sharing in research, supporting the belief that data underpinning research should be equally accessible and transparent to research outcomes themselves. This study manually reviews 130 journal articles against a scoring criterion focused on FAIRness and Openness. Findings show increases in the Completeness, Reusability and Accessibility of Microbial Biotechnology research data with genomic data being the most frequently shared data type compared to Image and Proteo-metabolomic. The presence of Data Availability Statements has a positive correlation with higher scores for FAIRness and Openness, while preprints only correlate to improved Completeness. Since the implementation of FAIR principles in 2016, we have observed significant improvements in data Completeness, Accessibility and Reusability accompanied by an increased presence of Data Availability Statements. Similarly, the COVID-19 onset had a comparable effect leading to significant improvements in data completeness and Reusability as well as the inclusion of Data Availability Statements. This study evaluates how well institutes in the School of Biological Sciences at the University of Edinburgh are sharing FAIR and Open research data from Microbial Biotechnology research, assessing progress over the past decade; identifying changes and promoting the best practices.

2. Data Reuse:

The provided dataset should facilitate further research and analysis in the field of FAIR and Open Data in Microbial Biotechnology. Researchers are encouraged to replicate study findings using this data, with the opportunity to ectend research into new areas. Before reusing the data, accompanying variable descriptions should be reviewed alongside the usage guidelines, ensuring accurate interpretation. 

Dataset Overview



Dataset Description

1. MicrobialBiotechnology_Publications_Dataset:
   
The dataset is derived from a comprehensive analysis of selected publications in the field of Microbial Biotechnology, presented in CSV format. It is designed for use with statistical software, like RStudio, to facilitate detailed analysis.
CSV File Structure: The dataset contains rows corresponding to selected publications, each characterized by a set of variables critical to our study. The columns in the CSV file represent these variables.

Excel File Structure (MicrobialBiotechnology_Publications_Dataset.xlsx)
-Sheet 1 (Dataset): Contains rows of selected publications and columns representing the variables used in our analysis.The raws that are highlighted in yellow, are the papers that have been randomly selected for reassessing
-Sheet 2 (Variable Descriptions): Provides a detailed explanation of each variable and the values they represent.

CSV File (MicrobialBiotechnology_Publications_Dataset.csv)
The CSV file is derived from Sheet 1 of the Excel file and was imported into RStudio for analysis.

Variable	Description - (Format)   
Title	= The title of the article -(Text)
DOI = Digital Object Identifier for the article -(Alphanumeric)
ResGrp = The research group or principal investigator's surname- (Text)
TypE = The type of disease studied (NCD or InfD)- (Categorical)
Institution	= The institution of the research group- (Text)
Journal = The journal in which the article was published -(Text)
Year = The publication year of the article -(Numeric)
AnalysisPgrm = Indicates if analysis software is stated (1) or not (0) -(Binary)
CodeArchived = Indicates if the analysis code is archived (1) or not (0); NA if not applicable -(Binary/NA)
DAS = Data Availability Statement presence and type -(Binary/NA)
CorresAuthor = Indicates if the group leader is a corresponding author (1) or not (0) -(Binary)
Preprints = Indicates if a preprint was shared (1) or not (0) -(Binary)
Complete = Completeness score of the data and metadata -(Numeric 1-4)
Reuse = Reusability score of the data -(Numeric 1-4)
Access = Accessibility score of the data -(Numeric 1-4)
Licence = Clarity and accessibility of the data usage license -(Numeric 1-4)
Image = Image data sharing status -(Binary/NA)
Genomics = Genomic data sharing status -(Binary/NA)

RMarkdown Code

MicrobialBiotechnology_Project_RMarkdown_Code.pdf
The provided PDF is a knitted version of the RMarkdown code, presenting a static and complete view of the code, figures, and tables as outputs. This format enhances accessibility, allowing those not versed with RStudio or RMarkdown to easily view and share the research findings. It also acts as an archival record, capturing the code in a fixed form to preserve the analysis for future reproducibility. Additionally, the PDF format offers the convenience of a quick review or a printout of the research methods and outcomes, streamlining the understanding of the study's methodology and findings in one document.

Usage Instructions:

To use the RMarkdown code

Open the .Rmd file in RStudio.
Import the csv file "MicrobialBiotechnology_Publications_Dataset.csv"

Ensure that the required libraries are installed:

dplyr
lubridate
ggplot2
tidyr
scales
MASS
patchwork
ordinal
VGAM
gmodels
emmeans
reshape2

Run each code chunk sequentially to reproduce the analyses and figures from our study.

