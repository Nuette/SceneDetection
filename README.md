# SceneDetection
Identify scenes in narratives.

**Version 1**
A simple model that identifies characters using coreference and time/place using Spacy's GPE, LOC, and DATE labels.
Summaries are identified by comparing adjectives to action verbs. If there are more adjectives than action verbs, it's likely a description. 
A sliding window was used to retain character, time and place information for sentences and combine sentences with matching features into a scene.
