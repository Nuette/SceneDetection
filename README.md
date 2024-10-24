# SceneDetection
Identify scenes in narratives.

**Version 1**


A simple model that identifies characters using coreference and time/place using Spacy's GPE, LOC, and DATE labels.
Summaries are identified by comparing adjectives to action verbs. If there are more adjectives than action verbs, it's likely a description. 
A sliding window was used to retain character, time and place information for sentences and combine sentences with matching features into a scene.

**Version 2**

Slightly more sophisticated than v1. We identify characters, time and place in a similar manner. We add a character_change_threshold and place_memory to keep track of characters and the place of a scene. We add a similarity_threshold using BERT to identify if a segment is significantly different to other texts. 
