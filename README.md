# RS-Final-Project
The project is about recommending developers to solve a bug based on their source code. I used a supervised dataset [any commit which are related to a bug has an asigned author (developers)]. I used LDA method to find the domians (topics) of each developer, then I asign them to a bug based on their domain. Also, I used a classification method (KNN) as a baseline to compare the result of LDA with the baseline. For dataset I used two method that I called them "NLP" and "AST". For NLP dataset, I used language processing tokenizer to extract the tokens within a source code. For "AST" dataset, I used Abstract Syntax Tree and considered each node of tree as a token. "Pydriller" that I import below is a libriary to drill (scrape) the github repository. I extracted one year data (commit) for 15 developers from "Panda" Repository. The structure of report in the jupyter notebook is as below:

1. Extracting data of github for NLP study
2. LDA method on NLP data
3. KNN method on NLP data
4. Extracting data for AST study
5. A step by step explanation of how AST function works and find the tokens
6. Run the AST function on whole dataset to extract tokens
7. KNN method on AST data
8. LDA method on AST data
9. Conclusion
