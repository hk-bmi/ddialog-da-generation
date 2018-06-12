**Coling 2018** - Dialogue Act Driven Conversation Model: An Experimental Study

IR based dialog generation with Dialogue Act using generation and discriminative model on DailyDialog dataset.

**This is a placeholder for the data and code associated with our paper titled "Dialogue Act Driven Conversation Model: An Experimental Study". We are currently in the process of obtaining approval from our organization to release the resources in public domain. We will update this page with the code, data and installation/execution instructions after we obtain the approval. **

# Abstract
The utility of additional semantic information for the task of next utterance selection in an automated dialogue system is the focus of study in this paper. In particular, we show that additional information available in the form of dialogue acts --when used along with context given in the form of dialogue history-- improves the performance irrespective of the underlying model being generative or discriminative. In order to show the model agnostic behavior of dialogue acts, we experiment with several well-known models such as sequence-to-sequence encoder-decoder model, hierarchical encoder-decoder model, and Siamese-based models with and without hierarchy; and show that in all models, incorporating dialogue acts improves the performance by a significant margin. We, furthermore, propose a novel way of encoding dialogue act information, and use it along with hierarchical encoder to build a model that can use the         *sequential* dialogue act information in a natural way. Our proposed model achieves an MRR of about **84.8** for the task of next utterance selection on a newly introduced Daily Dialogue dataset, and outperform the baseline models. We also provide a detailed analysis of results including key insights that explain the improvement in MRR because of dialog act information.

<!-- There are two folders:
* ##Data - It contains the corpus (DailyDialog dataset) that we have prepared for the above task, especially, we have extended the DailyDialog datset for the Siamese Model.
* ##Code - It contains two folders, one for **generative** model and other for **discriminative** model
    * ##generative
        * **ed**
        `python ed.py train-conv-hred.txt dd_tkn_train_dict.pk test-conv-hred-10.txt dd_tkn_data.emb`
        * **ed-da**
        `python ed_pda.py train-conv-hred.txt dd_tkn_train_dict.pk test-conv-hred-10.txt train-label-hred.txt test-label-hred-10.txt, dd_tkn_data.emb`
        * **hred**
        `python batch_with_context.py, train-conv-hred.txt, dd_tkn_train_dict.pk, test-conv-hred-10.txt`
        * **hred-da**
        `python batch_with_context_predicted_da.py train-conv-hred.txt dd_tkn_train_dict.pk test-conv-hred-10.txt train-label-hred.txt test-label-hred-10.txt`
    * discriminative
        * **siamese**
        `python dual_encoder_siamese.py train-conv-hred-siam.txt dd_tkn_train_dict.pk test-conv-hred-10.txt gt.txt dd_tkn_data.emb`
        * **siamese-da**
        `python dual_encoder_siamese_pda1.py train-conv-hred-siam.txt test-conv-hred-10.txt train-label-hred-siam.txt  test-label-hred-10.txt dd_tkn_train_dict.pk gt.txt dd_tkn_data.emb`
        * hsiamese
        `python hred_siamese_simple.py train-conv-hred-siam.txt dd_tkn_train_dict.pk test-conv-hred-10.txt gt.txt  dd_tkn_data.emb`
        * hsiamese-da
        `python hred_siamese_simple_pda1.py train-conv-hred-siam.txt test-conv-hred-10.txt train-label-hred-siam.txt  test-label-hred-10.txt dd_tkn_train_dict.pk gt.txt dd_tkn_data.emb`

**License**: The code and data released under this repository is under the *Eclipse Public License*

**Citation**: To cite this paper
				
Harshit Kumar, Arvind Agarwal, Sachindra Joshi, "Dialogue Act Driven Conversation Model: An Experimental Study", to appear in COLING 2018. -->

