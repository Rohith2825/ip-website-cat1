# SSNCE UCS2523 IMAGE PROCESSING AND ANALYSIS

Contrast Enhancement Techniques

## Methods

### Lowlight Image Enhancement

- HE-based
  - BPDHE `bpdhe`
  - DHE A Dynamic Histogram Equalization for Image Contrast Enhancement IEEE TCE 2007
  - DHECI
  - CLAHE (Contrast-limited adaptive histogram equalization) `clahe` `clahe_lab `
  - WAHE (Weighted Approximated Histogram Equalization)
  - CVC (Contextual and Variational Contrast enhancement) [PDF](http://ieeexplore.ieee.org/abstract/document/5773086/)
  - LDR (Layered Difference Representation) [website](http://mcl.korea.ac.kr/cwlee_tip2013/) (CVC, WAHE)
- Retinex-based
  - AMSR
  - LIME [website](http://cs.tju.edu.cn/orgs/vision/~xguo/LIME.htm)
  - NPE [website](http://blog.sina.com.cn/s/blog_a0a06f190101cvon.html)
  - SRIE (Simultaneous Reflection and Illumination Estimation) [CVPR2016](http://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Fu_A_Weighted_Variational_CVPR_2016_paper.html) [website](http://smartdsp.xmu.edu.cn/cvpr2016.html)
  - MF (Multi-deviation Fusion method) [website](http://smartdsp.xmu.edu.cn/weak-illumination.html)
  - `others/robustRetinex.m` Structure-Revealing Low-Light Image Enhancement Via Robust Retinex Model (TIP 2018) [website](https://github.com/martinli0822/Low-light-image-enhancement)
- Dehaze-based
  - Dong
- Camera-Response-Model-based
  - [Ying_2017_ICCV.m](https://github.com/baidut/OpenCE/blob/master/ours/Ying_2017_ICCV.m)
- Fusion-based
  - [Ying_2017_CAIP.m ](https://github.com/baidut/OpenCE/blob/master/ours/Ying_2017_CAIP.m) [python version](https://github.com/AndyHuang1995/New-Image-Contrast-Enhancement)
- Deep-learning-based
  - Learning a Deep Single Image Contrast Enhancer from Multi-Exposure Images _TIP 2018_ [website](https://github.com/csjcai/SICE)
- Others
  - `others/jed.m` JED "[Joint Enhancement and Denoising Method via Sequential Decomposition](http://www.icst.pku.edu.cn/course/icb/Projects/JED.html)" , *ISCAS 2018* [website](https://github.com/tonghelen/JED-Method)

### Related Work

- [Fast Image Processing with Fully-Convolutional Networks (ICCV 2017)](http://www.cqf.io/papers/Fast_Image_Processing_ICCV2017.pdf) (<https://github.com/CQFIO/FastImageProcessing>)
- [Deep Bilateral Learning for Real-Time Image Enhancements (Siggraph 2017)](https://groups.csail.mit.edu/graphics/hdrnet/data/hdrnet.pdf) (<https://github.com/mgharbi/hdrnet>)

## Test Images

- 500 from [Berkeley Segmentation Data Set and Benchmarks 500 (BSDS500)](http://www.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html#bsds500)
- 24 from [Kodak Lossless True Color Image Suite](http://r0k.us/graphics/kodak/)
- 7 of 4.2.0x from [The USCI-SIPI Image Database, Volume 3: Miscellaneous](http://sipi.usc.edu/database/database.php?volume=misc)
- 69 captured images from commercial digital cameras: [Download (15.3 MB)](http://mcl.korea.ac.kr/projects/LDR/LDR_TEST_IMAGES_DICM.zip)
- 4 synthetic images: [Download (445 kB)](http://mcl.korea.ac.kr/projects/LDR/LDR_TEST_IMAGES_SYNTHETIC.zip)

## Metrics

- entropy (DE)
- EME
- AB
- PixDist
- LOE

## Huge thanks to

1. A New Image Contrast Enhancement Algorithm using Exposure Fusion Framework (accepted by CAIP 2017，journal version submitted to IEEE Transactions on Cybernetics)

2. A New Low-Light Image Enhancement Algorithm using Camera Response Model (accepted by ICCV Workshop 2017)
