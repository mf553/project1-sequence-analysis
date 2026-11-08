# project1-sequence-analysis
Identifying Mutations in NGS Data

##Title & Purpose What does your program do, and what biological question does it address? (~30 words)
his program analyses DNA sequencing reads against a reference sequence to identify mutations, compare mismatch frequencies between control and treatment groups, and determine whether treatment is associated with increased DNA damage.

##How to run the program How do you open and run it in Colab? (~30 words)
Open the notebook from GitHub in Google Colab, click Runtime, Run all (or run cells individually), follow any prompts, and review the generated DNA mutation analysis results and statistics.

##Inputs and outputs. What input does it expect? What results does it return or display? (~60 words)
###Input:
 The program expects DNA sequencing read data that has been processed by the analyse_reads() function. Each read should include details such as sample name, group, validity, mismatch positions, and substitution types.

###Output:
 The program returns sample-level summaries, mismatch percentages, mutation counts, hotspot positions, and statistical comparisons between control and treatment groups, helping identify whether treatment increases DNA mutations.
Code design: Explain 2-3 specific decisions (beyond the project specifications) that you made and why. For example: how you divided work between functions, chose data structures, or handled invalid reads. What alternatives did you consider? (120 words)

Testing: Describe three informative tests that you ran to check the correctness or robustness your code. (60 words)
