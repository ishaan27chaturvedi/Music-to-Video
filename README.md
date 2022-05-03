# Music-to-Video

Creating music videos from song and their lyrics using VQGANs + CLIP + WAV2CLIP + Laplacian Segmentation. You can see the Google Colab Version [here](https://drive.google.com/drive/folders/1YA8zab3ewMGk1F-hHwky8FTspJxdRqLJ?usp=sharing)

## Description

This study is about making an improvement on the existing Music to Video generation framework, [MUSIC2VIDEO: AUTOMATIC GENERATION OF MUSIC VIDEO WITH FUSION OF AUDIO AND TEXT](https://arxiv.org/pdf/2201.03809.pdf). The original paper's github can be found [here](https://github.com/joeljang/music2video). The framework uses text (lyrics) and audio (song) to generate images, which are converted to videos. <br>
In terms of making improvements to the existing framework, the two concepts are tackled in different aspects. The original video was very stagnant, so I decided to add aesthetic modifiers and video effects like zooming and panning. While experimenting with these effects, it looked random and did not add meaning to the video. Therefore I segmented the audio to understand the repetitive parts of a song, using this information to create patterns with these effects in sync with the rhythm and beats of the song. 


## Outputs
* [version 1](https://www.youtube.com/watch?v=b3xOfeInlOg)
* [version 2](https://www.youtube.com/watch?v=0KMGvdu1IjY&t=6s)
* [version 3](https://youtu.be/ytscibWpAwQ)


## Evaluation & Survey
A survey was conducted to understand if this survey made any improvements. The survey can be found [here](https://docs.google.com/forms/d/1RwW-xCahbAb0tJPz5G5CKOssUIVeKCi9Ptn1KR1iCok/edit) and results of the survey can be found [here - graphical](https://docs.google.com/forms/d/1RwW-xCahbAb0tJPz5G5CKOssUIVeKCi9Ptn1KR1iCok/viewanalytics) and [here - csv](https://docs.google.com/spreadsheets/d/1F_T9DaMp5OdqYO6hEuGw6-t3tHiEVry-Dgf5-51V-nM/edit?usp=sharing). A total of 54 people of different ages, from various countries and professions, participated in this survey.


## Getting Started

### Dependencies

* [VQGAN - Transformers](https://compvis.github.io/taming-transformers/)
* [CLIP](https://openai.com/blog/clip/)
* [WAV2CLIP](https://arxiv.org/abs/2110.11499)
* [Laplacian Segmentation](http://bmcfee.github.io/papers/ismir2014_spectral.pdf)
* Librosa
* Pytorch
* Stegano
* Pandas
* sklearn
* Matplotlib
* [View this notebook cell to see all dependencies](https://colab.research.google.com/drive/11-s8mcnE36g7SCzj4iWAW9qCYrmoWdYp#scrollTo=gKYXIvDhZmEp&line=5&uniqifier=1)

### Installing

* This is Google Colab Notebook that can be imported into your colab or jupyter environment
* Make sure to download the lyrics (csv) and the song (mp3) and place them in an appropriate directory

### Executing program

* The notebook provides a detailed step by step to run the code
* Run it as it is once, then feel free to experiment


## Help

If you've found a new bug, go ahead and create a new GitHub issue. Be sure to include as much information as possible so I can reproduce the bug.


## Authors

The VQGAN+CLIP (z+quantize method) notebook this was based on is by Katherine Crowson (https://github.com/crowsonkb, https://twitter.com/RiversHaveWings). The original BigGAN + CLIP method was made by https://twitter.com/advadnoun. Translated into Spanish and added explanations, and modifications by Eleiber#8347, and the friendly interface was made thanks to Abulafia#3734. Translated back into English, and zoom, pan, rotation, and keyframes features by Chigozie Nri (https://github.com/chigozienri, https://twitter.com/chigozienri). Some UI improvements were made by Justin John (https://github.com/justinjohn0306). A linked helper spreadsheet for creating parameter strings is by Kendrick Feller (https://twitter.com/EphemeralInc)
Music2Video framework was first released by researchers at KAIST: MUSIC2VIDEO: AUTOMATIC GENERATION OF MUSIC VIDEO WITH FUSION OF AUDIO AND TEXT. The paper can be found here: https://arxiv.org/pdf/2201.03809.pdf. The music Segmentation is based on the paper: ANALYZING SONG STRUCTURE WITH SPECTRAL CLUSTERING. Link: https://brianmcfee.net/papers/ismir2014_spectral.pdf


## Version History

* 0.2
    * Added documnetation
    * Various bug fixes and optimizations
* 0.1
    * Initial Release


## License

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments

Prof Simon Colton<br>
Professor of Computational Creativity, Games and Artificial Intelligence<br><br>
Dr Mike Cook<br>
Research Fellow, Computational Creativity
