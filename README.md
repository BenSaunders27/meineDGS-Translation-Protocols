# MeineDGS Translation Protocols

In this respository, we release translation protocols on meineDGS, a large linguistic sign language dataset. The public meineDGS linguistic corpus can be accessed at [meineDGS](https://www.sign-lang.uni-hamburg.de/dgs-korpus/index.php/welcome.html), containing 330 sequences of free-flowing discourse between two deaf participants, with each around 10 mins in length.  Additionally, detailed spoken language transcripts, frame-level gloss annotations and 2D pose estimation sequences are provided. Discourse is centered around a wide variety of topics, age groups and format, with further details available on the meineDGS website. 

## Translation Protocols

To adapt the mdgs corpus for use as a translation dataset, we segment the free-flowing discourse data into 40,230 segments of German sentences, sign gloss translations and respective sign language videos. Sequence segmentation was performed using spoken language sentence boundaries, with corresponding frame boundaries provided. The title of each segment (e.g. 1583882A-1) contains the title of the original discourse sequence as given in the *Transcript* column (e.g. 1583882), the corresponding participant camera (A or B) and the position of the extracted segment in the original discourse sequence. The start and end frame for each sequence in the video are given at the end, as start|end (e.g. 951|1026).

Table 9 and 10 below show detailed statistics of the meineDGS-V and meineDGS protocols, respectively. Gloss variants used in meineDGS-V give distinction between sign variants, with each containing the same meaning but with differing motion. We chose to retain these variants to provide more challenging baselines for the community. Further public annotation conventions are outlined in [(Konrad, 2018)](https://www.sign-lang.uni-hamburg.de/dgs-korpus/arbeitspapiere/DGS-Korpus_AP03-2018-01v02_en.pdf), which we follow. Additionally, gloss frame alignments are provided as *GLOSS/start-frame/stop-frame* (e.g. BUCHSTABE1/11/34) relative to the start frame of the sequence.

![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS-V_Table.png?raw=true)
![alt text](https://github.com/BenSaunders27/meineDGS-Translation-Splits/blob/main/mDGS_Table.png?raw=true)

Our translation protocols are available as CSV files; **meineDGS_Protocol_Train.csv**, **meineDGS_Protocol_Dev.csv** & **meineDGS_Protocol_Test.csv** for both **\meineDGS** and **\meineDGS-V**. Each CSV file details *filename*, *camera*, *ger\_text*, *gloss*, *start\_time* and *stop\_time* for each split.

## License

To use the meineDGS dataset for computational research, a licence must be obtained from the [University of Hamburg](https://www.sign-lang.uni-hamburg.de/meinedgs/). Release of these protocols does not imply permission of use or provision of a license, with written permission required separately for each user. Please adhere to the data ownership policies and ensure you have the correct rights before use.

For any questions, please reach out to [b.saunders@surrey.ac.uk](b.saunders@surrey.ac.uk)

## Reference

If you use these translation protocols in your research, please cite the following papers:

```
@inproceedings{hanke2010dgs,
    title   =   {{DGS Corpus \& Dicta-Sign: The Hamburg Studio Setup}},
    author  =   {Hanke, Thomas and K{\"o}nig, Lutz and Wagner, Sven and Matthes, Silke},
    booktitle   =   {4th Workshop on the Representation and Processing of Sign Languages: Corpora and Sign Language Technologies (CSLT 2010), Valletta, Malta},
    year    =   {2010}}

@inproceedings{saunders2021signing,
    title   =	{{Signing at Scale: Learning to Co-Articulate Signs for Large-Scale Photo-Realistic Sign Language Production}},
    author  =	{Saunders, Ben and Camgoz, Necati Cihan and Bowden, Richard},
    booktitle   =	{Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
    year    =	{2022}}

```

## Acknowledgements
<sub>We thank Thomas Hanke and University of Hamburg for use of the meineDGS data. </sub>
