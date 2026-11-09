# project1-sequence-analysis
Identifying Mutations in NGS Data

**Title & Purpose**
this program analyses DNA sequencing reads against a reference sequence to identify mutations, compare mismatch frequencies between control and treatment groups, and determine whether treatment is associated with increased DNA damage.

**How to run the program How do you open and run it in Colab?** 
Open the notebook from GitHub in Google Colab, click Runtime, Run all (or run cells individually), follow any prompts, and review the generated DNA mutation analysis results and statistics.

**Inputs and outputs.** 

***Input:***
 The program expects DNA sequencing read data that has been processed by the analyse_reads() function. Each read should include details such as sample name, group, validity, mismatch positions, and substitution types.

***Output:***
 The program returns sample-level summaries, mismatch percentages, mutation counts, hotspot positions, and statistical comparisons between control and treatment groups, helping identify whether treatment increases DNA mutations.
 
**Code design**
I divided the program into separate functions, including analyse_reads(), summarise_samples(), and the group comparison function. This made the code more modular and easier to test, as each function performs a specific task. An alternative would have been placing all calculations in a single function, but this would have made debugging more difficult.

I used nested dictionaries to store sample information, such as valid read counts, mismatch statistics, substitution counts, and position counts. This allowed related data to be kept together and accessed efficiently. I considered using multiple lists, but dictionaries made the data easier to organise and summarise.

I also handled samples with no valid reads by setting mismatch_percentage to None and excluding them from statistical analysis to avoid misleading results and division-by-zero errors.

**Testing** 
I tested the program with an empty input list to confirm it returned an empty dictionary without errors. I tested samples containing no valid reads to ensure mismatch_percentage was correctly set to None and excluded from statistical analysis. Finally, I tested reads containing multiple mismatches to verify that one read was counted as a single mismatch-containing read while all mismatch events were counted correctly.
