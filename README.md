# Final-Project
Description: 
Differential gene expression in Mouse embryonic cap staged tooth germs With /without 2,3,7,8-tetrachlorodibenzo-p-dioxin (TCDD). ( Control and sample respectively).

Dataset: 
I am using GEO database from NCBI. This data is expression profiling by micro–array analysis. 
 The data is available in the form of Txt file. However, I am planning to use GEOquery library in the bio-conductor package that takes care of finding the file and unzip it. 
Link to the data:
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE4873 


Proposed analysis:
Planning to make heat-map and volcano plot in r to show differential gene expression.
Libraries:
ggplot,
GEOquery: to get the dataset in the R,
Bioconductor Package 


Proposed Timeline & Major milestones (or segments):
Successfully loading the data into R-studio as data-frame.
Normalize the data. 


User Interface:
Heat-map combined with the clustering to show which genes are up regulated and which genes are down regulated. 

Milestone 1 (11/13/18): 
Progress: I was able to upload data successfully into R From GEO database. I used GEOquery from the bioconductor package. 
I was able to successfully convert the data into expression matrix by using the Function exprs.
Next Steps:
Generate heatmap and Volcano-plot.
Feedback:
Add additional to look in the dataset.
Understand the data and figure out what are rows and columns

Milestone 2 (11/20/18)
Progress: I added gene Id as an additional factor in my dataset and now my data is easy to understand. (earlier it was like 1,2 &3 and not making any sense what I am looking at).
I made histogram with the data which doesn't look like guassian. After that I did log2 transformation to convert the data into guassian curve.(data is still skewed to the left) 
I made boxplot and heatmap with the data and failed to do T-test(it says that data is not logical because of the NA, Infinity and -inf)
Next Step: Try to remove NA, infinity and -Infinity values from the data.
Normalize data by dividing mean of each column for each column
try t-test after this.


