---
authors: Richard Lindholm, Oscar Marklund, Olof Mogren, John Martinsson
box-bg-imgsrc: ''
doi: https://doi.org/10.48550/arXiv.2503.02422
eprint: '2503.02422'
generatebibtex: 'yes'
imgalt: Top K Entropy uncertainty aggregation selects the top K segment
  entropies (here K=3) obtained from the segments of the file. The resulting
  uncertainty for the file is the average of the selected segment entropies.
imgsrc: '/images/posts/2025-eusipco.png'
layout: posts
longversion: "<img src=\"/images/posts/2025-aggregation.png\" style=\"float: right\"> Abstract: The vast amounts of audio data collected in Sound Event Detection (SED)
  applications require efficient annotation strategies to enable supervised learning.
  Manual labeling is expensive and time-consuming, making Active Learning (AL) a promising
  approach for reducing annotation effort. We introduce Top K Entropy, a novel uncertainty
  aggregation strategy for AL that prioritizes the most uncertain segments within
  an audio recording, instead of averaging uncertainty across all segments. This approach
  enables the selection of entire recordings for annotation, improving efficiency
  in sparse data scenarios. We compare Top K Entropy to random sampling and Mean Entropy,
  and show that fewer labels can lead to the same model performance, particularly
  in datasets with sparse sound events. Evaluations are conducted on audio mixtures
  of sound recordings from parks with meerkat, dog, and baby crying sound events,
  representing real-world bioacoustic monitoring scenarios. Using Top K Entropy for
  active learning, we can achieve comparable performance to training on the fully
  labeled dataset with only 8% of the labels. Top K Entropy outperforms Mean Entropy,
  suggesting that it is best to let the most uncertain segments represent the uncertainty
  of an audio file. The findings highlight the potential of AL for scalable annotation
  in audio and time-series applications, including bioacoustics."
pdf: https://arxiv.org/pdf/2503.02422.pdf
permalink: /publications/2025/aggregation/
shortversion: "RIDR recently presented new research on efficient annotation strategies for bioacoustic sound events at EUSIPCO 2025, where it was selected for an oral presentation. The study introduces Top K Entropy, a novel approach for uncertainty aggregation in active learning where several data points are grouped in each file (such as audio segments in recording files). This method can significantly reduce labeling effort, which is often a bottleneck in supervised learning for sound event detection. By improving the aggregation of uncertainties, and allowing for prioritizing the most informative audio segments, Top K Entropy achieves model performance comparable to fully labeled datasets while using as little as 8% of the labels. Evaluations on mixtures of real-world bioacoustic recordings, such as meerkat, dog, and baby cries, show clear improvements over random sampling and traditional mean entropy strategies. The results demonstrate that fewer annotations can still deliver high-quality models, particularly for sparse and challenging datasets. This research highlights the potential of active learning for scalable annotation in audio and time-series data, with important applications in bioacoustic monitoring. Congratulations to Richard Lindholm, Oscar Marklund, Olof Mogren, and John Martinsson for this impactful contribution!"
tags:
- prio
- frontpage
title: Aggregation Strategies for Efficient Annotation of Bioacoustic Sound Events
  Using Active Learning
venue: EUSIPCO 2025
venuelink: https://arxiv.org/abs/2503.02422
venueshort: EUSIPCO

---
