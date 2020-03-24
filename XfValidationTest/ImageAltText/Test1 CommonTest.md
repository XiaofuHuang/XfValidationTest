# [Test 1] Common Test - Image Alt Text Duplicated

## Test case 1: Images - 6
![test alt text 1](./images/pig.jpg)
<img src = "./images/pig.jpg" alt = "test alt text 1" />
![**test** alt text 1](./images/pig.jpg) 
![<b>test</b> alt text 1](./images/pig.jpg)
![<div><b>test</b></div> alt text 1](./images/pig.jpg) 
![test alt text 1](./images/error.jpg)
![unique alt text 1](./images/pig.jpg)
![](./images/pig.jpg)

## Test case 2: Images in HTML - 3
<IMG src = "./images/pig.jpg" alt = "test alt text 2" />
<div><img alt = "test alt text 2" src = "./images/pig.jpg" /><div>

<div>
<img src = "./images/pig.jpg" 
alt = "test alt text 2" /><div>

<a alt = "unique alt text 2"></a>
<img src = "./images/pig.jpg" />

## Test case 3: Images in Triple Colon Block - 2
::: image type="testimage" source="./images/pig.jpg" alt-text="test alt text 3":::
::: image source="./images/pig.jpg" alt-text="test alt text 3":::
::: image source="./images/pig.jpg" alt-text="unique alt text 3":::

## Test case 4: Images in Code Block - 0
```
::: image type="testimage" source="./images/pig.jpg" alt-text="ignore alt text 4":::
<img src = "./images/pig.jpg" alt = "ignore alt text 4" />
![ignore alt text 4](./images/pig.jpg)
```

~~~
::: image type="testimage" source="./images/pig.jpg" alt-text="ignore alt text 4":::
<img src = "./images/pig.jpg" alt = "ignore alt text 4" />
![ignore alt text 4](./images/pig.jpg)
~~~

## Test case 5: Images in Link -4
[![test alt text 5](./images/pig.jpg)](http://www.microsoft.com)
[abc ![test alt text 5](./images/pig.jpg)](http://www.microsoft.com)
[<img src="./images/pig.jpg" alt="test alt text 5" />](http://www.microsoft.com)
[abc <img src="./images/pig.jpg" alt="test alt text 5" />](http://www.microsoft.com)

## Test case 6: Images in Paragrath - 5
Here are some words. ![test alt text 6](./images/pig.jpg) ![test alt text 6](./images/pig.jpg)
Here are soome words. ![test alt text 6](./images/pig.jpg) <img src = "./images/pig.jpg" alt = "test alt text 6" />

Here is another paragrath. ![test alt text 6](./images/pig.jpg)

Here is another paragrath. <img src = "./images/pig.jpg" alt = "test alt text 6" />

Here is another paragrath. <img src = "./images/pig.jpg" 
alt = "test alt text 6" />

## Test case 7: Images in Other Container Block - 6
### <img src = "./images/pig.jpg" alt = "test alt text 7" />
### ![test alt text 7](./images/pig.jpg)
- <img src = "./images/pig.jpg" alt = "test alt text 7" />
- ![test alt text 7](./images/pig.jpg)

| o                                                       | o |
| --------------------------------------------------------| - |
| ![test alt text 7](./images/pig.jpg)                    | x | 
| <img src = "./images/pig.jpg" alt = "test alt text 7" />| x | 

## Test case 8: Images in Same Line - 1
![test alt text 8](./images/pig.jpg) ![test alt text 8](./images/pig.jpg) 

