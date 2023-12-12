# ConceptualCaptions-940k(NOT READY YET)
A subset of Google's ConceptualCaptions(3M) dataset which include 940k samples.

## Information
The data was from Google's [ConceptualCaptions](https://ai.google.com/research/ConceptualCaptions/)(CC) .
- 940k images-text pairs were selected from the original CC dataset, the caption-image data saved in **clean_train.tsv** , the image IDs saved in **clean_trainImages.txt** .
- Then , we use Hugging Face's pipelines to generate additional captions for the images, e.g. [BLIP](https://hf-mirror.com/Salesforce/blip-image-captioning-large) , [VIT-GPT2](https://hf-mirror.com/nlpconnect/vit-gpt2-image-captioning) and [MS-GIT](https://hf-mirror.com/microsoft/git-large-textcaps) . Check **[ModelName].tsv** & **clean_trainImages_[ModelName]** to get caption-image data and image IDs  .
- The LLM-generate-captions were checked and adjusted , we try to make it clean (by removing some special symbols or tokens that have no training value such as dates and names) .
Finally , we make the "ConceptualCaptions-940k" dataset for image caption or related multi-modal AI task training here .

## Download
The dataset is now availible for downloading in Kaggle , here is the [link](https://www.kaggle.com/datasets/aldenhovel/conceptualcaptions-940ksubset) .
At least 67GB space is required .

## Data Examples & Notebooks
Ort , still not ready yet .

## References
- [ConceptualCaptions(3M)](https://ai.google.com/research/ConceptualCaptions/)
- [ConceptualCaptions(12M)](https://github.com/google-research-datasets/conceptual-12m)
