# Numpy
___
## Array :
به مثل لیست است اما فرق ان 
- تمام خانه های ان از یک نوع دیتا تایپ است
- وقتی ساخته شد اندکس به ان اضافه یا کم کرده نمیتوانیم اما مقدار خانه را میشه تغییر داد
- سرعت دستزسی به ان خیلی بیشتر است
- به مثل یک متریکس به ان دیده میشود
  
`import numpy as np`
`array = np.array([1'2'3])`

`print(array + 2)` -----> [3 4 5]
`print([1,2,3] + 2)` -----> error


| method or attribute | perfomation                            | Syntax                            | information             |
| ------------------- | -------------------------------------- | --------------------------------- | ----------------------- |
| size                | تعداد تمام اندکس ها را بر میگردانn     | array.size                        |                         |
| ndim                | تعداد اندکس                            | array.ndim                        |                         |
| ship                | {a , b , c} , {dimention, row, culmn}  | array.ship                        |                         |
| zeros               | ساختن مریکس صفزی                       | np.zeros((a, b. c),       np.int) | (dimention, row, culmn) |
| ones                | ساختن array که همه اندکس ان یک است     | np.ones((a, b, c), np.int)        |                         |
| full                | ساختن array که همه اندکس ان x است      | np.full((a, b, c), x, np.int)     |                         |
| random.random       | عدد رندوم میدهد بین (صفر - یک)  n دانه | np.random,random(n)               |                         |
|                     |                                        |                                   |                         |

