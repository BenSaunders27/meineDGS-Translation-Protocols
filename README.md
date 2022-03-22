# meineDGS-Translation-Splits
meineDGS Translation Splits


In this appendix, we provide further details of our released translation protocols on the \acf{mdgs} dataset. The public linguistic dataset, DGS-Korpus, can be accessed at \url{https://www.sign-lang.uni-hamburg.de/meinedgs/ling/start-name_en.html}. DGS-Korpus contains 330 sequences of free-flowing discourse between two deaf participants, each up to 10 mins in length. Discourse is centered around a wide variety of topics, age groups and format, with further details available at \url{https://www.sign-lang.uni-hamburg.de/dgs-korpus/index.php/welcome.html}. To use the \ac{mdgs} dataset, permission must be obtained from University of Hamburg \footnote{\url{thomas.hanke@uni-hamburg.de}}. Release of these protocols does not imply permission of use, with permission required separately for each user of this dataset.

 We segment the free-flowing discourse data into 40,230 segments of German sentences, sign gloss translations and respective sign language videos. Sequence segmentation was performed using spoken language sentence boundaries, with corresponding frame boundaries provided. The title of each segment (e.g. 1583882A-1) contains the original discourse title as given in the \textit{Transcript} column (e.g. 1583882), the corresponding participant camera (A or B) and the position of the extracted sequence in the original discourse. The translation protocols are publicly available at \url{https://github.com/BenSaunders27/meineDGS-Translation-Splits}, detailing \textit{filename}, \textit{camera}, \textit{ger\_text}, \textit{gloss}, \textit{start\_time} and \textit{stop\_time}.


Table \ref{tab:mDGSv_Stats} and \ref{tab:mDGS_Stats} show detailed statistics of the \ac{mdgsv} and \ac{mdgs} protocols, respectively. Gloss variants used in \ac{mdgsv} give distinction between sign variants, with each containing the same meaning but with differing motion. We chose to retain these variants to provide more challenging baselines for the community. Further public annotation conventions are outlined in \cite{konrad2018public}, which we follow. Additionally, gloss frame alignments are provided as \textit{GLOSS/start-frame/stop-frame} (e.g. BUCHSTABE1/11/34) to enable further research into \ac{cslr}.


![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS-V_Table.png?raw=true)
![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS_Table.png?raw=true)

