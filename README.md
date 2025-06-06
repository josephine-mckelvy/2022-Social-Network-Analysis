# Social Network Analysis
code from Jeffrey Smith for analyzing coauthorship networks and topic modeling for publications in the Rapid Acceleration of Diagnostics for Underserved Populations (RADx-UP) initiative
(graphical ReadMe here: https://miro.com/app/board/uXjVPuznJ_k=/?share_link_id=474547388392)

# Purpose:
to store datasets and R code for social network analysis of coauthorships and content analysis of manuscript topics for RADx-UP publications

# Inputs:
  + author affiliations (e.g., organization names & types) (.xlsx)
  + publication lists (e.g., citation meta data) (.xlsx)
  + content analysis datasets from REDCap (e.g., research topics, methods, findings)(.xlsx)

# Outputs:
  + adjacency matrix of all coauthorship connections
  + edge list of senders and receivers in coauthorships
  + igraphs of the sociograms to show strength of ties and diversity of networks
  + cluster graph from multiple correspondence analysis by COVID-19 testing or vaccine uptake (Y-axis) and clinical or community engagement focus (X-axis)

# Data Collection & Visualization
1. Gather citation metadata and other information on scholarly products (e.g., journal articles, conference papers, and grants) from:
  -automated searches of RADx-UP grant numbers (in PubMed, Scopus) 
  -quarterly publications tracking surveys (to RADx-UP project leads)
  -n=70 publications
2. Categorize information from publications (e.g., target populations, study settings, study design, analytic methods, results, Translationsal Science benefits) via data entry into a REDCap survey instrument.
  -2 reviewers independently conduct this content analysis for each publication.
  -a third arbiter resolves differences between these independent reviews of each publication.
3. Clean datasets for missingness and merge data to generate adjacency matrix, edge list for igraphs.
4. Visualize social networks of coauthorship and clusters of publication topics.   
