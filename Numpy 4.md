# Numpy
___
## Array :
به مثل لیست است اما فرق ان 
- تمام خانه های ان از یک نوع دیتا تایپ است
- وقتی ساخته شد اندکس به ان اضافه یا کم کرده نمیتوانیم اما مقدار خانه را میشه تغییر داد
- سرعت دستزسی به ان خیلی بیشتر است
- به مثل یک متریکس به ان دیده میشود
  
```python
import numpy as np
array = np.array([1,2,3])

print(array + 2) #----->  [3 4 5]
print([1,2,3] + 2) #----->  error

```

| method or attribute | perfomation                                                     | Syntax                             | information                                                                             |     |     |
| ------------------- | --------------------------------------------------------------- | ---------------------------------- | --------------------------------------------------------------------------------------- | --- | --- |
| size                | تعداد تمام اندکس ها را بر میگردان                              | array.size                         |                                                                                         |     |     |
| ndim                | تعداد بعد ها                                                   | array.ndim                         |                                                                                         |     |     |
| shap                | (a , b , c) , (dimention, row, culmn) اگر دو بعدی باشد          | array.shap                         | اگر بیشتر از دو بعد بود (تعداد بلوک‌ها, تعداد سطر در هر بلوک, تعداد ستون در هر سطر)<br> |     |     |
| zeros               | ساختن مریکس صفزی                                                | np.zeros((a, b. c),       np.int_) | (تعداد بلوک‌ها, تعداد سطر در هر بلوک, تعداد ستون در هر سطر)                             |     |     |
| ones                | ساختن array که همه اندکس ان یک است                              | np.ones((a, b, c), np.int_)        |                                                                                         |     |     |
| full                | ساختن array که همه اندکس ان x است                               | np.full((a, b, c), x, np.int_)     |                                                                                         |     |     |
| random.random       | عدد رندوم میدهد بین (صفر - یک)  n دانه                          | np.random,random(n)                |                                                                                         |     |     |
| reshape             | دوباره shape را تغییر میدهد اما ذخیره نمیکند                    | array.reshape((a, b))              | (row, culmn)                                                                            |     |     |
| resize              | دوباره shape را تغییر میدهد و ذخیره میکند                       | array.resize((a, b))               |                                                                                         |     |     |
| linspace            | یک array میدهد که از a شروع میشود تا b و فاصله بین دو عدد x است | np.linspace(a, b, x)               |                                                                                         |     |     |
```python
import numpy as np
```
## shape & len() & ndim & shap
```python 
array = np.array([[1,2],[3,4]])
array.size #----> 4
len(array) #----> 2
array.ndim #----> 2
array.shape #----> (2,2)

ary = np.array([[[1, 2]], [[3, 4]],[[3, 4]], [[5, 6]]])
ary.ndim #----> 3
ary.shape #----> (4,1,2)


```
## zeros & ones & full & random.random
```python
zero = np.zeros(10, np.int_) #----> [0 0 0 0 0 0 0 0 0 0]
one = np.ones(10, np.int_) #----> [1 1 1 1 1 1 1 1 1 1]
ful = np.full(10, 5, np.int_) # [5 5 5 5 5 5 5 5 5 5]
random = np.random.random(5) #----> [3.8773  8.73845 3.49854 7.36802 6.2528]
```
## reshape & resize & linspace
```python
array = np.array([1,2,3,4,5,6])
print(array.reshape((3,2))) 
 #[[1 2]
 # [3 4]
 #[5 6]]
array.resize((3,2))
print(array)
 #[[1 2]
 # [3 4]
 #[5 6]]
ary = np.linspace(0,20,6)
print(ary) #----> [ 0.  4.  8. 12. 16. 20.]
