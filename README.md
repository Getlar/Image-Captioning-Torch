# FlickR-8 Image Captioning using PyTorch

This repository contains a simple Image Captioning model using a **SENet Encoder** and a **Transformer Decoder**.

The model was trained on the training and test set of the original **FlickR-8** dataset (7000). Validation set was used for hyperparameter tuning (1000).

The test set is a custom set of manually annotated images by me. (175)

No lemmatization was used, only stopword removal and some basic cleaning. (wanted to create captions that are close to sentences)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1FWzczDZsEEqFfk7SWBkXLmqCeUOJZJjt#scrollTo=tdy3SNKxf0uI)

### Results on the validation set:

| BLEU - 1 | BLEU - 2 | BLEU - 3 | BLEU - 4 |
| -------- | -------- | -------- | -------- |
| 48.57    | 30.66    | 18.68    | 10.73    |

### Results on the test set:

| BLEU - 1 | BLEU - 2 | BLEU - 3 | BLEU - 4 |
| -------- | -------- | -------- | -------- |
| 27.75    | 8.43     | 1.98     | 0.04     |

#### Some examples:

```
Predicted Caption:
man in red is skiing in the snow

Actual Caption:
man skiing down snowy mountain slope
person in red pants snowboarding
skier moving fast on powder snow
snowcovered slope with downhill skier
man wearing helmet skiing in snow
```

```sh
Predicted Caption:
person is skiing down snowy hill

Actual Caption:
person snowboarding down snowy hill
snowboarder sliding on snow creating spray
man wearing dark outfit snowboarding
snowboarder making turn on snowy slope
action shot of snowboarder on mountain
```

```sh
Predicted Caption:
man is climbing on rock

Actual Caption:
three people climbing rocky mountain side
climbers wearing helmets scaling steep cliff
group hiking up rocky terrain together
persons attached to ropes climb grey rock
team wearing blue yellow and grey climb outdoors
```
