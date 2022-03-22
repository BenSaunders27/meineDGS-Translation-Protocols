# meineDGS-Translation-Splits
meineDGS Translation Splits


In this appendix, we provide further details of our released translation protocols on the \acf{mdgs} dataset. The public linguistic dataset, DGS-Korpus, can be accessed at \url{https://www.sign-lang.uni-hamburg.de/meinedgs/ling/start-name_en.html}. DGS-Korpus contains 330 sequences of free-flowing discourse between two deaf participants, each up to 10 mins in length. Discourse is centered around a wide variety of topics, age groups and format, with further details available at \url{https://www.sign-lang.uni-hamburg.de/dgs-korpus/index.php/welcome.html}. To use the \ac{mdgs} dataset, permission must be obtained from University of Hamburg \footnote{\url{thomas.hanke@uni-hamburg.de}}. Release of these protocols does not imply permission of use, with permission required separately for each user of this dataset.

 We segment the free-flowing discourse data into 40,230 segments of German sentences, sign gloss translations and respective sign language videos. Sequence segmentation was performed using spoken language sentence boundaries, with corresponding frame boundaries provided. The title of each segment (e.g. 1583882A-1) contains the original discourse title as given in the \textit{Transcript} column (e.g. 1583882), the corresponding participant camera (A or B) and the position of the extracted sequence in the original discourse. The translation protocols are publicly available at \url{https://github.com/BenSaunders27/meineDGS-Translation-Splits}, detailing \textit{filename}, \textit{camera}, \textit{ger\_text}, \textit{gloss}, \textit{start\_time} and \textit{stop\_time}.


Table \ref{tab:mDGSv_Stats} and \ref{tab:mDGS_Stats} show detailed statistics of the \ac{mdgsv} and \ac{mdgs} protocols, respectively. Gloss variants used in \ac{mdgsv} give distinction between sign variants, with each containing the same meaning but with differing motion. We chose to retain these variants to provide more challenging baselines for the community. Further public annotation conventions are outlined in \cite{konrad2018public}, which we follow. Additionally, gloss frame alignments are provided as \textit{GLOSS/start-frame/stop-frame} (e.g. BUCHSTABE1/11/34) to enable further research into \ac{cslr}.

```{=latex}

\begin{table}[t!]
\centering
\resizebox{1\linewidth}{!}{%
\begin{tabular}{@{}p{1.6cm}|ccc|ccc@{}}
\toprule
\multicolumn{1}{c}{} & \multicolumn{3}{c}{Sign Gloss} & \multicolumn{3}{c}{German} \\
           & Train   & Dev    & Test   & Train  & Dev   & Test  \\  \midrule
segments   & 40,230 &  4,996 & 4,977 & \multicolumn{3}{c}{$\xleftarrow{\rule{2.0cm}{0pt}}same$} \\
frames     & 6,146,153 & 764,451 & 758,883 & \multicolumn{3}{c}{$\xleftarrow{\rule{2.0cm}{0pt}}same$} \\
vocab.     & 10,042 & 4,644 & 4,620 & 18,680  & 6,224  & 6,231  \\
tot. words & 215,392 & 26,855 & 26,969 & 389,427 & 48,376 & 48,551 \\
tot. OOVs  & - & 371 & 339 & - & 1,103 & 1,171 \\
singletons & 2,681 & - & -  & 8,909 & - & - \\
\bottomrule
\noalign{\smallskip} 
\end{tabular}}
\caption{Key statistics of the \acf{mdgsv} dataset split.}
\label{tab:mDGSv_Stats}
\end{table}

\begin{table}[t!]
\centering
\resizebox{1\linewidth}{!}{%
\begin{tabular}{@{}p{1.6cm}|ccc|ccc@{}}
\toprule
\multicolumn{1}{c}{} & \multicolumn{3}{c}{Sign Gloss} & \multicolumn{3}{c}{German} \\
           & Train   & Dev    & Test   & Train  & Dev   & Test  \\  \midrule
segments   & 40,230 &  4,996 & 4,977 & \multicolumn{3}{c}{$\xleftarrow{\rule{2.0cm}{0pt}}same$} \\
frames     & 6,146,153 & 764,451 & 758,883 & \multicolumn{3}{c}{$\xleftarrow{\rule{2.0cm}{0pt}}same$} \\
vocab.     & 4,337 & 2,490 & 2,487 & 18,680  & 6,224  & 6,231  \\
tot. words & 215,392 & 26,855 & 26,969 & 389,427 & 48,376 & 48,551 \\
tot. OOVs  & - & 118 & 112 & - & 1,103 & 1,171 \\
singletons & 778 & - & -  & 8,909 & - & - \\
\bottomrule
\noalign{\smallskip} 
\end{tabular}}
\caption{Key statistics of the \acf{mdgs} dataset split.}
\label{tab:mDGS_Stats}
\end{table}

```

![alt text](https://https://github.com/BenSaunders27/meineDGS-Translation-Splits/edit/main/nocenter.jpg?raw=true)
