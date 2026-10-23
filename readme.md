## First look at your sequencing data

You just received sequencing data. This short tutorial helps you take a first look at it, shortly after receiving it, and decide one thing: does anything look off? To follow the tutorial, please visit [this website](https://ndombrowski.github.io/sequencing_qc/).

To follow this tutorial you do not need to know the command line. You copy and paste a small number of commands, and you look at a few numbers and one report. You first work through all steps with practice data from a real sequencing run with a real problem, and then repeat them with your own data.

## Why look at your data right away?

Assume you send some data of for sequencing. It often takes some weeks to get the sequencing data back and you have other projects to follow up. Often this means that the data won't get inspected months after receiving it. However, after you finally find time to start your analysis workflow you realize something is wrong, 40% of samples have very few reads and you have to figure out what is going on.

If you wait for a long time inspecting the quality of your sequencing data it can become much harder to figure out what went wrong, or how to fix it. Maybe the PCR products are no longer available, maybe you realize your lab notes are incomplete or the person at the sequencing center who handle the data is gone.

If you look at the read numbers in the first week, the problem would have been visible in five minutes, while it still might be easier to fix a potential issue.

## What you will do

1.  Copy data to Crunchomics, the UvA computer cluster
2.  Count the reads in every sample, and check for samples with far fewer reads than the rest
3.  Make quality reports with FastQC, and look at a few of them in your browser
4.  Decide: everything looks fine, or something needs a closer look. For the second case, the tutorial gives a checklist and says who to contact

I wrote this tutorial for researchers at the Institute for Biodiversity and Ecosystem Dynamics (IBED) at the University of Amsterdam, who can get access to Crunchomics, the Genomics Compute Environment for SILS and IBED. For the command-line basics, it builds on the [Introduction to the CLI workshop](https://ndombrowski.github.io/cli_workshop/) and if you want to know more about how to efficiently deal with large amounts of data.

## License

© 2026 Nina Dombrowski. The text, figures, code and practice data in this repository are licensed under the [Creative Commons Attribution 4.0 International license (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/), see [LICENSE](LICENSE). You are free to share and adapt the material for any purpose, as long as you give appropriate credit and indicate if you made changes.

The practice data (`data/practice_data.tar.gz`) comes from a real amplicon sequencing run and is shared with permission. Each file was reduced to 2% of its reads, and the sample IDs were randomized.

## Use of AI tools

I wrote this tutorial with help from Claude Code (Anthropic), an AI coding assistant. I used it to:

-   draft and restructure the tutorial pages, following an existing CLI tutorial and a style guide that I wrote
-   draft the checklist of what to check when something looks off, which I then reviewed against lab practice
-   keep track of open tasks and check the pages for consistency

I decided on the content, the structure and the teaching approach, and I reviewed every change. Any remaining errors are mine.