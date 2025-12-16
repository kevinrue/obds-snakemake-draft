Repository used to draft materials for an [OBDS][obds] 1-day lesson about [Snakemake][snakemake].

## Background

The Oxford Biomedical Data Science (OBDS) Training Programme delivers training in the skills and methods required for the analysis and interpretation of large-scale biomedical datasets, particularly genomic and functional genomic data.
Read more [here][obds].

The Snakemake workflow management system is a tool to create reproducible and scalable data analyses.
Read more [here][snakemake].

## How to use

Run the workflow with:

```bash
snakemake --executor slurm --jobs 4 --printshellcmds
```

`--executor slurm` is optional but tells the workflow to submit jobs to the Slurm job manager installed on the training server.

`--jobs 2` is optional but controls the maximal number of jobs that the workflow can submit concurrently.

`--printshellcmds` is optional but tells the workflow to display the command being run by each job (very useful for debugging!).


[obds]: https://www.imm.ox.ac.uk/research/units-and-centres/mrc-wimm-centre-for-computational-biology/training/oxford-biomedical-data-science-training-programme
[snakemake]: https://snakemake.readthedocs.io/en/stable/

