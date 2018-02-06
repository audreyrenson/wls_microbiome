* Documentation for CUNY phenotypic data folder
(All .dta files were saved as Stata version 12)

Census_1940_PARTIAL.dta
unique id is idpriv & rtype
n=153
As the 1940 census data are still being cleaned this file contains the measures for 153 of the grads.  When the data are complete we hope to have 1940 census data for ~90% of the 188 grads in the mibi sample.  Note that this is a marker of the location of the grads in 1940.  For the grads this will be very early in their life, and in a few cases before they were born. I do not match these data to the full siblings of the grads.  I think you can use these measures for the sibling data as long as you aee careful in noting the age of the sibling in 1940. Some of the siblings in the WLS may not have lived in that location in 1940.  Many were not born and for those that were alive the family may have lived somewhere else.

CUNY_October_2017_MiBiSAQ_Intak_CASES.dta
unique id is idpriv & rtype
n=431
Measures from the MiBi SAQ, the intake data from UWSC (information on the sample when it came to the Survey Center), and the CASES instrument (answwers to in-person questions when the interviewer visited participants to invite them to the study).  THIS FILE CONTAINS THE INFORMATION THAT THE PARTICIPANT RECORDED IN THE FOOD DIARY.  This file REPLACES all the files previously shared in that directory.

CUNY_October_2017_Survey.dta
unique id is idpriv & rtype
n=431
The complete WLS survey data from the 431 participants in the mibi sample.  This is mainly the public version of the data with a few exceptions.  First the id uses idpriv so it can be matched to the mibi data.  It adds these additional variables that are not in the survey data.
1) is_spouse  Use this variable to quickly identify the 100 spouses in the mibi sample.  These 100 cases will have missing measures on all the survey data.  If you want information that the spouses provided directly in the 200X spouse interview please talk to Carol Roan
2) hasmibisib  This variable equals one if the participant and their sibling are BOTH a part of the mibi project.  You can link the grad/sib pairs by using the measure familypriv. 
3) hasspouse  This variable equals one if the participant's spouse is also in the mibi data.  Spouse pairs have the same value of idpriv and you can link them using rtype.
* g = grad
* s= sib
* e = sib spouse
* p= grad spouse

R3/4/5_Geocodes.dta
These files contain only the geocodes for the requested round of data.  There is no unique id.  Attach the characteristics of the place to these files and Carol Roan will match them to the individuals in the mibi project.
