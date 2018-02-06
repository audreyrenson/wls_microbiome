/Fastq -- directory containing fastq zips.   https://en.wikipedia.org/wiki/FASTQ_format : Nucleotide sequence and quality score ASCII files. Primary key is Rey Lab ID (in file name).  Each record has it's own file.  All 1056 fastqs are zipped into 9 separate files to make download from BOX possible

fastq_id_link.dat -- link between rey lab ID (1-3) and idpriv (5-10) with a respondent indicator on the end (11).  [g = grad, s = sib, p = grad spouse, e = sib spouse]  idpriv can be used to link to WLS official release phenotypic/survey data.

/food_diary  -- directory with WLS microbiome SAQ (diet/pets/etc...);  Available in .sas7bdat, .dta, .sav, and .rdata. Primary key is idpriv.  Rtype is respondent indicator and matches the linking file.

Genus.txt  -- data file with participants as columns and microbe genus as rows.  Tab delimited.  Primary key is IDPRIV.  Created by code in WLS_data_manipulation.html.

WLS_mothur.html -- A document by Kim Dill-McFarland containing notes and "mothur code for processing the fastq files."

WLS_data_manipulation.html -- A document by Kim Dill-McFarland "describes manipulation of the WLS and microbiota data sets to be used in analysis."

WLS_analysis.html -- A document by Kim Dill-McFarland with notes and R code for the analysis of these data.

SharedVenns.txt -- Tab delimited table with columns for group (sp, sib, unrel), close (4,3,A,B), shared, and venn (A,B).  Seems to be a table created instead of actual Venn diagram showing the overlap between groups as a number...maybe percentage (shared column).  Probably produced by mothurs venn command or something similar.  Though I'm not seeing this referenced in any of the .html files with mothur code.

WLS.final.an.unique_list.0.02.cons.taxonomy -- data file which contains consensus taxonomies for each OTU. Columns are OTU, Size, Taxonomy.  Created by mothur but not explicitly in WLS_mothur.html  Probably renamed manually after code ran.??

WLS.OTU.txt -- dta file with participants in rows and OTU(operational taxonomic unit) number as column.  Created by mothur but not explicitly in WLS_mothur.html  Probably renamed manually after code ran.

WLS.meta.txt  -- data file containing meta data from Coverage and Alpha-diversity sections WLS_mothur.html.  Primary key is IDPRIV. 

WLS.taxonomy.txt -- Taxonomic ranks for each OTU (Otu00001, Otu00002, etc...).  Primary key is OTU number.
