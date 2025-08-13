# Reddit Comment Moderation Classifier

**Bringing 'Comment Sense' to Reddit Moderation**

This repository contains code and resources for building a binary classifier that predicts whether a Reddit comment broke a specific subreddit rule. The project is inspired by real-world content moderation challenges and uses a dataset of moderated comments to train and evaluate models.

---

## Overview

If you’ve ever had a comment taken down on Reddit and wondered "why?", you’re not alone. Each subreddit has its own set of guidelines, and understanding moderation decisions can be complex. This competition aims to bring clarity by using machine learning to predict which rule (if any) a comment may have broken.

### Background

This work is inspired by research from [Deepak Kumar, Yousef AbuHashem, and Zakir Durumeric](https://arxiv.org/abs/2101.05196), where large language models were used to guess the reasons moderators removed comments. The dataset is based on the work of [Eshwar Chandrasekharan and Eric Gilbert](https://dl.acm.org/doi/10.1145/3308558.3313417), which collected millions of moderated comments. The dataset used here is several years old and unlabeled, with a small labeled dev set provided for training and evaluation.

---

## Dataset

- **Source**: Older, unlabeled Reddit comments with a small labeled dev set.
- **Rules**: Hypothetical rules derived from real subreddit guidelines.
- **Splits**:
  - Dev set: Small labeled subset for training and validation.
  - Test set: 30% public, 70% private for evaluation.

---
