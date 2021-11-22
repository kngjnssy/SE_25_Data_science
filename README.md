## An attempt to assess biodiversity at various SAFE locations
### Background

Our dataset was collected as part of the Stability of Altered Forest Ecosystem (SAFE) research project *[Continuous bio-acoustic monitoring](https://www.safeproject.net/projects/project_view/175) in the tropical rainforests of Sabah, Borneo.* As described, *“the project is set in an area being actively deforested and converted to palm oil plantations, creating the ideal location to study the eﬀect of a changing habitat upon biodiversity.”*

Currently we have access to tabular data describing the recorded audio files (**Point_count_recordings**) and observations of two research assistants (**Point_count_data**). These two tables can be linked by the “Point_count_ID” column and therefore locate the corresponding audio segment to each (audio or audio-visual) observation. As the dataset description states, *“associated with each point count is an audio recording file, so (theoretically) this could be used as a training dataset for automated bioacoustic studies”.*

### Aim of the analysis

As I explored the available metadata and the limited number of audio recordings, the following questions came to my mind: 

- Are differences in land use influence biodiversity?
- Is there a measurable decline in biodiversity near sites with increased human activity? How to analyse soundscape as a whole?
- How to detect broad scale changes?
 
#### Analysing soundscapes and geospatial data

For evaulating the quality of the biodiversity at specific locations, I decided to compute the [Acoustic Complexity Index](https://github.com/patriceguyot/Acoustic_Indices)
