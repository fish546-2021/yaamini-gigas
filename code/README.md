# code

Shell and R Markdown scripts used to examine methylation data. All scripts are sorted into two folders: [Haws (Hawai'i diploid and triploid ctenidia samples)](https://github.com/RobertsLab/project-oyster-oa#changes-in-dna-methylation-in-diploid--triploid-crassostrea-gigas-exposed-to-different-ph-levels-id-haws) and [Manchester (Washington diploid gonad samples)](https://github.com/RobertsLab/project-oyster-oa#pacific-oyster-ocean-acidification-trials-at-chew-hatchery-id-manchester).

## Haws

- [01-trimgalore.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Haws/01-trimgalore.sh): Shell script used on `mox` to trim adapter sequences out of data
- [02-bismark.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Haws/02-bismark.sh): Shell script used on `mox` to align sequences to bisulfite-converted genome and extract methylation information

## Manchester

- [01-fastqc.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Manchester/01-fastqc.sh): Mox script used to assess raw data quality
- [02-trimgalore.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Manchester/02-trimgalore.sh): Mox script used to trim adapter sequences out of data
- [03-fastqc.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Manchester/03-fastqc.sh): Mox script used to assess trimmed data quality after [`fastqc`](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/) did not run successfully within `trimgalore`
- [04-bismark.sh](https://github.com/fish546-2021/yaamini-gigas/blob/main/code/Manchester/04-bismark.sh): Mox script to align sequences to bisulfite-converted genome and extract methylation information
