# Deep Transfer Learning Baselines for Sentiment Analysis in Russian

This repository contains the fine-tuned Multilingual Bidirectional Encoder Representations from Transformers (M-BERT), RuBERT, and two versions of Multilingual Universal Sentence Encoder (M-USE) for sentiment classification in Russian referenced in [Deep Transfer Learning Baselines for Sentiment Analysis in Russian](https://www.sciencedirect.com/science/article/abs/pii/S0306457320309730).

<div class="tg-wrap"><table>
<thead>
  <tr>
    <th>Dataset</th>
    <th>Measure</th>
    <th>Current SOTA</th>
    <th>M-BERT</th>
    <th>RuBERT</th>
    <th>M-USE-CNN</th>
    <th>M-USE-Trans</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="3">SentiRuEval-2016 TC</td>
    <td>F<sub>1</sub></td>
    <td>68.42</td>
    <td>66.29<br></td>
    <td><b>70.68</b><br></td>
    <td>63.64</td>
    <td>68.27</td>
  </tr>
  <tr>
    <td>macro F<sub>1</sub><sup>PN</sup></td>
    <td>66.07</td>
    <td>61.78</td>
    <td><b>66.40</b></td>
    <td>58.97</td>
    <td>62.77</td>
  </tr>
  <tr>
    <td>micro F<sub>1</sub><sup>PN</sup></td>
    <td>74.11</td>
    <td>72.45</td>
    <td><b>76.71</b></td>
    <td>71.31</td>
    <td>75.00</td>
  </tr>
  <tr>
    <td rowspan="3">SentiRuEval-2016 Banks</td>
    <td>F<sub>1</sub></td>
    <td><b>74.06</b></td>
    <td>65.31</td>
    <td>72.83</td>
    <td>66.71</td>
    <td>72.40</td>
  </tr>
  <tr>
    <td>macro F<sub>1</sub><sup>PN</sup></td>
    <td><b>69.53</b></td>
    <td>58.00</td>
    <td>65.89</td>
    <td>58.73</td>
    <td>65.04</td>
  </tr>
  <tr>
    <td>micro F<sub>1</sub><sup>PN</sup></td>
    <td><b>71.76</b></td>
    <td>60.52</td>
    <td>68.43</td>
    <td>62.41</td>
    <td>68.21</td>
  </tr>
  <tr>
    <td rowspan="3">SentiRuEval-2016 TC</td>
    <td>F<sub>1</sub></td>
    <td><b>68.54</b></td>
    <td>60.47</td>
    <td>64.39</td>
    <td>60.57</td>
    <td>64.28</td>
  </tr>
  <tr>
    <td>macro F<sub>1</sub><sup>PN</sup></td>
    <td><b>63.47</b></td>
    <td>53.16</td>
    <td>57.76</td>
    <td>52.37</td>
    <td>57.60</td>
  </tr>
  <tr>
    <td>micro F<sub>1</sub><sup>PN</sup></td>
    <td><b>67.51</b></td>
    <td>57.03</td>
    <td>61.38</td>
    <td>57.76</td>
    <td>61.18</td>
  </tr>
  <tr>
    <td rowspan="3">SentiRuEval-2016 Banks</td>
    <td>F<sub>1</sub></td>
    <td><b>79.51</b></td>
    <td>67.65</td>
    <td>70.58</td>
    <td>66.32</td>
    <td>69.62</td>
  </tr>
  <tr>
    <td>macro F<sub>1</sub><sup>PN</sup></td>
    <td><b>67.44</b></td>
    <td>56.97</td>
    <td>60.95</td>
    <td>54.74</td>
    <td>59.12</td>
  </tr>
  <tr>
    <td>micro F<sub>1</sub><sup>PN</sup></td>
    <td><b>70.09</b></td>
    <td>59.32</td>
    <td>63.33</td>
    <td>57.61</td>
    <td>62.17</td>
  </tr>
  <tr>
    <td>RuSentiment</td>
    <td>F<sub>1</sub></td>
    <td>n/s</td>
    <td>71.37</td>
    <td><b>72.03</b></td>
    <td>66.27</td>
    <td>68.60</td>
  </tr>
  <tr>
    <td></td>
    <td>weighted F<sub>1</sub></td>
    <td><b>78.50</b></td>
    <td>75.13</td>
    <td>75.71</td>
    <td>71.05</td>
    <td>73.42</td>
  </tr>
  <tr>
    <td>Kaggle Russian News Dataset</td>
    <td>F<sub>1</sub></td>
    <td>70.00</td>
    <td>71.36</td>
    <td><b>73.63</b></td>
    <td>71.27</td>
    <td>72.66</td>
  </tr>
  <tr>
    <td>LINIS Crowd</td>
    <td>F<sub>1</sub></td>
    <td>37.29</td>
    <td>42.73</td>
    <td><b>60.51</b></td>
    <td>56.34</td>
    <td>56.95</td>
  </tr>
  <tr>
    <td>RuTweetCorp (binary)</td>
    <td>F<sub>1</sub></td>
    <td>75.95</td>
    <td>83.04</td>
    <td><b>83.69</b></td>
    <td>81.34</td>
    <td>83.17</td>
  </tr>
  <tr>
    <td>RuTweetCorp (trinary)</td>
    <td>F<sub>1</sub></td>
    <td>78.1</td>
    <td>80.10</td>
    <td><b>80.79</b></td>
    <td>78.39</td>
    <td>79.69</td>
  </tr>
  <tr>
    <td>RuReviews</td>
    <td>F<sub>1</sub></td>
    <td>75.45</td>
    <td>77.31</td>
    <td><b>77.44</b></td>
    <td>76.63</td>
    <td>76.94</td>
  </tr>
</tbody>
</table></div>

SOTA approaches for RuReviews, RuSentiment, Kaggle Russian News Dataset, and RuTweetCorp were described in papers [(Smetanin and Komarov, 2019)](https://ieeexplore.ieee.org/document/8807792), [(Baymurzina et al., 2019)](http://www.dialog-21.ru/media/4586/baymurzinadrplusetal-015.pdf), [(Shalkarbayuli et al., 2018)](https://iopscience.iop.org/article/10.1088/1742-6596/1117/1/012002), and [(Rubtsova, 2018)](https://www.mdpi.com/2078-2489/9/8/184), consequently. The SOTA approach for LINIS Crowd was implemented based on the paper [(Koltsova et al., 2016)](https://publications.hse.ru/en/chapters/192815883).

## Sentiment Datasets in Russian
Despite the fact that Russian is one of the most common languages in the World Wide Web, generally it is not as well-resourced as the English language, especially in the field of sentiment analysis. Even though many studies aim at sentiment classification, only few of them makes their datasets publicly available for the research community.


| Dataset  | Classes | Average lengths | Max lengths | Train Samples | Test Samples | Overall Samples | Download Link |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| SentiRuEval-2016 [(Loukachevitch and Rubtsova, 2016)](http://www.dialog-21.ru/media/3410/loukachevitchnvrubtsovayv.pdf) | 3 | 87.0928 | 172 | 18,035 | 5,560 | 23,595 | [Project page](http://www.dialog-21.ru/evaluation/2016/sentiment/) |
| SentiRuEval-2015 Subtask [(Loukachevitch et al., 2015)](http://www.dialog-21.ru/media/1024/loukachevitchnvetal.pdf) | 3 | 81.4986 | 172 | 8,580  | 7,738 | 16,318 | [Project page](http://www.dialog-21.ru/evaluation/2015/sentiment/) |
| RuTweetCorp (Rubtsova, 2013)| 3 | 89.1725 | 189 | n/a | n/a | 334836 | [Project page](http://study.mokoron.com) |
| LINIS Crowd [(Koltsova et al., 2016)](https://publications.hse.ru/en/chapters/192815883)| 5  |  n/a  |  n/a  |  n/a  |  n/a  |  n/a  | [Project page](http://linis-crowd.org) |
| RuSentiment [(Rogers et al., 2018)](https://www.aclweb.org/anthology/C18-1064/)| 5 | 82.0279 | 800 | 28218 | 2967 | 31185 | [Project page](http://text-machine.cs.uml.edu/projects/rusentiment) |
| Kaggle Russian News Dataset | 3 | 3911.8501 | 381498 | n/a | n/a | 8263 | [Kaggle page](https://www.kaggle.com/c/sentiment-analysis-in-russian) |
| RuReviews [(Smetanin and Komarov, 2019)](https://ieeexplore.ieee.org/document/8807792) | 3 | 130.0693 | 1007 | n/a | n/a | 90,000 | [GitHub page](https://github.com/sismetanin/rureviews) |


## Fine-Tuned Models
To download fine-tuned models for Russian, please follow the link [https://yadi.sk/d/Xp5vLG_5xCQL-Q](https://yadi.sk/d/Xp5vLG_5xCQL-Q).

## Citation
```
@article{Smetanin2020Deep,
  title = {Deep transfer learning baselines for sentiment analysis in Russian},
  author = {Sergey Smetanin and Mikhail Komarov},
  journal = {Information Processing & Management},
  volume = {58},
  number = {3},
  pages = {102484},
  year = {2021},
  issn = {0306-4573},
  doi = {https://doi.org/10.1016/j.ipm.2020.102484},
  url = {https://www.sciencedirect.com/science/article/pii/S0306457320309730}
}
```

## Documentation and How to report bugs
* TensorFlow documentation: [https://www.tensorflow.org/api_docs](https://www.tensorflow.org/api_docs).
* Scikit-learn documentation: [http://scikit-learn.org/stable/documentation.html](http://scikit-learn.org/stable/documentation.html). 
* BERT repository: [https://github.com/google-research/bert](https://github.com/google-research/bert). 
* If you find any issues, please open a bug here on GitHub.

## License
See [LICENSE](LICENSE.txt).
