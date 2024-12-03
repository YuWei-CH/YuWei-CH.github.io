---
title: "reform"
excerpt: "reform is a python-based command line tool that allows for fast, easy and robust editing of reference genome sequence and annotation files. <br/><img src='/images/reform.png'>"
github: https://github.com/gencorefacility/reform
browser: https://gencore.bio.nyu.edu/reform/
collection: portfolio
---

Execution of reform requires a reference sequence (fasta), reference annotation (GFF or GTF), the novel sequences to be added (fasta), and corresponding novel annotations (GFF or GTF). A user provides as arguments the name of the modified chromosome and either the position at which the novel sequence is inserted, or the upstream and downstream sequences flanking the novel sequences. This results in the addition and/or deletion of sequence from the reference in the modified fasta file. In addition to the novel annotations, any changes to the reference annotations that result from deleted or interrupted sequence are incorporated into the modified gff. Importantly, modified gff and fasta files include a record of the modifications.

Learn more at [reform](https://gencore.bio.nyu.edu/reform/)


