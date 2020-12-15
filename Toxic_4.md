![toxic](https://i.ibb.co/wBkzfQM/toxic-final.png) 


# Instructions

### Files
 |  Files & Links |  Description |
 |---------|---------|
 | [pred.csv][predcsv] | ***Result Link*** of Span Prediction on the test.csv |
 | [model][model] | Our ***best model's*** link |
 | [trainfinal.csv][traincsv] | Our training file provided by our TAs. |
 | [devfinal.csv][devcsv] | Initial test file provided by our TAs, but currently we use it as validation dataset. |
 | [test.csv][testcsv] | Our test file provided by our TAs. |
 
### Training Script
  - The trainig script can be found [here][train].
  - Divide the *trainfinal* dataset into training and validation dataset and upload it to cloab notebook. 
  - >(Finally we are using *trainfinal* as training and *devfinal* as validation dataset.)
    > Our model is being saved at "./drive/My Drive/best" so we also need to mount the drive.
    > You can directly access our [model][model]

### Prediction generation Script
  - The Prediction generation script can be found [here][predict].
  - > Upload *test.csv* to cloab notebook.
    > Download and directly access our [model][model]
    > Save this model at "./drive/My Drive/Submission/best" by mounting your drive.
    > Run all the cells of the colab file.

### Evaluation Script
  - The evaluation script can be found [here][eval].
  - >Upload the actual csv file containg the ground truth labels and the prediction.csv file.
    > Run all the cells in the colab file.
    > The **F1-score**  will be printed at the end.


### Libraries needed to be imported

We use the following libraries:
* ast
* csv
* random
* statistics
* sys
* itertools
* string
* pandas
* sklearn
* spacy

### Installation

Install the spacy and sklearn along with models as (no need if you are running in colab) :
```
  pip install spacy sklearn
  python -m spacy download en_core_web_sm
```


 
### Refrences
 - Official **Toxic Spans Detection *Semeval (Task 5)*** [*webpage*][website] & [*GitHub Repository*][repo].

   [repo]: <https://github.com/ipavlopoulos/toxic_spans>    
   [website]:<https://sites.google.com/view/toxicspans>
   [model]: <https://drive.google.com/drive/folders/1_DSJ3-zgVCqh2EWfmGDHMRwhEDuFcM6O?usp=sharing>
   [train]: <https://colab.research.google.com/drive/121DRdJv203tVHd-ghe8yyGKTduH3B8xn?usp=sharing>
   [predict]: <https://colab.research.google.com/drive/1M_pAEK-u3M7xrn-1lPHLx9JFY-2-MOJn?usp=sharing>
   [eval]: <https://colab.research.google.com/drive/1D4G5RLDTAOKOaVymm7VuM_LtRPzQGOcs?usp=sharing>
   [predcsv]: <https://drive.google.com/file/d/1jRm1nv8rMSmfGsQK_lG6285Fpq2a-6Kg/view>
   [testcsv]: <https://drive.google.com/file/d/1qe46c0BWCB9H2flHpgh8ojuHiTeGQO5T/view?usp=sharing>
   [traincsv]: <https://drive.google.com/file/d/1qNQ6lNMTa3IieVPNXm_JVGkgXxbQkL7s/view?usp=sharing>
   [devcsv]: <https://drive.google.com/file/d/1BMOd-KCEJM-J1qZVg4akMCA6Cwc5xutq/view?usp=sharing>