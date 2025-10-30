# cda_ptsd311

Project for analysis of study 311 data using Rawls et al, alcohol paper
analysis approach.

For privacy, data is store in BoxDrive at BoxDrive/311_Rawls_analysis


The clinical measures that are included are the MADRS (depression symptoms scale), the PSSI5 (PTSD symptom scale), Ruminative Response Scale (RRS), CAPS-5 (PTSD symptom scale), 

Cognitive testing measures include Dot counting, 1-back, 2-back, Set shifting task, Flanker task, Executive Function composite score, Cognitive Control composite score, and Working Memory composite score. 

For the PSSI5 and CAPS5 scales, I have also included PTSD subcluster scores (INT=intrusion sx; AVO=avoidance sx; COGMOOD=cognition and mood sx; ARO=hyperarousal sx). 

For the RRS, I also included subscales for Brooding, Depressive rumination, and Reflective rumination.

For each of these scales, I have included Pre-infusion scores, Post-infusion scores, and a Pre-Post Delta score. 

I also made separated datasets on different tabs for participants that received ketamine and participants that received placebo, in case you wanted to easily look at either group separately.

This is probably more data than you need but I thought I would get you all of the relevant outcome data that I have.

Also, I have been using the PSSI5 scores for PTSD outcomes as this scale was collected closer to each infusion than the CAPS5 and showed more robust treatment effects than the CAPS5. For completeness, however, I included CAPS5.

## Getting grid data for study 311

Here is how to retrieve events and procedures for study 311 and storing them into json files.

Code can be found here: https://github.com/kelvinlim/grid_api/releases 

```
(base) kolim@Kelvins-Mac-Studio grid_api % ~/bin/gridapi-macos-1.0.7 studies events 311 --format json > ~/BoxDrive/311_Rawls_analysis/events.json              
(base) kolim@Kelvins-Mac-Studio grid_api % ~/bin/gridapi-macos-1.0.7 studies procedures 311 --format json > ~/BoxDrive/311_Rawls_analysis/procedures.json
(base) kolim@Kelvins-Mac-Studio grid_api % 
```
