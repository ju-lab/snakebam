# snakebam mutect2
Snakemake pipeline to call SNVs and Indels with Mutect2 pipeline with filtering steps. 
1. PoN (Panel of Normal) filter
2. Etimate contamination level and filter contaminant reads
3. Potential FFPE/OxoG artifacts. 


## How to configure  sampleConfig.yaml

```yaml
samples:
    '3897':
        tumor_bam: /absolute/or/relative/paths/to/tumour.bam
        normal_bam: /absolute/or/relative/paths/to/tumour.bam
    sample_1229:
        tumor_bam: /absolute/or/relative/paths/to/tumour.bam
        normal_bam: /absolute/or/relative/paths/to/tumour.bam

```
Note: If sample name is a number, such as `3897` as above, you need to make it into a string by using '' 
