# Variable Aperture Bokeh Rendering via Customized Focal Plane Guidance

Kang Chen, Shijun Yan, Aiwen Jiang, Han Li, Zhifeng Wang, "Variable Aperture Bokeh Rendering via Customized Focal Plane Guidance", arXiv, 2024 

[![paper](https://img.shields.io/badge/arXiv-Paper-<COLOR>.svg)](https://arxiv.org/abs/)

> **Abstract:** Bokeh rendering is one of the most popular techniques in photography. It can make photographs visually appealing, forcing users to focus their attentions on particular area of image. However, achieving satisfactory bokeh effect usually presents significant challenge, since mobile cameras with restricted optical systems are constrained, while expensive high-end DSLR lens with large aperture should be needed.  Therefore, many deep learning-based computational photography methods have been developed to mimic the bokeh effect in recent years. Nevertheless, most of these methods were limited to rendering bokeh effect in certain single aperture. There lacks user-friendly bokeh rendering method that can provide precise focal plane control and customised bokeh generation. There as well lacks authentic realistic bokeh dataset that can potentially promote bokeh learning on variable apertures. To address these two issues, in this paper, we have proposed an effective controllable bokeh rendering method, and contributed a Variable Aperture Bokeh Dataset (VABD). In the proposed method, user can customize focal plane to accurately locate concerned subjects and select target aperture information for bokeh rendering. Experimental results on public EBB! benchmark dataset and our constructed dataset VABD have demonstrated that the customized focal plane together aperture prompt can bootstrap model to simulate realistic bokeh effect. The proposed method has achieved competitive state-of-the-art performance with only 4.4M parameters, which is much lighter than mainstream computational bokeh models.

<img src = "fig/model.png">

## Effect on VABM

> **Note:** Visual comparison of previous classical models on the VABD dataset. From left to right, the original image with an aperture size of f/16, IR-SDE, BokehOrNot, EBokehNet , our VABM, and the target image . To facilitate the comparison between model performances, the three apertures are taken from the same scene and angle, and from top to bottom are images with aperture sizes of (f/1.8), (f/2.8), and (f/8), respectively. The results are better when viewed enlarged.

<img src = "fig/Constract_in_VABM.png">

> **Note:** Under single-target apertures, quantitative comparison of the performance and parameters with mainstream SOTA models on VABD dataset from
all-in-focus image (of aperture f/16.0) to different bokeh effects (of respective apertures f/1.8, f/2.8, and f/8.0). The best and second-best results are highlighted and
underlined, respectively.

<img src = "fig/score.png">

## Bokeh Dataset
###  Everything is Better with Bokeh!(EBB!)

> **Note:** We will open source our dataset shortly after the paper is published.

### Variable Aperture Bokeh Dataset (VABD)

> **Note:** To get the EBB! dataset, click [here](https://competitions.codalab.org/competitions/24716)