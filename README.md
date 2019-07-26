# teiModel

In this folder, two versions of the TEI model used for First World War Wills project (i.e. transcriptions of the wills and authority files):

* in the version-1 folder : the unique and global model used till May 2018. 
    * ODD file, 
    * HTML version of the documentation, 
    * Relax NG schema, 
    * examples: one containing the transcription of a will; and four other files (three of them containing examples of authority records on persons, places and military units ; the last one contains the vocabulary that can be used for analysing the content of the wills, as concerns the vision of death and the state of mind of the authors).
    
* in the version-2 folder: the latest version of the model, that uses the ODD chaining technique (see http://teic.github.io/TCW/howtoChain.html) and includes:
    * the ODD document that defines a global model for the future TeiCorpus file that will include all the TEI files of the project (the transcription of each will and the authority files). This ODD document is provided in 2 versions:
        * one that refers to the current TEI specification (as usually done) (file named `TeiModel_for_FirstWorldWarWills_v2_global_ODD.xml`)
        * one that results from compiling the first version, and that includes every formal definition used for the elements and attributes chosen (file named `TeiModel_for_FirstWorldWarWills_v2_global_ODD_compiled.xml`)
    * the HTML documentation and RNG schema generated from this ODD global model
    * the ODD document that defines the model used for the transcription of the wills. This ODD document (file named `TeiModel_for_FirstWorldWarWills_v2_transcription_ODD.xml`) uses the ODD global compiled file as its source and only re-defines (mode="replace") some elements
    * the RNG schema (file named `TeiModel_for_FirstWorldWarWills_v2_transcription.rng`) generated from the transcription ODD file)
    * a test TEI XML file that validates against the transcription RNG schema

We will add other ODD and RNG files to the version-2 folder soon. 