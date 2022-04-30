# Datasheet: *Short Stories Paragraph Genre*

Author: *Claire Chour*

Organization: *Group 33*


## Motivation

*The questions in this section are primarily intended to encourage dataset creators to clearly articulate their reasons for creating the dataset and to promote transparency about funding interests.*

1. **For what purpose was the dataset created?** Was there a specific task in mind? Was there a specific gap that needed to be filled? Please provide a description.

	*The dataset was created by Project Gutenberg for the purpose of providing
access to 60,000+ eBooks. From these short stories, we took a paragraph from
each short story, as reading through all the short stories would take too long. The
specific task in mind was determining whether we could build a model that
predicts whether a short story was the genre of mystery, romance, sci-fi/fantasy,
or none.*

2. **Who created this dataset (e.g. which team, research group) and on behalf of which entity (e.g. company, institution, organization)**?

	*Project Gutenberg created it for reading enjoyment and unlimited free
redistribution of the public.*

3. **What support was needed to make this dataset?** (e.g. who funded the creation of the dataset? If there is an associated grant, provide the name of the grantor and the grant name and number, or if it was supported by a company or government agency, give those details.)

	*Project Gutenberg takes donations from loyal customers. The Project Gutenberg
Literary Archive Foundation is the non-profit corporation that oversees Project
Gutenberg’s operation. It receives and processes payments for Project
Gutenberg.*

4. **Any other comments?**

	*No*


## Composition

*Dataset creators should read through the questions in this section prior to any data collection and then provide answers once collection is complete. Most of these questions are intended to provide dataset consumers with the information they need to make informed decisions about using the dataset for specific tasks. The answers to some of these questions reveal information about compliance with the EU’s General Data Protection Regulation (GDPR) or comparable regulations in other jurisdictions.*

1. **What do the instances that comprise the dataset represent (e.g. documents, photos, people, countries)?** Are there multiple types of instances (e.g. movies, users, and ratings; people and interactions between them; nodes and edges)? Please provide a description.

	*The dataset represents a plethora of short stories of different genres.*

2. **How many instances are there in total (of each type, if appropriate)?**

	*There is not a set number of instances, as there are unlimited genres, but we
only chose to identify 3 or none.*

3. **Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set?** If the dataset is a sample, then what is the larger set? Is the sample representative of the larger set (e.g. geographic coverage)? If so, please describe how this representativeness was validated/verified. If it is not representative of the larger set, please describe why not (e.g. to cover a more diverse range of instances, because instances were withheld or unavailable).

	*The dataset contains 1000 paragraphs from 1000 short stories of different
instances, so it is a sample of the entire dataset. The sample is not
representative of the larger set, as there could be some genres we missed when
randomizing which short stories to take a paragraph from. Project Gutenberg did
categorize by genre sometimes, but there are a lot more than 1000 short stories
to pick from, so it is not representative of the larger set.*

4. **What data does each instance consist of?** "Raw" data (e.g. unprocessed text or images) or features? In either case, please provide a description.

	*The data consists of genres of mystery, romance, sci-fi/fantasy, and others.
When reading other genres, we would simply default to none.*

5. **Is there a label or target associated with each instance?** If so, please provide a description.

	*For some instances, there were labels of what genre the story could have been
due to the short story’s title; however, we tried to not look at that, as it would
induce bias*

6. **Is any information missing from individual instances?** If so, please provide a description, explaining why this information is missing (e.g. because it was unavailable). This does not include intentionally removed information, but might include, e.g. redacted text.

	*No, our dataset contained all the information from instances we needed*

7. **Are relationships between individual instances made explicit (e.g. users' movie ratings, social network links)?** If so, please describe how these relationships are made explicit.

	*The relationships between individual instances are not always explicit. We had to
read through each paragraph in order to determine the genre of the short story.*

8. **Are there recommended data splits (e.g. training, development/validation, testing)?** If so, please provide a description of these splits, explaining the rationale behind them.

	*We did not specify how to split the data. Instead, we simply split the data
randomly 70% training and 30% test. The reason behind this is because we tried
to make sure that our dataset was evenly distributed of short stories that were
mysterious, romantic, sci-fi/fantasy, or none.*

9. **Are there any errors, sources of noise, or redundancies in the dataset?** If so, please provide a description.

	*There were no redundancies in this dataset since we manually checked after we
created our dataset. However, we did have some errors in our model (we
conducted full error analysis). The errors were that some short stories would be
identified differently than the actual; in other words, the predicted and actual
result were different.*

10. **Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g. websites, tweets, other datasets)?** If it links to or relies on external resources, a) are there guarantees that they will exist, and remain constant, over time; b) are there official archival versions of the complete dataset (i.e., including the external resources as they existed at the time the dataset was created); c) are there any restrictions (e.g. licenses, fees) associated with any of the external resources that might apply to a future user? Please provide descriptions of all external resources and any restrictions associated with them, as well as links or other access points, as appropriate.

	*The dataset is self-contained, as it does not rely on external resources. Project
Gutenberg is open-source, so there were no restrictions such as licenses or fees
associated with it.*

11. **Does the dataset contain data that might be considered confidential (e.g. data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals' non-public communications)?** If so, please provide a description.

	*No, there is no confidential data.*

12. **Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety?** If so, please describe why.

	*No, the dataset is simply short stories that would not be regarded as offensive.*

13. **Does the dataset relate to people?** If not, you may skip the remaining questions in this section.

	*Yes, sometimes the short stories would talk about characters who were people.*

14. **Does the dataset identify any subpopulations (e.g. by age, gender)?** If so, please describe how these subpopulations are identified and provide a description of their respective distributions within the dataset.

	*No, we did not identify any subpopulations.*

15. **Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset?** If so, please describe how.

	*Yes, it would be somewhat possible to identify individuals, but it would require
more than just taking one paragraph from each short story.*

16. **Does the dataset contain data that might be considered sensitive in any way (e.g. data that reveals racial or ethnic origins, sexual orientations, religious beliefs, political opinions or union memberships, or locations; financial or health data; biometric or genetic data; forms of government identification, such as social security numbers; criminal history)?** If so, please provide a description.

	*The dataset could potentially contain data that may be considered sensitive, as
some short stories talked about sexual orientations and religion.*

17. **Any other comments?**

	*No*


## Collection

*As with the previous section, dataset creators should read through these questions prior to any data collection to flag potential issues and then provide answers once collection is complete. In addition to the goals of the prior section, the answers to questions here may provide information that allow others to reconstruct the dataset without access to it.*

1. **How was the data associated with each instance acquired?** Was the data directly observable (e.g. raw text, movie ratings), reported by subjects (e.g. survey responses), or indirectly inferred/derived from other data (e.g. part-of-speech tags, model-based guesses for age or language)? If data was reported by subjects or indirectly inferred/derived from other data, was the data validated/verified? If so, please describe how.

	*The data was acquired through reading a paragraph of each short story, so the
data was directly observable from the raw text.*

2. **What mechanisms or procedures were used to collect the data (e.g. hardware apparatus or sensor, manual human curation, software program, software API)?** How were these mechanisms or procedures validated?

	*There were no complex procedures to collect the data; it was simply through
reading each short story.*

3. **If the dataset is a sample from a larger set, what was the sampling strategy (e.g. deterministic, probabilistic with specific sampling probabilities)?**

	*We took a random paragraph from each short story. We did not usually take one
from the first paragraph of each shor story since studies showed that the first
paragraph of stories are usually not as informative regarding the genre.*

4. **Who was involved in the data collection process (e.g. students, crowdworkers, contractors) and how were they compensated (e.g. how much were crowdworkers paid)?**

	*My group members, as well as whoever helped from AP2, were the only ones
involved in the data collection process. Nobody was paid.*

5. **Over what timeframe was the data collected?** Does this timeframe match the creation timeframe of the data associated with the instances (e.g. recent crawl of old news articles)? If not, please describe the timeframe in which the data associated with the instances was created. Finally, list when the dataset was first published.

	*The data was collected from 1971 until now (short stories are still being added
today).This timeframe matches the creation timeframe of the data associated
with the instances. The dataset was first published in 1971.*

7. **Were any ethical review processes conducted (e.g. by an institutional review board)?** If so, please provide a description of these review processes, including the outcomes, as well as a link or other access point to any supporting documentation.

	*No, there were no ethical review processes conducted.*

8. **Does the dataset relate to people?** If not, you may skip the remainder of the questions in this section.

	*No.*

9. **Did you collect the data from the individuals in question directly, or obtain it via third parties or other sources (e.g. websites)?**

	*N/A*

10. **Were the individuals in question notified about the data collection?** If so, please describe (or show with screenshots or other information) how notice was provided, and provide a link or other access point to, or otherwise reproduce, the exact language of the notification itself.

	*N/A*

11. **Did the individuals in question consent to the collection and use of their data?** If so, please describe (or show with screenshots or other information) how consent was requested and provided, and provide a link or other access point to, or otherwise reproduce, the exact language to which the individuals consented.

	*N/A*

12. **If consent was obtained, were the consenting individuals provided with a mechanism to revoke their consent in the future or for certain uses?** If so, please provide a description, as well as a link or other access point to the mechanism (if appropriate).

	*N/A*

13. **Has an analysis of the potential impact of the dataset and its use on data subjects (e.g. a data protection impact analysis) been conducted?** If so, please provide a description of this analysis, including the outcomes, as well as a link or other access point to any supporting documentation.

	*N/A*

14. **Any other comments?**

	*No*


## Preprocessing / Cleaning / Labeling

*Dataset creators should read through these questions prior to any pre-processing, cleaning, or labeling and then provide answers once these tasks are complete. The questions in this section are intended to provide dataset consumers with the information they need to determine whether the “raw” data has been processed in ways that are compatible with their chosen tasks. For example, text that has been converted into a “bag-of-words” is not suitable for tasks involving word order.*

1. **Was any preprocessing/cleaning/labeling of the data done (e.g. discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)?** If so, please provide a description. If not, you may skip the remainder of the questions in this section.

	*Yes, we made all the letters in the short stories lowercase and cleaned up some
punctuation.*

2. **Was the "raw" data saved in addition to the preprocessed/cleaned/labeled data (e.g. to support unanticipated future uses)?** If so, please provide a link or other access point to the "raw" data.

	*No, we did not save it.*

3. **Is the software used to preprocess/clean/label the instances available?** If so, please provide a link or other access point.

	*We used the Python function lower().
https://www.programiz.com/python-programming/methods/string/lower*

4. **Any other comments?**

	*No*


## Uses

*These questions are intended to encourage dataset creators to reflect on the tasks  for  which  the  dataset  should  and  should  not  be  used.  By  explicitly highlighting these tasks, dataset creators can help dataset consumers to make informed decisions, thereby avoiding potential risks or harms.*

1. **Has the dataset been used for any tasks already?** If so, please provide a description.

	*Yes, this dataset has been standardized for statistical analysis of qualitative
linguistics, used to visualize sentiment shifts, and used to analyze the frequency
of words.*

2. **Is there a repository that links to any or all papers or systems that use the dataset?** If so, please provide a link or other access point.

	*Here are some links:
https://arxiv.org/abs/1812.08092
https://github.com/clarencestephen/Project-Gutenberg
https://github.com/maevadevs/Project-Gutenberg-NLP*

3. **What (other) tasks could the dataset be used for?**

	*This task could be used to determine whether a short story is a specific genre or
not (instead of determining multiple genres) and for narrative patterns.*

4. **Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?** For example, is there anything that a future user might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g. stereotyping, quality of service issues) or other undesirable harms (e.g. financial harms, legal risks) If so, please provide a description. Is there anything a future user could do to mitigate these undesirable harms?

	*No, because they are just short stories.*

5. **Are there tasks for which the dataset should not be used?** If so, please provide a description.

	*Yes, the dataset should not be used for tasks that would work poorly with textual
data. For instance, linear regression would not be appropriate for this dataset.*

6. **Any other comments?**

	*No*


## Distribution

*Dataset creators should provide answers to these questions prior to distributing the dataset either internally within the entity on behalf of which the dataset was created or externally to third parties.*

1. **Will the dataset be distributed to third parties outside of the entity (e.g. company, institution, organization) on behalf of which the dataset was created?** If so, please provide a description.

	*No.*

2. **How will the dataset will be distributed (e.g. tarball on website, API, GitHub)?** Does the dataset have a digital object identifier (DOI)?

	*The dataset can be distributed via Project Gutenberg, API, or Github. No, the
dataset does not have a DOI.*

3. **When will the dataset be distributed?**

	*The dataset can be distributed anytime now.*

4. **Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?** If so, please describe this license and/or ToU, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms or ToU, as well as any fees associated with these restrictions.

	*No.*

5. **Have any third parties imposed IP-based or other restrictions on the data associated with the instances?** If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms, as well as any fees associated with these restrictions.

	*No.*

6. **Do any export controls or other regulatory restrictions apply to the dataset or to individual instances?** If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any supporting documentation.

	*No.*

7. **Any other comments?**

	*No*


## Maintenance

*As with the previous section, dataset creators should provide answers to these questions prior to distributing the dataset. These questions are intended to encourage dataset creators to plan for dataset maintenance and communicate this plan with dataset consumers.*

1. **Who is supporting/hosting/maintaining the dataset?**

	*The dataset does not jeed to be maintained unless we want to add more data
points, as it does not need to be updated.*

2. **How can the owner/curator/manager of the dataset be contacted (e.g. email address)?**

	*The owner can be contacted through
https://www.gutenberg.org/about/contact_information.html*

3. **Is there an erratum?** If so, please provide a link or other access point.

	*No.*

4. **Will the dataset be updated (e.g. to correct labeling errors, add new instances, delete instances)?** If so, please describe how often, by whom, and how updates will be communicated to users (e.g. mailing list, GitHub)?

	*No.*

5. **If the dataset relates to people, are there applicable limits on the retention of the data associated with the instances (e.g. were individuals in question told that their data would be retained for a fixed period of time and then deleted)?** If so, please describe these limits and explain how they will be enforced.

	*N/A*

6. **Will older versions of the dataset continue to be supported/hosted/maintained?** If so, please describe how. If not, please describe how its obsolescence will be communicated to users.

	*No, the older versions of the dataset will not be maintained, and this can be
communicated to users through a note on the bottom or top of the text.*

7. **If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so?** If so, please provide a description. Will these contributions be validated/verified? If so, please describe how. If not, why not? Is there a process for communicating/distributing these contributions to other users? If so, please provide a description.

	*No.*

8. **Any other comments?**

	*No*
