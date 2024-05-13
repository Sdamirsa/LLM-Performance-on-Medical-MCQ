# Table of Content
- [Project Summary and Aim](#project-summary)
- [Experiment on Gastroenterology Context](#experiment-on-gastroenteorlogy)
  - [Gastroenterology - Data and Design](#gastroenterology---data-and-design)
  - [Gastroenterology - Performance of 20 LLMs](#gastroenterology---performance-of-20-llms)
  - [Gastroenterology - Performance of 4 VLMs](#gastroenterology---performance-of-4-vlms)
- [Live Literature Review](#live-literature-review)
- [Team and Affiliaiton](#team-and-affiliaiton)
- [Contribute and Connect](#contribute-and-connect)


# Project Summary

# Experiment on Gastroenteorlogy

## Gastroenterology - data and design
...This will be published after the paper is published... 

## Gastroenterology - Performance of 20 LLMs
...This will be published after the paper is published... 

## Gastroenterology - Performance of 4 VLMs
...This will be published after the paper is published... 

# Live Literature Review
[LLM's Performance on Medical MCQs](https://docs.google.com/spreadsheets/d/1mYmuju1V_lpf12x297BdbB-hGb5fza07G76aa9Ckn60/edit?usp=sharing)

| Field; Author                    | Dataset                                   | Handling Image-Inclusive Qs          | Evaluation Metrics                                                      | Stratified Performance                                      | Report Quality - Prompt                                                                | Report Quality -Web Use | Report Quality -Model        | Report Quality -Evaluation | llm-performance                                                                                 | human-performance                                                                                |
| -------------------------------- | ----------------------------------------- | ------------------------------------ | ----------------------------------------------------------------------- | ----------------------------------------------------------- | -------------------------------------------------------------------------------------- | ----------------------- | ---------------------------- | -------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Soft Skill; Brin et al.          | 80 soft skill Qs USMLE SA (AMBOSS & NBME) | Excluded                             | • Accuracy<br>• Consistency                                             | None                                                        | Yes (QA followed by "are you sure?")                                                   | Sufficient              | Insufficient                 | Insufficient               | • GPT4: 90%<br>• GPT3.5: 62.5%                                                                  | • Average: 78%                                                                                   |
| USMLE; Gilson et al.             | 100 step 1 USMLE SA (AMBOSS & NBME)       | Excluded                             | • Accuracy<br>• Error source (logic, internal, or external information) | None                                                        | Yes (Just QA)                                                                          | Fully                   | Fully (Dec 15 version)       | Fully                      | • GPT3.5: 56%, 59%, 44%, 42%<br>• InstructGPT: 45%, 54%, 36%, 35%<br>• GPT3: 22%, 19%, 29%, 17% | • Pass: 60%                                                                                      |
| USMLE; Kung et al.               | 367 step 1 USMLE SA (USMLE 2022 SA)       | Excluded                             | • Accuracy<br>• Concordance<br>• Insight                                | None                                                        | Yes (three variants: open-ended, MCQ without justification, MCQ with justification)    | Insufficient            | Fully                        | Fully                      | • GPT3.5: Step 1, 41.2%; Step 2, 49.5%; Step 3, 59.8%                                           | • Pass: 60%                                                                                      |
| Ophthalmology; Moshirifar et al. | 467 medicine SA (StatPearls)              | Images replaced by image description | • Accuracy                                                              | • Difficulty<br>• Sub-category                              | Yes (Just QA)                                                                          | Fully                   | Fully (May 9)                | Insufficient               | • GPT4: 73.2%<br>• GPT3.5: 55.6%                                                                | • Average: 58.1% (\*\*\*\*)                                                                      |
| Ophthalmology; Mihalache et al.  | 125 board SA (OphtoQuestion)              | Excluded                             | • Accuracy                                                              | • Sub-category<br>• Word length                             | Yes (Just QA)                                                                          | Sufficient              | Insufficient (no model name) | Partially Sufficient       | • GPT3.5: 46.4%                                                                                 | NA                                                                                               |
| Ophthalmology; Cai et al.        | 250 board SA                              | Answered without image information   | • Accuracy<br>• Hallucination                                           | • Patient Care Phase<br>• Difficulty                        | Yes (Just QA)                                                                          | Insufficient            | Fully (March 2023)           | Insufficient               | • GPT3.5: 58.8%<br>• GPT4: 71.6%                                                                | • Average: 72.2%                                                                                 |
| Gastroenterology; Suchman et al. | 455 board SA (ACG )                       | Excluded                             | • Accuaracy                                                             | • Sub-category<br>• Difficulty                              | Yes (Just QA)                                                                          | Insufficient            | Fully (March 2023)           | Insufficient               | • GPT3.5: 65.1%<br>• GPT4: 62.4%                                                                | • Pass: 70%                                                                                      |
| Nephrology; Noda et al.          | 99 board SA in Japenese language          | Answered without image information   | • Accuaracy                                                             | • Taxonomy<br>• Sub-category<br>• image-inclusive<br>• Year | Yes (QA + "answer following question")                                                 | Fully                   | Insufficient                 | Insufficient               | • GPT3.5: 31.3%<br>• GPT4: 54.5%<br>• Bard: 32.3%                                               | • 1st year avg: 36.4%<br>• 3nd year avg: 49.5%<br>• 4th year avg: 67.7%                          |
| Cardiology; Skalidis et al.      | 362 board exam (EECC)                     | Excluded                             | • Accuaracy                                                             | \-                                                          | Yes (Just QA)                                                                          | Partially               | Insufficient                 | Partially Sufficient       | • GPT3.5: 58.8%                                                                                 | • Pass: ~60%                                                                                     |
| Dermatology; Passby et al.       | Speciality certificate exam               | Excluded                             | • Accuaracy                                                             | • Sub-category                                              | Yes (Just QA)                                                                          | Insufficient            | Insufficient                 | Insufficient               | • GPT3.5: 63%<br>• GPT4: 90%                                                                    | • Pass: ~70%                                                                                     |
| Plastic Surgery; Humar et al.    | 1129 in-service exam                      | Excluded                             | • Accuracy                                                              | • Year<br>• Sub-category                                    | Yes (Just QA)                                                                          | Fully                   | Insufficient                 | Partially Sufficient       | • GPT3.5: 55.8%                                                                                 | • 1st year: 49 %tile<br>• 2nd year: 13 %tile<br>• 3rd year: 5 %tile<br>• All residents: 12 %tile |
| Otolaryngology; Hoch et al.      | 479 MCQ and 2097 single-choice Board SA   | Excluded                             | • Accuracy                                                              | • Sub-category                                              | Yes (Please answer the following question. Note that only one option is correct: + QA) | Partially               | Sufficient (3 May version)   | Insufficient               | •GPT3.5: 34% on multiple-choice and 57% on single-choice                                        | NA                                                                                               |
| Neurosurgery; Ali et al.         | 149 board SA (SANE)                       | Answered without image information   | • Accuaracy<br>• Hallucination                                          | • Sub-category<br>• Complexity<br>• Word length             | Yes (Just QA)                                                                          | Insufficient            | Fully (March and April 2023) | Insufficient               | • GPT3.5: 62.4%<br>• GPT4: 82.6%<br>• Bard: 44.2%                                               | NA                                                                                               |
| Orthopedic Surgery; Lum et al.   | 212 in-training exam(OITE )               | Excluded                             | • Accuaracy                                                             | • Taxonomy                                                  | Yes (Q + "Select the single best answer" + Options)                                    | Partially               | Insufficient                 | Fully                      | • GPT3.5: 47%                                                                                   | • Pass: 10th percentile (GPT failed)<br>• PGY1: 40th %tile                                       |

*[Last update: April 2024]*

# Team and Affiliaiton
This project was created and is maintained by Seyed Amir Ahmad Safavi-Naini, directed by Ali Soroush and Girish Nadkarni at Mount Sinai Clinical Intelligence Center (MSCIC) and Charles Bronfman Institute for Personalized Medicine at Icahn School of Medicine at Mount Sinai. Special thanks to Bara El-Kurdi for co-directing the Gastroenterology Experiment. 
List of contributors: Zahra Shahhoseini, Sara Rafiee

# Contribute and Connect
We welcome any contribution to expanding this to prepare a benchmark of LLMs in medicine. If you have prepared an MCQ dataset, contact sdamirsa@gmail.com so we can guide you through reproducing the result, generating outputs, and evaluating the answers. Make sure you have the right to use the dataset, beforehand.
In addition, we totally understand our shortcomings and would welcome any refinements to this pipeline.


