# Day 12 — Galaxy QC → Trim → Assembly → QUAST

## Sample
- sampleID: W
- raw data: (Downloaded off class modules / dataset 12)

## Tools (Galaxy / usegalaxy.org)
- FastQC: VERSION .74+galaxy1
- fastp: VERSION 1.1.0+galaxy0
- SPAdes: VERSION 4.2.0+galaxy0
- QUAST: VERSION 5.3.0+galaxy1

## Steps
1. FastQC on raw reads → saved report as: Wforward_fastqc.html
2. fastp trimming (default settings) → saved report as: Wfasttrimmerreport.html
3. FastQC on trimmed reads → saved report as: Wfastptrimmerreport.html
4. SPAdes assembly on trimmed reads → saved contigs as: W_spadesasemlycontigs.fasta
5. QUAST evaluation on contigs → saved report as: W_quast_report.pdf

## Notes / interpretation
- (1–3 bullets on what changed after trimming)
- (1–3 bullets on what QUAST suggests about contiguity)