**Input:**
* **vcf** - file to be annotated, can be compressed,
* **output_name** - output file will be named output_name.vcf,
* **database** - compressed file to annotate with (index is produced within the app).


**Available databses (originally used in this order):**

| Dataset | vcf name | duration* | price* |
|----|----|----:|----:|
| clinvar | clinvar.v2.vcf.gz | 0:00:53 | $0.0042 |
| mitomap diseases | mitomap-diseases.vcf.gz | - | - |
| gnomad-exomes | gnomad-exomes-all-populations.vcf.gz | 0:02:39 | $0.0127 |
| gnomad-genomes | gnomad-genomes-all-populations.vcf.gz |0:27:26 |$0.1308|
| 1000 genomes | kg.vcf.gz | 0:02:51 | $0.0136|
| mitomap | mitomap.vcf.gz |0:00:50|$0.0039|
| sift | sift.vcf.gz |0:03:14|$0.0155|
| cadd | cadd.vcf.gz |
| m-cap | m-cap.vcf.gz |0:01:30|$0.0072|
| iseq | iseq-population-frequencies.vcf.gz |0:00:48|$0.0039|


*on `test_FBN1.vcf.gz` (previous version without producing file `*_annotate_log.txt`)


**dx run command**

`dx run iseq_snpsift_annotate -ivcf='test_FBN1.vcf.gz' -ioutput_name='test_FBN1_annotated_clinvar' -idatabase='genetraps-resources:vcf/clinvar.v2.vcf.gz' `
