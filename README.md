<div align="center">

<samp>
<h2> SurgFusion-Net: Diversified Adaptive Multimodal Fusion Network for Surgical Skill Assessment </h2>
</samp> 

| **[[```arXiv```](<https://arxiv.org/abs/2603.00108>)]** | **[[```Paper```](<https://ieeexplore.ieee.org/document/11647247>)]** |
|:-------------------:|:-------------------:|

</div> 

## SurgFusion-Net Architecture
<div align='center'>
<img src='https://github.com/HRL-Mike/SurgFusion-Net/blob/main/assets/SFN-archi.png' width=750>
</div>

## About RAH-skill and RARP-skill Datasets
The RAH-skill Dataset consists of 37 videos of the vaginal vault closure phase from Robot-assisted Hysterectomy (RAH) cases collected at University College London Hospital and Yeovil Hospital under ethical approval and patient consent (IRAS ID: 309024). Each video corresponds to a single patient case. Videos were recorded at 30 Hz and stored in “.mp4” format. Each video was segmented into three phases: right angle securement, middle section closure, and left angle securement. Non-suturing frames were removed, and each phase was scored using the [M-GEARS](https://pubmed.ncbi.nlm.nih.gov/39106003/) tool.
All videos were blindly double-annotated by two trained surgeons with 90% or higher inter-rater agreement on pre-validated videos. Final scores represent the mean of the two raters, yielding 110 M-GEARS scores ranging from 14 to 30 across all phases, with strong inter-rater reliability (Spearman rho: $\rho$ = 0.756, 95\% CI [0.369, 0.908], p = 0.002).

The RARP-skill dataset contains 33 videos, a subset of the open-source [SAR-RARP50](https://arxiv.org/abs/2401.00496) dataset, of dorsal venous complex ligation from Robot-Assisted Radical Prostatectomy (RARP) collected at University College Hospital (Westmoreland Street, London, UK). Each video corresponds to a single patient case. Videos were recorded at 60 Hz and stored in “.avi” format. Based on video quality, 33 videos were selected for annotation. A total of 20 videos were blindly double-annotated by a trained and a resident surgeon, with the rest annotated by the trained surgeon and reviewed by the resident surgeon. Inter-rater agreement (85\%) was established on JIGSAWS suturing videos and discrepancies were resolved through joint review to reach consensus. This yielded 33 M-GEARS scores ranging from 18 to 28. Strong inter-rater reliability was confirmed on the 20 videos for both absolute M-GEARS scores (Spearman rho: $\rho$ = 0.7026, 95\% CI [0.3774, 0.8735], p $<$ 0.001) and score ranking (Spearman rho: $\rho$ = 0.7281, 95\% CI [0.4214, 0.8854], p $<$ 0.001)

## How to Download RARP-skill Dataset

## How to Download RAH-skill Dataset


## Training Command:


## Acknowledgement
The implementation of PitVQA++ relies on resources from <a href="https://github.com/salesforce/BLIP">BLIP</a>, <a href="https://github.com/huggingface/transformers">Huggingface Transformers</a>, <a href="https://github.com/rwightman/pytorch-image-models/tree/master/timm">timm</a> and our previous work [PitVQA](https://github.com/mobarakol/PitVQA). We thank the original authors for their open-sourcing.

## Citation
If you use the data and code for your research, please cite our paper.
```bibtex
@article{he2026surgfusion,
  title={SurgFusion-Net: Diversified Adaptive Multimodal Fusion Network for Surgical Skill Assessment},
  author={He, Runlong and Tesfai, Freweini M. and Boal, Matthew W. E. and Sirajudeen, Nazir and Anastasiou, Dimitrios and Xu, Jialang and Hoque, Mobarak I. and Edwards, Philip J. and Kelly, John D. and Sridhar, Ashwin and Kadkhodamohammadi, Abdolrahim and Chandrasekaran, Dhivya and Clarkson, Matthew J. and Stoyanov, Danail and Francis, Nader and Mazomenos, Evangelos B.},
  journal={IEEE Transactions on Medical Imaging},
  year={2026},
  publisher={IEEE},
  doi={10.1109/TMI.2026.3722251},
  note={Early Access}
}
```
