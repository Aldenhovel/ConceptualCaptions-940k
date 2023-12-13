# ConceptualCaptions-940k
A subset of Google's ConceptualCaptions(3M) dataset which include 940k image-text samples. 

## Information
The data was from Google's [ConceptualCaptions](https://ai.google.com/research/ConceptualCaptions/)(CC) . 940k images-text pairs were selected from the original CC dataset, the caption-image data saved in **clean_train.tsv** , the image IDs saved in **clean_trainImages.txt** . Then , we use Hugging Face's pipelines to generate additional captions for the images, e.g. 
- [BLIP](https://hf-mirror.com/Salesforce/blip-image-captioning-large)
- [VIT-GPT2](https://hf-mirror.com/nlpconnect/vit-gpt2-image-captioning) (not ready)
- [MS-GIT](https://hf-mirror.com/microsoft/git-large-textcaps) (not ready)

Check **[ModelName].tsv** & **[ModelName].txt** to get caption-image data and image IDs . The LLM-generate-captions were checked and adjusted , we try to make it clean (by removing some special symbols or tokens that have no training value such as dates and names) . Finally , we make the "ConceptualCaptions-940k" dataset for image caption or related multi-modal AI task training here .

## Download
The dataset is now availible for downloading in Kaggle : [conceptualcaptions-940ksubset](https://www.kaggle.com/datasets/aldenhovel/conceptualcaptions-940ksubset) .
Before downloading , at least 68GB space is required .
1. Download `imgs.7z.001` ~ `imgs.7z.092` and unzip `imgs.7z.001` (recommand using [Bandizip](https://bandizip.en.softonic.com/)) , get image files.
2. Download image list TXT file and its captions TSV file , for example , `blip.txt` and `blip.txv` .
3. Load image list get all the image file names , find the caption in TSV file , find the image in `imgs/` .

## Data Examples & Notebooks
Coming soon .

## References
- [ConceptualCaptions(3M)](https://ai.google.com/research/ConceptualCaptions/)
- [ConceptualCaptions(12M)](https://github.com/google-research-datasets/conceptual-12m)
