# meineDGS-Translation-Splits

In this respository, we release translation protocols on meineDGS (mDGS), a large linguistic sign language dataset. The public dataset, mDGS, can be accessed at [mDGS](https://www.sign-lang.uni-hamburg.de/dgs-korpus/index.php/welcome.html), containing 330 sequences of free-flowing discourse between two deaf participants, each up to 10 mins in length. Additionally, detailed spoken language transcripts and frame-level gloss annotations are provided. Sign language discourse is centered around a wide variety of topics, age groups and format, with further details available on their website. To use the \ac{mdgs} dataset, permission must be obtained from the [University of Hamburg](thomas.hanke@uni-hamburg.de). Release of these protocols does not imply permission of use, with written permission required separately for each user. Please adhere to the data ownership policies and ensure you have the right to download this data before use.

To adapt mdgs for use as a translation dataset, we segment the free-flowing discourse data into 40,230 segments of German sentences, sign gloss translations and respective sign language videos. Sequence segmentation was performed using spoken language sentence boundaries, with corresponding frame boundaries provided. The title of each segment (e.g. 1583882A-1) contains the original discourse title as given in the *Transcript* column (e.g. 1583882), the corresponding participant camera (A or B) and the position of the extracted sequence in the original discourse. 
 
Our translation protocols are available as CSV files; **mDGS_Protocol_Train.csv**, **mDGS_Protocol_Dev.csv** & **mDGS_Protocol_Test.csv**, detailing *filename*, *camera*, *ger\_text*, *gloss*, *start\_time* and *stop\_time* for each split.

Table 9 and 10 below show detailed statistics of the mDGS-V and mDGS protocols, respectively. Gloss variants used in mDGS-V give distinction between sign variants, with each containing the same meaning but with differing motion. We chose to retain these variants to provide more challenging baselines for the community. Further public annotation conventions are outlined in \cite{konrad2018public}, which we follow. Additionally, gloss frame alignments are provided as *GLOSS/start-frame/stop-frame* (e.g. BUCHSTABE1/11/34).


![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS-V_Table.png?raw=true)
![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS_Table.png?raw=true)


Citation


