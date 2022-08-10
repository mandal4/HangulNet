## Benchmark data for Hangul OCR

We construct a new benchmarks for Hangul OCR which has intractable number of classes. The proposed benchmark reveals the
**class-imbalance** and **target-class selecting** issues in Hangul OCR. 
<img width="600" alt="hangul" src="https://user-images.githubusercontent.com/34879386/179895019-09831f14-6fe0-438f-8ad6-35a4526d0ff5.png">


> ### Download Link
|Name|Link|Description
|:---:|:---:|:---:|
|AI Hub<br/> train-set|[Website*](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=105#:~:text=316%20%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C%20%3A%2086-,%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C,-%EC%83%98%ED%94%8C%20%EB%8D%B0%EC%9D%B4%ED%84%B0)|It consists of about 100,000 images of Hangul characters. A total of 674,110 text areas are extracted to evaluate the performance of character recognition. Of these, 10,000 are separated into the test set, and the rest are used as a training data.|
|AI Hub<br/> test-set|[Google Drive](https://drive.google.com/file/d/1D4tN_69CRWFPi286fDbxYvntKvo9OkF8/view?usp=sharing)|-|
|MLT-h <br/>test-set|[Google Drive](https://drive.google.com/file/d/1b2PgWI1PybtU4epeljIROpcC_Vo9gEgl/view?usp=sharing)|[MLT](https://rrc.cvc.uab.es/?ch=8) dataset was introduced in ICDAR to resolve the problem of multi-lingual text detection and script identification. We exploit only the Hangul text regions in the MLT17 test-set for the evaluation, and name it as MLT-h. We have found many annotation errors in this data set, we rectified those noisy labels.|
|SFW <br/>test-set|[Google Drive](https://drive.google.com/file/d/1oBFPk3Ke8iLsUfiMAgxCjK_GO-41gAN3/view?usp=sharing)|To emphasize the class-imbalance problem in Korean character recognition, we have synthesized a new dataset containing a large number of minority classes using [SynthTiger](https://github.com/clovaai/synthtiger). The dataset contains a total of 18,831 standard foreign words that are registered in the [National Institute of the Korean Language](https://stdict.korean.go.kr/main/main.do).|
|Unseen Characters <br/>test-set|[Google Drive](https://drive.google.com/file/d/163mrhOq2Pom0Y4CDHC7LqCHHo5yGnvgE/view?usp=sharing)|To evaluate robustness on the unseen characters, we have selected 72 characters in SFW that could not be represented with a common character encoding, and generated an image per character. |

*AI Hub train-set shall be downloaded from the official website. We cropped text regions for training and this dataset will be available soon.

<br/>

> ### Sample images
#### * `AI Hub` 
<img width="300" alt="스크린샷 2022-07-21 오전 11 37 10" src="https://user-images.githubusercontent.com/8290383/180117903-5bfc55a6-969a-4d4e-b4bd-a9f55665a761.png">

#### * `MLT-h`
<img width="150" src="https://user-images.githubusercontent.com/34879386/180130563-3e30cc3b-b0ab-4871-83df-08c1d6b25019.png"> <img width="150" src="https://user-images.githubusercontent.com/34879386/180130579-1ce64a12-6443-488a-ad4f-e934e29ea1ac.png">

#### * `SFW` 
<img width="300" alt="스크린샷 2022-07-21 오전 11 42 29" src="https://user-images.githubusercontent.com/8290383/180118543-7fd931a8-35b1-480e-8c33-53ccb91baef9.png">

#### * `Unseen Characters`
<img width="70" src="https://user-images.githubusercontent.com/34879386/177490243-ae37b295-3a2d-45d4-a8a7-9c4cf34e9510.png"> <img width="70" src="https://user-images.githubusercontent.com/34879386/177490292-99662d7c-62ed-46c1-9f45-ab99e0843312.png"> <img width="70" src="https://user-images.githubusercontent.com/34879386/177490316-f4df4070-e6fe-4f6e-80ea-587fea025410.png">

<br/>

> ### Citation
TODO
