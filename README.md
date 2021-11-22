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

The study *Acoustic Indices for Biodiversity Assessment and Landscape Investigation* explains the approach I decided to follow:

*Several α acoustic indices have been developed to try to assess the richness or complexity of an acoustic community or soundscape [...]
The concept of “complexity indices” is based on the assumption that the acoustic output of a community or a landscape will increase in complexity with the number of singing individuals and species. An index that captures the heterogeneity of sound should then give a proxy of animal acoustic activity. [...] An acoustic complexity index, ACI, was developed to produce a direct quantification of soundscape complexity by computing the variability of the intensities registered in audio recordings, despite the presence of constant human-generated-noise [1, 2]. The ACI works on the matrix returned by a short-term Fourier transform (STFT) applied to the complete recording or to a series of successive windows. The computation mainly consists in summing up the absolute difference between two adjacent values of intensity, Ik − Ik+1, where k is the kth position in the intensity values recorded along a single frequency bin of the STFT[3].*


For evaulating the quality of the biodiversity at specific locations, I picked the [Acoustic Complexity Index](https://github.com/patriceguyot/Acoustic_Indices)

### Conclusion 

As the above already mentioned *Acoustic Indices for Biodiversity Assessment and Landscape Investigation* puts it:

*"To finda single index that summarizes all biodiversity facets is undoubtedly utopian. There will not be any single value that will reliably estimate all levels of local or regional diversity. "*


- [1] N. Pieretti, A. Farina, D. Morri: A new methodology to infer the singing activity of an avian community: the Acoustic
Complexity Index (ACI). Ecological Indicators 11 (2011)
868–873.
- [2] A. Farina, N. Pieretti, L. Piccioli: The soundscape methodology for long-term bird monitoring: a Mediterranean Europe case-study. Ecological Informatics 6 (2011) 354–363.
- [3] Sueur, Jérôme & Farina, Almo & Gasc, Amandine & Pieretti, Nadia & Pavoine, Sandrine. (2014). Acoustic Indices for Biodiversity Assessment and Landscape Investigation. Acta Acustica united with Acustica. 100. 10.3813/AAA.918757. 
