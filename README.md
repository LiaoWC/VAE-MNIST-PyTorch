
## 訓練版本 1

> KLD loss weight 漸升版。

## Loss

KLD loss 權重在 200 epoch 前為 0，200 epochs 後權重為：

![](img/img0.png)

#### KLD Loss

![](img/img1.svg)

#### Reconstruction Loss

![](img/img2.svg)

#### Total Loss

![](img/img3.svg)

## Epoch 180

![](img/img4.png)

## Epoch 220

![](img/img5.png)

![](img/img6.png))

放大來看

![](img/img7.png)

![](img/img8.png)

## Epoch 240

![](img/img9.png)

## Epoch 500

![](img/img10.png)

## Epoch 1000

![](img/img11.png)

## Epoch 2200

![](img/img12.png)

![](img/img13.png)

![](img/img14.png)

## 訓練版本 2

> Cyclically 更新 KLD loss weight，並且手動調整最大 weight。

### Epoch 100

![](img/img15.png)

↑ Testing

![](img/img16.png)

↑ 兩維度 -1~1 產生 41×41 張圖片

![](img/img17.png)

↑ 所有資料化成 Latent Code

### Epoch 2300

#### Testing

![](img/img18.png)

#### Loss

![](img/img19.svg)

↑ KLD Loss

![](img/img20.svg)

↑ KLD Loss Weight

![](img/img21.svg)

↑ Reconstruction Loss

![](img/img22.svg)

↑ Total Loss

#### 兩維度 -1~1 產生 41×41 張圖片

![](img/img23.png)

#### 所有資料化成 Latent Code

![](img/img24.png)

![](img/img25.png)

↑ 點點尺寸縮小並過濾至只有 -300~300