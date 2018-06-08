# snakebam mutect2
Snakemake pipeline to call SNVs and Indels with Mutect2 pipeline with filtering steps

# How to run
Type in the following command in the directory where Snakefile is located. 
```bash
$ snakemake -p done --profile profile
```

## sampleConfig.yaml

```yaml
samples:
    '3897':
        tumor_bam: /absolute/or/relative/paths/to/this/tumor.bam
        normal_bam: /absolute/or/relative/paths/to/this/normal.bam
    sample_1229:
        tumor_bam: /absolute/or/relative/paths/to/that/tumor.bam
        normal_bam: /absolute/or/relative/paths/to/that/normal.bam

```
Note: If sample name is a number, such as `3897` as above, you need to make it into a string by using '' 
