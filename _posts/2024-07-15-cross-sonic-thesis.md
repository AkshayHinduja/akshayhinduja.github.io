---
title   : "Underwater Localization and Mapping for Cost-Effective Robots"
author  : "<b>Akshay Hinduja</b>"
journal : "PhD Thesis, Carnegie Mellon University, 2024"
teaserurl: "/assets/images/csonic-architecture.webp"
imurl   : "/assets/images/csonic-architecture.webp"
paperurl: "/assets/pdf/Akshay_Hinduja_PhD_Thesis.pdf"
paperlabel: "Thesis (PDF)"
categories: Publication
---

## Summary
The full thesis is available here as a [PDF](/assets/pdf/Akshay_Hinduja_PhD_Thesis.pdf) (81 pages, 4.9 MB).

This thesis addresses localization and mapping for low-cost underwater robots using imaging sonar and acoustics. It spans degeneracy-aware SLAM factors, acoustic pseudoranging for low-power bio-inspired robots, cGAN sonar filtering for occupancy mapping, and pose-supervised sonar image correspondence (SONIC).

The final chapter, *C-SONIC: Cross-Sonar Image Correspondence for Generalized Feature Matching in Imaging Sonars*, extends SONIC across sonars. Sonar images change with the frequency mode, the range settings and the manufacturer's binning, so a network trained on one configuration does not transfer to another. C-SONIC adds a cross-attention module at the encoder level, shown above, so that the feature maps of the two images condition each other before coarse and fine matching. The result is a single model that finds reliable correspondences between images taken with different frequency and range parameters. This opens the possibility of localizing a cheaper vehicle with a lower-cost sonar against a map built by a vehicle with a higher-frequency sonar.

The chapter contributes a cross-sonar matching model that covers most of the Blueprint Subsea Oculus family, together with a framework to train new models on other imaging sonars, and a 550K image-pair dataset with differing frequency and range parameters, pose information and per-frame metadata, including a small subset modeled on the SoundMetrics DIDSON sonar.

<figure class="pub-figure">
  <img src="/assets/images/csonic-matching.webp" alt="Sonar image pairs from a test tank, low frequency on the left and high frequency on the right, with matches drawn by C-SONIC, SONIC and SuperPoint with LightGlue">
  <figcaption>Real-world matching in a test tank. The left image of each pair is in the low frequency mode and the right in the high frequency mode. C-SONIC finds many more correct matches than a retrained SONIC network or SuperPoint with LightGlue.</figcaption>
</figure>

## Citation
```
A. Hinduja, "Underwater Localization and Mapping for Cost-Effective Robots,"
PhD thesis, Carnegie Mellon University, Pittsburgh, PA, July 2024.
```
