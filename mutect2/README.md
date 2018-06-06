# snakebam mutect2
Snakemake pipeline to call SNVs and Indels with Mutect2 pipeline with filtering steps

## sampleConfig.yaml

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
