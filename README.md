**Input:**
* **vcf** - file to be annotated, can be compressed,
* **output_name** - output file will be named output_name.vcf,
* **database** - compressed file to annotate with (index is produced within the app).

**Available databses (originally used in this order):**
| Dataset | vcf name | duration (on `test_FBN1.vcf.gz`) | price (on `test_FBN1.vcf.gz`) |
|----|----|----|----|
| clinvar | clinvar.v2.vcf.gz | 0:00:53 | $0.0042 |
| mitomap diseases | mitomap-diseases.vcf.gz | - | - |
| gnomad-exomes | gnomad-exomes-all-populations.vcf.gz | 0:02:39 | |
| gnomad-genomes | gnomad-genomes-all-populations.vcf.gz |
| 1000 genomes | kg.vcf.gz |
| mitomap | mitomap.vcf.gz |
| sift | sift.vcf.gz |
| cadd | cadd.vcf.gz |
| m-cap | m-cap.vcf.gz |
| iseq | iseq-population-frequencies.vcf.gz |

**dx run command**
`dx run iseq_snpsift_annotate -ivcf='test_FBN1.vcf.gz' -ioutput_name='test_FBN1_annotated_clinvar' -idatabase='genetraps-resources:vcf/clinvar.v2.vcf.gz' `
