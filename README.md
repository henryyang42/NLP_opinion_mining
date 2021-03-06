# NTU NLP 2017 - Term Project 1

## [Hotel Review Opinion Mining](https://inclass.kaggle.com/c/ntu-nlp-2017-term-project-1)

### Task

From a hotel review as the following,

```text
總體感覺充其量四星吧，根本達不到五星。尤其是二樓的西餐廳的飯菜實在做的不敢恭維，根本不像西餐，口味也有待提高，品種也少。環境有點亂哄哄，唯一的優勢可能是便宜。

```

extract aspect-specific opinions like:

- 環境 negative
- 價格 positive
- 餐廳 negative

### Data

- **[aspect_review.txt](data/aspect_review.txt)** - small review dataset with aspect-polarity labels
- **[polarity_review.txt](data/polarity_review.txt)** - large review dataset with only polarity labels
- **[NTUSD_pos.txt](data/NTUSD_pos.txt) / [NTUSD_neg.txt](data/NTUSD_neg.txt)** - sentiment dictionary
- **[aspect_term.txt](data/aspect_term.txt)** - example terms that refer to certain aspect
- **[test_review.txt](data/test_review.txt)** - test reviews to extract aspect-specific opinions
- **[test.csv](data/test.csv)** - test questions
- **[sample_submission.csv](data/sample_submission.csv)**
- Preprocessed data (Segmentation)
  - **[test_seg.csv](data/test_seg.csv)** - ``test.csv`` combine with ``test_review.txt``
  - **[aspect_review\_seg.csv](data/aspect_review_seg.csv)**
  - **[polarity_review\_seg.csv](data/polarity_review_seg.csv)**
- Preprocessed data (Segmentation & Pos tagged)
  - **[test_posseg.csv](data/test_posseg.csv)** - ``test.csv`` combine with ``test_review.txt``
  - **[aspect_review\_posseg.csv](data/aspect_review_posseg.csv)**
  - **[polarity_review\_posseg.csv](data/polarity_review_posseg.csv)**

### Public Data Label Distribution


| Label | Freq |
|:-----:|:----:|
| -1    | 0.23963 |
| 0     | 0.57719 |
| 1     | 0.18318 |
