# cAdv

### Background
This code implements the cAdv attack in Unrestricted Semantic Adversarial Attacks. cAdv adaptively changes the colors in certain regions of an image to create an adversarial examples. We do not bound Lp Norm but is still able to achieve realistic images.

Original Image of class Umbrella

<img src="test_images/n04507155_191.JPEG" width="224" height="224">

Output Image of class Golfcart

<img src="results/n04507155_191.png">


### Download the pretrained models
```bash
$ sh download_model.sh
```

### Running tests
To run a targeted attack, run the following
```bash
$ python test.py --num_iter 500 --targeted 1 --target 575 --gpu 0
```
num_iter is the number of update steps for the attack. Set targeted to 0 for untargeted attack.

