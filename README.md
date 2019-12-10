# Overview

The data presented in this repository were collected as part of a research project entitled _Exploring Writing Achievement and Its Role in Success at 4-Year Postsecondary Institutions._ This project was funded by the Institute of Education Science, U.S. Department of Education, [Award Number R305A160115](https://ies.ed.gov/funding/grantsearch/details.asp?ID=1807), and led by Dr. Jill Burstein (Principal Investigator) and Dr. Daniel McCaffrey (co-Principal Investigator). 

# Description

The repository contains the following main set of files:

- [`writing-samples/*.txt`](writing-samples): De-identified authentic university coursework writing data. There are 997 files in this directory, each representing one of the coursework assignments. 735 students participated in this study. A partially overlapping subset of students (N=418) submitted multiple coursework writing assignments. 

  Participants were enrolled at 4-year universities, and writing assignments were collected from courses primarily targeting first-year students. We refer to these files as the **University Coursework Writing Corpus**.  All assignment files are plaintext and UTF-8 encoded, where necessary.

- [`student_data.csv`](student_data.csv) : Data collected from student participants. Two types of data are collected: 
    - **Writing Attitude Survey Data**: This [survey](docs/surveys/writing_attitudes_survey.pdf) measured four components of writing attitudes and beliefs: (1) Goals for Writing, (2) Confidence about Writing Tasks, (3) Beliefs about Writing, and (4) Feelings about Writing. Note that the order of survey questions in this CSV file is _not_ the same as the original order of the questions in the survey. The survey was completed by 566 out of 735 total study participants. For the others, these columns are blank.

    - **Outcomes/Success Predictor Measures**:  A subset of outcomes/success predictor measures for the study participants, including: (1) their course grade (for the course in which writing assignments and surveys were submitted), (2) their study semester GPA, and (3) their SAT Total/ACT Composite score (recoded as `SAT Total score`).

  In total, there are 735 rows and 64 columns in this CSV file. A detailed description of each column can be found [here](docs/student_data_columns.csv).

- [`writing_features.csv`](writing_features.csv) : Various features based on the writing samples in the writing corpus. The following types of data are included:
    - **Assignment Preparation Survey Data**: [Survey](docs/surveys/assignment_preparation_survey.pdf) responses (N=929) collected from students regarding each coursework assignment they submitted. 

    - **Genre Annotations**: Human annotations for each assignment pertaining to assignment type, source requirements, source use, writing aim, and assignment version. 
 
    - **Automated Writing Evaluation (AWE) Features**:  Feature values generated for each of the 997 writing assignments from two different automated writing evaluation (AWE) systems. The features are computed based on grammar and mechanics errors, use of figurative & argumentative language, and vocabulary, among others. The two different AWE systems used to generate these features were e-Rater (Attali & Burstein, 2006) and Writing Mentor (Burstein et al., 2018)

  In total, there are 997 rows and 119 columns in this CSV file. A detailed description of each column can be found [here](docs/writing_features_columns.csv).


# Additional Documents

The following additional files can be found under [`docs`](docs).

- [`student_data_columns.csv`](docs/student_data_columns.csv) : A CSV file describing in detail each of the columns found in `student_data.csv`. 

- [`writing_features_columns.csv`](docs/writing_features_columns.csv) : A CSV file describing in detail each of the columns found in `writing_features.csv`. 

- [`surveys/assignment_preparation_survey.pdf`](docs/surveys/assignment_preparation_survey.pdf) : The instrument used for the assignment preparation survey. 

- [`surveys/writing_attitudes_survey.pdf`](docs/surveys/writing_attitudes_survey.pdf) : The instrument used for the writing attitudes survey. It is adapted from an instrument developed by MacArthur, Philippakos, & Graham (2016) to measure motivation among college writers. 

- [`forms/*.pdf`](docs/forms) : Blank copies of the student consent forms issued to the student participants.

- [`processes/deidentification_procedures.pdf`](docs/processes/deidentification_procedures.pdf) : This file contains a description of the steps that we followed in order to de-identify (remove any personally identifying information) from the writing samples and student metadata.

- [`processes/genre_annotation.pdf`](docs/processes/genre_annotation.pdf) : This file contains a description of the genre annotation performed to classify writing assignments based on broad assignment types.

# Related Publications & Presentations

- Burstein, J., McCaffrey, D., Beigman Klebanov, B., Ling, G. & Holtzman, S. (2019). [Exploring Writing Analytics and Postsecondary Success Indicators](https://eric.ed.gov/?q=%22%22&ff1=subWriting+Research&ff2=eduPostsecondary+Education&id=ED598690). In *Companion Proceedings 9^th International Conference on Learning Analytics & Knowledge (LAK19), Tempe, AZ.*

- Burstein, J., Invited Speaker, [Writing Analytics: Automated Writing Evaluation Feedback to Support Learning](https://events.nyu.edu/#!view/event/event_id/223975), Learning Analytics Research Network (LEARN) Seminar Series, New York University, February 12, 2019.

- Burstein J., Invited Speaker, [Natural Language Processing for Education: Applications for Reading and Writing Proficiency](https://spraakbanken.gu.se/larka/nlp4call7/NLP4CALL_slides_5.pdf), The Seventh Workshop on NLP for Computer- Assisted Language Learning (NLP4CALL), University of Stockholm, Stockholm, Sweden, November 7, 2018.

- Burstein, J., McCaffrey, D., Beigman Klebanov, B., & Ling, G. (2017). [Exploring Relationships between Writing and Broader Outcomes with Automated Writing Evaluation.](http://www.google.com/url?q=http%3A%2F%2Fwww.aclweb.org%2Fanthology%2FW%2FW17%2FW17-5011.pdf&sa=D&sntz=1&usg=AFQjCNHTJ-5a32cTH4-Pj1h06GtAFZ-jUA) In *Proceedings of the 12th Workshop on Innovative Use of NLP for Building Educational Applications (BEA)*, EMNLP 2017, Copenhagen, Denmark.

- Burstein, J. Elliot, N., Beigman Klebanov, B., Madnani, N., Napolitano, D., Schwartz, M., Houghton, P. & Molloy, H. (2018).  [Writing Mentor: Writing Progress Using Self-Regulated Writing Support](https://journals.colostate.edu/index.php/analytics/article/view/213).  Journal of Writing Analytics. Vol. 2: 285-313.

- MacArthur, C. A., Philippakos, Z. A., & Graham, S. (2016). A multi-component measure of writing motivation with basic college writers. *Learning Disability Quarterly, 39*, 31-43. DOI: 10.1177/0731948715583115.

# License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This data is released under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

# Contact Us

If you have any questions about the data, please send us an [email](mailto:ETS_IES_WAVES@ets.org?cc=hmolloy@ets.org,phoughton@ets.org,zmladineo@ets.org&subject=IES%20Writing%20Achievement%20Data).

# Acknowledgements

The data provided in this repository was collected via research supported by the Educational Testing Service, and the Institute of Education Science, U.S. Department of Education, [Award Number R305A160115](https://ies.ed.gov/funding/grantsearch/details.asp?ID=1807).

Thanks to Michael Flor, Binod Gyawali, Ben Leong, and Maxwell Schwartz for engineering support. Many thanks to our research assistants, Patrick Houghton, Hillary Molloy and Zydrune Mladineo, for managing a complex data collection.
