# base unreleased

## BREAKING CHANGES

* Change default `multiple_sep` to `;` (PR #25). This aligns with an upcoming breaking change in
  Viash 0.9.0 in order to avoid issues with the current default separator `:` unintentionally
  splitting up certain file paths.

## NEW FEATURES

* `arriba`: Detect gene fusions from RNA-seq data (PR #1).

* `fastp`: An ultra-fast all-in-one FASTQ preprocessor (PR #3).

* `busco`: 
    - `busco/busco_run`: Assess genome assembly and annotation completeness with single copy orthologs (PR #6).
    - `busco/busco_list_datasets`: Lists available busco datasets (PR #18).
    - `busco/busco_download_datasets`: Download busco datasets (PR #19).

* `featurecounts`: Assign sequence reads to genomic features (PR #11).

* `bgzip`: Add bgzip functionality to compress and decompress files (PR #13).

* `pear`: Paired-end read merger (PR #10).

* `lofreq/call`: Call variants from a BAM file (PR #17).

* `lofreq/indelqual`: Insert indel qualities into BAM file (PR #17).

* `multiqc`: Aggregate results from bioinformatics analyses across many samples into a single report (PR #42).

* `star/star_align_reads`: Align reads to a reference genome (PR #22).

* `gffread`: Validate, filter, convert and perform other operations on GFF files (PR #29).  

* `salmon`:
    - `salmon/salmon_index`: Create a salmon index for the transcriptome to use Salmon in the mapping-based mode (PR #24).
    - `salmon/salmon_quant`: Transcript quantification from RNA-seq data (PR #24).

* `samtools`:
    - `samtools/samtools_flagstat`: Counts the number of alignments in SAM/BAM/CRAM files for each FLAG type (PR #31).
    - `samtools/samtools_idxstats`: Reports alignment summary statistics for a SAM/BAM/CRAM file (PR #32).
    - `samtools/samtools_index`: Index SAM/BAM/CRAM files (PR #35).
    - `samtools/samtools_sort`: Sort SAM/BAM/CRAM files (PR #36).
    - `samtools/samtools_stats`: Reports alignment summary statistics for a BAM file (PR #39).
    - `samtools/samtools_faidx`: Indexes FASTA files to enable random access to fasta and fastq files (PR #41).
    - `samtools/samtools_collate`: Shuffles and groups reads in SAM/BAM/CRAM files together by their names (PR #42).
    - `samtools/samtools_view`: Views and converts SAM/BAM/CRAM files (PR #48).
    - `samtools/samtools_fastq`: Converts a SAM/BAM/CRAM file to FASTQ (PR #52).

* `falco`: A C++ drop-in replacement of FastQC to assess the quality of sequence read data (PR #43).


## MAJOR CHANGES

## MINOR CHANGES

* Uniformize component metadata (PR #23).

* Update to Viash 0.8.5 (PR #25).

* Update to Viash 0.9.0-RC3 (PR #51).

## DOCUMENTATION

## BUG FIXES

* Add escaping character before leading hashtag in the description field of the config file (PR #50).

* Format URL in biobase/bcl_convert description (PR #55).