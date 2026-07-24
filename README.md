# 🔬 Quality Control of NGS Sequencing Data using Galaxy

## 📖 Overview

This tutorial focuses on the **quality assessment of FASTQ sequencing files** using the **Galaxy** platform. Quality control (QC) is a critical first step in any Next-Generation Sequencing (NGS) workflow, ensuring that sequencing data is reliable before performing downstream analyses such as **RNA-Seq**, **ChIP-Seq**, **Whole Genome Sequencing (WGS)**, or other OMICS studies.

By evaluating sequence quality early in the workflow, potential issues such as low-quality reads, sequencing biases, adapter contamination, and overrepresented sequences can be identified and corrected.

---

## 🎯 Objectives

- Assess the quality of raw FASTQ files
- Identify potential sequencing issues
- Understand common quality metrics
- Prepare sequencing data for downstream analyses
- Learn best practices for NGS quality control

---

## 🔬 Quality Control Workflow

The standard quality control process for NGS data includes:

```text
Raw FASTQ Files
       │
       ▼
Quality Assessment
       │
       ▼
Identify Low-Quality Reads
       │
       ▼
Adapter Trimming & Filtering
       │
       ▼
High-Quality Reads
       │
       ▼
Downstream Analysis
(RNA-Seq • ChIP-Seq • Variant Calling • Genome Assembly)
```

---

## 🛠️ Quality Assessment Tools

Depending on the sequencing technology, different quality control tools can be used.

| Sequencing Data | Tool | Purpose |
|-----------------|------|---------|
| 📄 Short Reads | **FASTQE** | Quick quality assessment of short-read sequencing data |
| 📄 Short & 📏 Long Reads | **FastQC** | Comprehensive sequencing quality analysis |
| 📏 Long Reads | **NanoPlot** | Quality assessment and visualization of long-read sequencing data |
| 🧬 Oxford Nanopore | **PycoQC** | Sequencing run quality analysis for Nanopore data |

---

## ✂️ Read Trimming & Filtering

After quality assessment, low-quality regions and sequencing adapters can be removed using:

- **Cutadapt** – Adapter trimming and quality filtering for short-read sequencing data

This step improves data quality and increases the reliability of downstream analyses.

---

## 📊 Applications

Quality control is an essential preprocessing step for many bioinformatics workflows, including:

- 🧬 RNA-Seq
- 🧪 ChIP-Seq
- 🌍 Whole Genome Sequencing (WGS)
- 🧫 Whole Exome Sequencing (WES)
- 🧬 Variant Calling
- 🦠 Metagenomics
- 🔬 Other OMICS analyses

---

## 🎓 Learning Outcomes

Through this tutorial, I learned how to:

- Evaluate the quality of raw FASTQ files
- Interpret sequencing quality metrics
- Detect common sequencing issues
- Select appropriate QC tools based on sequencing technology
- Prepare high-quality datasets for downstream bioinformatics analyses
- Perform reproducible quality control workflows using Galaxy
