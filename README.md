# AUTOMATIC-ICD-CODING
This repo enables the user input a text description or summary for a medical encounter. It then returns the top n most probable ICD codes where n is specified by the user.
recommended n values: 5-15. This enables the model catch more similar and probable codes.
A language model embeds the input text and computes the cosine-similarity with all the ICD codes. This similarity score helps rank the ICD codes by probability conditioned on the input text.
A good next step is to fine-tune multi-label language models on MIMIC II, III and IV datasets but these aren't free for download.
