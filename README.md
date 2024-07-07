---
title: Art Style Classifier
emoji: 🏆
colorFrom: yellow
colorTo: gray
sdk: gradio
sdk_version: 4.37.2
app_file: app.py
pinned: false
license: apache-2.0
---

# Art Style Classifier

Classify your art by fine art style. 

A [HuggingFace Space](https://huggingface.co/spaces/awhb/comic-medium-classifier), which is also embedded in a static webpage deployed on [GitHub Pages](https://awhb.github.io/comic-art-classifier/).

Built using the FastAI library following the FastAI course. Training dataset of around 4000 images obtained from WikiArt by user `Sivar Azadi`, reposted as a
[Kaggle Dataset](https://www.kaggle.com/datasets/sivarazadi/wikiart-art-movementsstyles).

Do checkout my process of fine-tuning the ConvNeXt-small-22k model using the fastai library on this [Kaggle Notebook](https://www.kaggle.com/code/awhangbin/wikiart-fine-art-styles-classification-w-fastai). Leave an upvote there if you enjoy! 


# Instructions to deploy to HF spaces 
(Note: Current local repo should already be tracking a HF remote space)

### Part 1: Init Git LFS
1. Run `git lfs install` after installing git-lfs (OS-dependent, I used Homebrew)
2. Run `git lfs track "*.jpg"`.
3. Run `git add .gitattributes`, `git commit -m "Track images with Git LFS"`.
4. Run `git add ...` for all image files. 
5. Run `git commit -m "Add art images tracked by Git LFS"`

### Part 2: Deploy to HF-Spaces
6. Run `git push`.