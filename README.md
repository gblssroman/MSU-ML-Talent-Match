# 🏆 ML Talent Match of Moscow State University // Prizewinners Solution
📝 **Task:**
Make a high-quality matching & ranking of applicants' resumes to the specific vacancies.

✅ **Result:**
Up to 94% time savings for HR specialists.

# Our team:
* [Roman Prasad](https://github.com/gblssroman)
* [Solomon Chakaev](https://github.com/veidlink)
* [Nikita Chuikin](https://github.com/AnalyseOptimize)
* [Vladislav Taskaev](https://github.com/vladik-pwnz)

# Data:
We were given two JSON-files (you can find them in our repo):

* **First** containing pairs Resume-[N candidates] with the label ```"failed_resumes"```/```"confirmed_resumes"```
* **Second** containing pairs Resume-[N candidates] without labels

# Our approach
## 1. EDA
* JSON -> CSV Parsing
* Data cleaning (RegExp & N/A processing)
* Removing non-valuable features by checking their distributions according to the acceptance in train

Columns, which correlate the most with the target, contain text data:

In vacancies:
```'Vacancy Name', 'Keywords', 'Description', 'Comment'```

In resumes: 
```'About', 'Key Skills', 'Position', 'Experience Description', 'Organization', 'Faculty', 'Specialty'```.

It should be noted, that the candidate's age and gender are not encountered ethically (there are no visible correlations in age, still, but 
there is a small inbalance between gender acceptance rates). Hence, we are mostly sticking to NLP practices as we have a task in this sphere.
Text preprocessing methods, such as lemmatization, were used but are not implemented in our final approach.

Data preprocessing is fully automated in our Streamlit App (JSON-only files are supported).


## 2. Models
### CatBoost & Clusterization
...

### AutoML
...

### Fine-tuning BERT & roBERTa-XLM
...

## 3. Best result
...

