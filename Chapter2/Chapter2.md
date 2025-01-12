### Introduction
#### Document Purpose
The key purpose of the Requirements Definition is to record the mid-level and detailed requirements for the project and express these from the perspective of an end-user goal. i.e. a User Story.  

#### Target Audience
All business and IT stakeholders.

### Business Context, Scope and High-Level Requirements
The following items are recorded and baselined in the Scope Definition document and not duplicated here:

- Project Background
- Problem/Opportunity Statement
- Business Objectives
- Critical Success Factors
- Drivers and Constraints
- Definition of Scope
- High Level Requirements (Functional and Non-Functional)

### Business Process Model
The Business Process Model covers the proposed processes to ensure a common understanding among all stakeholders and covers the whole project scope, including those aspects that are not expected to have an IT solution.  This enables any additional area that might require an IT solution to be identified.

The main section includes a number of requirements artefacts that span across the in-scope processes:

Business Process Scope Diagram – a visual representation of the business processes in scope of the project and the associated ‘actors’ who will be interacting with these processes;

![Business process](https://user-images.githubusercontent.com/45914355/82267568-ac9d7100-9964-11ea-8467-1d1423c6093d.png)

Business Event – This change will be driven by the development of an algorithm to summarise and paraphrase medical trials (as published within medical journals), and present the output as a snapshot utilising social media.  This will provide a validated and authoritative stance on health and medical issues, which will be presented in a straight-forward and engaging manner. 


### Actors

|Actor <img width=75/>|	Description <img width=725/>|
|---|---|
|Users |	New or existing users who wish to view contemporary, succinct, and evidence-based health information. |

### Process
#### Current Process
HillsHealth.org was the original development completed in 2012.  The manual process of creating the summarised reviews was labour intensive, and the lack of any SEO or social media presence has meant that traffic has remained low.  

#### Proposed Process (draft)

![Process Overview](https://user-images.githubusercontent.com/45914355/85082902-22953200-b1c8-11ea-8064-19a9aff0e8e7.png)

|Step <img width=300/>|Notes <img width=500/>|
|---|---|
|1. Define the question|Topical, of interest, triggered from GP data analysis|
|2. Plan eligibility criteria|What intervention are your searching for and for which issue/population?|
|3. Search for studies with filter|Pubmed API/PubMed Central/Embase using question, MeSH terms, eligibility (2002 onwards, human trials, relevant study types)|
|4. Tabulate characteristics of most relevant trials to question|See 'Return the following…' below.  Max = 100|
|5. Score the abstracts/papers, append result to table and sort|See 'Score based on…' below, add score to table and sort by score.|
|6. Review output and draw conclusions|Manually review results and draw a conclusion to the original question|
|7. Create visual to answer question|Produce a visualisation that answers the original question|

|Topic <img width=75/>|Return the following… (return as columns with 1 row per paper). *Italics may require full access* <img width=725/>|
|---|---|
|Title|Title of paper|
|Objective|Objective of the study (or first 2 scentances of abstract if not stated)|
|Participants|What age, sex and disease severity/co-morbidity, where did they come from/live, ethnicity, socio-demographic?|
|Outcomes|Confidence interval and risk ratio/odds ratio/Number needed to treat (dichotomous data), mean difference/standardised mean difference (continuous data)|
|Conclusion|Appendix Conclusion (or last 2 scentances)|
|Conclusion|Plain language summary (if available)|
|Reference|doi|
|Reference|Keywords|

|Topic <img width=75/>|	Score based on… <img width=650/>|	Score <img width=75/>|
|---|---|---|
|Journal|	What is the journal impact factor?  Scopus.com / clarivate.com||	
|Study|	Is the paper described as a Systematic review of randomly controlled trials / RCT?|	0 (EXCLUDE)|
|Study|	Is the paper described as a Randomly controlled trial?||	
|Study|	Is the paper described as a systematic review of cohort studies?|	0 (EXCLUDE)|
|Study|	Is the paper described as a Cohort study / longitudinal?||	
|Study|	Is the paper described as a Consensus statement?||	
|Study|	Is the paper described as a Systematic review of case control studies?|	0 (EXCLUDE)|
|Study|	Is the paper described as a Case-control study?||	
|Study|	Is the paper described as Expert opinion / cross-sectional survey / case report / case series?||	
|Paper|	What is the number of participants/patients/subjects?||	
|Paper|	*Is the study described as randomised?*||	
|Paper|	*Is the study described as blind / double blind?*||	
|Bias|	*Does the paper describe those who withdrew / dropped out?*||	
|Bias|	*Does the paper list a conflict of interest?*||	
|Bias|	*Was the study listed on a trial register/clinical trials?*||	

|Topic <img width=75/>|	Not returned at this time… <img width=725/>|
|---|---|
|Participants|	*How were the participants recruited?*|
|Participants|	*How were the participants allocated/randomised?*|
|Participants|	*Setting – outpatient/hospitalized.*| 
|Participants|	*Who was included/excluded from the study?*|
|Intervention|	*What treatment or other intervention was offered or was it only compared to a placebo?*|
|Intervention|	*Frequency/duration of the intervention?*|
|Outcomes|	*What outcome measure(s) were used?*|
|Outcomes|  *Type or frequency of adverse reactions?*|
|Outcomes|	*Was follow-up complete enough (or response rate if survey)?*|

### Requirements Statements

![Req1 1](https://user-images.githubusercontent.com/45914355/82155372-6238c900-986c-11ea-834a-6293c2afd0d0.png)

![Req1 22](https://user-images.githubusercontent.com/45914355/82132836-f870de80-97db-11ea-8963-06ff0e2979ce.png)

![Req1 3](https://user-images.githubusercontent.com/45914355/82155226-4aad1080-986b-11ea-8024-1e207d0236e9.png)
