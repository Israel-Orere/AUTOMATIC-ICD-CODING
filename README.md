# AUTOMATIC-ICD-CODING
This repo enables the user input a text description or summary for a medical encounter. It then returns the top n most probable ICD codes where n is specified by the user.
recommended n values: 5-15. This enables the model catch more similar and probable codes.
A language model embeds the input text and computes the cosine-similarity with all the ICD codes. This similarity score helps rank the ICD codes by probability conditioned on the input text.
Input text should be entered in a way that steers the model towards optimal results. For example, in the anonymized dataset, column, value pairs can be entered thus: 'column':'value'. Physical examination and medication are columns that can have their values entered in the recommended format to add more context to the sentence. Any column of relevance should have their column value pairs added in the input text. 
The base use cases are encounter descriptions from the encounters.csv files as these represent direct contact between patient and doctor.
