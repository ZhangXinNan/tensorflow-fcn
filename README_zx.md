
训练代码在 [kittiseg](https://github.com/MarvinTeichmann/KittiSeg)

```
(py3.6_tf) zhangxin@zhangxin-AW:~/github/tensorflow-fcn$ python test_fcn32_vgg.py 
Traceback (most recent call last):
  File "test_fcn32_vgg.py", line 15, in <module>
    img1 = scp.misc.imread("./test_data/tabby_cat.png")
AttributeError: module 'scipy.misc' has no attribute 'imread'

```

解决 方法 ：
```
conda install pillow
```

```
Traceback (most recent call last):
  File "test_fcn32_vgg_zx.py", line 35, in <module>
    down_color = utils.color_image(down[0])
  File "/home/zhangxin/github/tensorflow-fcn/utils.py", line 5, in color_image
    import matplotlib as mpl
ModuleNotFoundError: No module named 'matplotlib'

```


```
conda install matplotlib
```