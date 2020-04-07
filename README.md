# COVID19 Language Resources: Datasets
We are collecting the COVID-19 Language-based AI research papers and datasets. If you have paper to recommend or any suggestions, please feel free to contact us.

#### 1. We released a Chinese medical dialogue dataset about COVID-19 and other types of pneumonia. Patients who are concerned that they may be infected by COVID-19 or other pneumonia consult doctors and doctors provide advice. There are *12789* consultations and each consultation has at least 8 senteces.
The whole file is a python list, and each item in the list is a dictionary，as shown below

## Example
[{'id': 'dis', 'text': '医生您好！发烧两天，最高38.7，头痛，全身酸疼乏力，不咳嗽，不流涕，呼吸无异常。现已退烧，头痛基本消失，但是咽喉及中央气管略有灼烧疼，胸口两侧对称跳着疼，头顶头皮一处跳着疼，左腹一处偶尔也跳着疼，无力，不爱吃饭。无湖北接触史，偶尔外出去超市采购，都戴口罩。前段时间压力大，连续一周熬夜做文字工作。请问这是什么情况啊？是不是新冠肺炎？谢谢医生！（男，35岁）'} <br>
{'id': 'doc', 'text': '您好！这种情况有多久了？'} <br>
{'id': 'doc', 'text': '有没有鼻塞？'} <br>
{'id': 'doc', 'text': '咳嗽？气喘？'} <br>
{'id': 'dis', 'text': '三天了，前两天发烧头疼，今天不烧了'} <br>
{'id': 'dis', 'text': '只在第一天晚上鼻塞过，不咳嗽，不气喘'} <br>
{'id': 'doc', 'text': '咳嗽？'} <br>
{'id': 'doc', 'text': '咳嗽？'} <br>
{'id': 'doc', 'text': '胸痛？'} <br>
{'id': 'doc', 'text': '应该是病毒性感冒'}<br>
{'id': 'doc', 'text': '不像肺炎'}<br>
{'id': 'doc', 'text': '建议多喝水，休息，按时吃感冒药如日夜百服宁片或泰诺感冒片，另外可吃些含片，清火的药如清开灵或熊胆胶囊等。'}<br>
{'id': 'dis', 'text': '不咳嗽，胸口两侧对称地方跳着疼，头皮，左腹各有跳着疼'}<br>
{'id': 'dis', 'text': '对了，退烧后，左嘴角上下起了一些疱疹'}<br>
{'id': 'doc', 'text': '还是考虑病毒性感冒'}<br>
{'id': 'dis', 'text': '病毒性感冒是不是传染？家里有孩子，请问怎样防护？'}<br>
{'id': 'doc', 'text': '感冒会传染，'}<br>
{'id': 'doc', 'text': '可以适当隔离，戴口罩'}<br>
{'id': 'dis', 'text': '好的，谢谢医生！'}<br>
{'id': 'doc', 'text': '不客气'}]<br>

The code for read "COVID_Dialogue_Dataset.pk":<br>
```python
with open('COVID_Dialogue_Dataset1.pk','rb') as f:
    data = pickle.load(f)
data[0]
```
The dataset is built from [chunyu](https://www.chunyuyisheng.com/) and all copyrights of the data belong to [chunyu](https://www.chunyuyisheng.com/).<br>

If you find this dataset useful, please cite:

```
@article{liu2020Covid19_Dialog,
  title={Chinese_Covid19_Dialog: Chinese Medical Dialogue Datasets about COVID-19},
  author={Wenge Liu and Lin Xu and Jianheng Tang and Shuai Lin and Junfan Lin and Xiaodan Liang},
  journal={ https://github.com/lwgkzl/COVID19_Language_Understanding}, 
  year={2020}
}
```

# COVID19 Language Resources: Papers
TODO.
