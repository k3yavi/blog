---
layout:     post
title:      "Genomics: RNA-seq"
subtitle:   ""
date:       2015-02-25 14:33:00
author:     "Avi Srivastava"
header-img: "img/post-bg-04.jpg"
---

<p>
	RNA-seq:
	* Collection of experimental and computational methods to determine the identity and abundance of RNA sequences.
	* derived from generational changes from sequencing technology like first and second generation.

	First Generation:
	* Called as Sanger dideoxy sequencing.
	* Use electrophoresis to get nucleic acid fragment length.
	* Standard sequence length was 600-1k bases

	Second Generation:
	* Called as NGS (Next Generation Sequencing)
	* Run in parallel format, so single run can give sequence of millions
	* A standard was 6000M sequencing reaction of 100 nucleotide give 600 billion bases sequence

	Third Generation:
	* Similar to second but use template individual molecule of DNA.
	* Fewer Sequencing reactions the previous in few millions 
	* Length of sequence per reaction is increased to around 1500 nucleotide.

	Difference from older Micro arrays or WHY RNA-seq:
	* RNA-seq has high throughput
	* Higher Sensitivity
	* Ability to discover new transcripts, gene models, and small noncoding RNA species.
	* Difference in level of gene expression in normal and infected cells.
	* How gene splicing changes in different events.
	* General Annotation of gene from single to human cells was quite poor

	Abbreviations:
	SR50: Single Read 50 nucleotide
	PE100: Paired end 100 nucleotide

	RNA-seq Platforms:
	Illumina:
	* Cluster Generation: Many copies of cDNA are formed
	* Sequence by synthesis: Reaction where in each synthesis round, the addition of a single nucleotide is determined by a fluorescent signal, is imaged, to get the location and type of nucleotide to give nucleotide sequence.
	* Modes: SR and PE . PE100 can give 6 billion paired end read in single run to give 600 Gb of data.
	* 8.5 Gb data in 2 day
	SOLID:
	* Promoted by Applied Biosystems
	* Used ligation instead of synthesis
	* highly accurate due to two check of nucleotide
	* very useful to detect SNP
	Roche 454:
	* also on synthesis methods
	* Use pyrosequencing advantage of longer reads up to 1000 bases.
	 * can give 1M reads per run with avg 700 nt per read and 700Mb in less then one day.
	Ion Torrent:
	* New platform uses adaptor ligated library followed by seq by synthesis.
	* Instead fluorescent signal it detect changes in pH of solution when nulceotide is added.
	* Biggest advantage of low cost affordable sequencer.
	* Powered down when not in use and resumed
	* 60-80M reads at 200 bases per reads with 10 Gb of data in 2-4h
	Pacific Bioscience:
	* Third Generation platform.
	* sequence by synthesis
	* Real time very fast sequencer
	* Avg 5k nt. in 1-2 hours
	Nanopore Technologies:
	* Third generation sequencing
	* Simple leads to small platform device size as small as Usb stick
	* Technically challenged due to measurement of small changes in current.

	Remember:

	* The collection of exons and introns that make up a gene is called a gene model. 

	* we should keep in mind that we can compensate for low accuracy by having more reads. 


	Reference:
	All the thoughts are from book:
	http://www.amazon.com/RNA-seq-Data-Analysis-Mathematical-Computational/dp/1466595000
</p>