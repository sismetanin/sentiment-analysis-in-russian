# Sentiment Analysis in Russian
This repository contains links to models for sentiment analysis of texts in Russian, which were trained within [Evaluation of Pre-Trained Transformers for Sentiment Analysis of Texts in Russian]() and [Deep Transfer Learning Baselines for Sentiment Analysis in Russian](https://www.sciencedirect.com/science/article/abs/pii/S0306457320309730) articles.

## Evaluation of Pre-Trained Transformers for Sentiment Analysis of Texts in Russian

<table>
<thead>
  <tr>
    <th rowspan="4">Model</th>
    <th rowspan="4">Score<br></th>
    <th rowspan="4">Rank</th>
    <th colspan="12">Dataset</th>
  </tr>
  <tr>
    <td colspan="6">SentiRuEval-2016<br></td>
    <td colspan="2" rowspan="2">RuSentiment</td>
    <td rowspan="2">KRND</td>
    <td rowspan="2">LINIS Crowd</td>
    <td rowspan="2">RuTweetCorp</td>
    <td rowspan="2">RuReviews</td>
  </tr>
  <tr>
    <td colspan="3">TC</td>
    <td colspan="3">Banks</td>
  </tr>
  <tr>
    <td>micro F<sub>1</sub></td>
    <td>macro F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>micro F<sub>1</sub></td>
    <td>macro F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>wighted F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
    <td>F<sub>1</sub></td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>SOTA</td>
    <td>n/s</td>
    <td></td>
    <td>76.71</td>
    <td>66.40</td>
    <td>70.68</td>
    <td>67.51</td>
    <td>69.53</td>
    <td>74.06</td>
    <td>78.50</td>
    <td>n/s</td>
    <td>73.63</td>
    <td>60.51</td>
    <td>83.68</td>
    <td>77.44</td>
  </tr>
  <tr>
    <td>XLM-RoBERTa-Large</td>
    <td>76.37</td>
    <td>1</td>
    <td>82.26</td>
    <td>76.36</td>
    <td>79.42</td>
    <td>76.35</td>
    <td>76.08</td>
    <td>80.89</td>
    <td>78.31</td>
    <td>75.27</td>
    <td>75.17</td>
    <td>60.03</td>
    <td>88.91</td>
    <td>78.81</td>
  </tr>
  <tr>
    <td>SBERT-Large</td>
    <td>75.43</td>
    <td>2</td>
    <td>78.40</td>
    <td>71.36</td>
    <td>75.14</td>
    <td>72.39</td>
    <td>71.87</td>
    <td>77.72</td>
    <td>78.58</td>
    <td>75.85</td>
    <td>74.20</td>
    <td>60.64</td>
    <td>88.66</td>
    <td>77.41</td>
  </tr>
  <tr>
    <td>MBARTRuSumGazeta</td>
    <td>74.70</td>
    <td>3</td>
    <td>76.06</td>
    <td>68.95</td>
    <td>73.04</td>
    <td>72.34</td>
    <td>71.93</td>
    <td>77.83</td>
    <td>76.71</td>
    <td>73.56</td>
    <td>74.18</td>
    <td>60.54</td>
    <td>87.22</td>
    <td>77.51</td>
  </tr>
  <tr>
    <td>Conversational RuBERT</td>
    <td>74.44</td>
    <td>4</td>
    <td>76.69</td>
    <td>69.09</td>
    <td>73.11</td>
    <td>69.44</td>
    <td>68.68</td>
    <td>75.56</td>
    <td>77.31</td>
    <td>74.40</td>
    <td>73.10</td>
    <td>59.95</td>
    <td>87.86</td>
    <td>77.78</td>
  </tr>
  <tr>
    <td>LaBSE</td>
    <td>74.11</td>
    <td>5</td>
    <td>77.00</td>
    <td>69.19</td>
    <td>73.55</td>
    <td>70.34</td>
    <td>69.83</td>
    <td>76.38</td>
    <td>74.94</td>
    <td>70.84</td>
    <td>73.20</td>
    <td>59.52</td>
    <td>87.89</td>
    <td>78.47</td>
  </tr>
  <tr>
    <td>XLM-RoBERTa-Base</td>
    <td>73.60</td>
    <td>6</td>
    <td>76.35</td>
    <td>69.37</td>
    <td>73.42</td>
    <td>68.45</td>
    <td>67.45</td>
    <td>74.05</td>
    <td>74.26</td>
    <td>70.44</td>
    <td>71.40</td>
    <td>60.19</td>
    <td>87.90</td>
    <td>78.28</td>
  </tr>
  <tr>
    <td>RuBERT</td>
    <td>73.45</td>
    <td>7</td>
    <td>74.03</td>
    <td>66.14</td>
    <td>70.75</td>
    <td>66.46</td>
    <td>66.40</td>
    <td>73.37</td>
    <td>75.49</td>
    <td>71.86</td>
    <td>72.15</td>
    <td>60.55</td>
    <td>86.99</td>
    <td>77.41</td>
  </tr>
  <tr>
    <td>MBART-50-Large-Many-to-Many</td>
    <td>73.15</td>
    <td>8</td>
    <td>75.38</td>
    <td>67.81</td>
    <td>72.26</td>
    <td>67.13</td>
    <td>66.97</td>
    <td>73.85</td>
    <td>74.78</td>
    <td>70.98</td>
    <td>71.98</td>
    <td>59.20</td>
    <td>87.05</td>
    <td>77.24</td>
  </tr>
  <tr>
    <td>SlavicBERT</td>
    <td>71.96</td>
    <td>9</td>
    <td>71.45</td>
    <td>63.03</td>
    <td>68.44</td>
    <td>64.32</td>
    <td>63.99</td>
    <td>71.31</td>
    <td>72.13</td>
    <td>67.57</td>
    <td>72.54</td>
    <td>58.70</td>
    <td>86.43</td>
    <td>77.16</td>
  </tr>
  <tr>
    <td>EnRuDR-BERT</td>
    <td>71.51</td>
    <td>10</td>
    <td>72.56</td>
    <td>64.74</td>
    <td>69.07</td>
    <td>61.44</td>
    <td>60.21</td>
    <td>68.34</td>
    <td>74.19</td>
    <td>69.94</td>
    <td>69.33</td>
    <td>56.55</td>
    <td>87.12</td>
    <td>77.95</td>
  </tr>
  <tr>
    <td>RuDR-BERT</td>
    <td>71.14</td>
    <td>11</td>
    <td>72.79</td>
    <td>64.23</td>
    <td>68.36</td>
    <td>61.86</td>
    <td>60.92</td>
    <td>68.48</td>
    <td>74.65</td>
    <td>70.63</td>
    <td>68.74</td>
    <td>54.45</td>
    <td>87.04</td>
    <td>77.91</td>
  </tr>
  <tr>
    <td>MBART-50-Large</td>
    <td>69.46</td>
    <td>12</td>
    <td>70.91</td>
    <td>62.67</td>
    <td>67.24</td>
    <td>61.12</td>
    <td>60.25</td>
    <td>68.41</td>
    <td>72.88</td>
    <td>68.63</td>
    <td>70.52</td>
    <td>46.39</td>
    <td>86.48</td>
    <td>77.52</td>
  </tr>
</tbody>
</table>

## Deep Transfer Learning Baselines for Sentiment Analysis in Russian

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

### Sentiment Datasets in Russian
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


### Fine-Tuned Models
To download fine-tuned models for Russian, please follow the link [https://yadi.sk/d/Xp5vLG_5xCQL-Q](https://yadi.sk/d/Xp5vLG_5xCQL-Q).

### Citation
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

# License
See [LICENSE](LICENSE.txt).
