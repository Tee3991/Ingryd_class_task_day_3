# Ingryd_class_task_day_3
Writing a python program that calculate the mean,median ....
## The Mean
student_Temp= [21,32,33,34,25,30,22,31,36,25,36,23,20,37,27,19,28,29,39,40,33]

#mean of student_temp = sum of temp/len of student_temp

mean_temp = round(sum(student_Temp)/len(student_Temp),2)

print(f'The mean of the student temprature is : {mean_temp}')
output: The mean of the student temprature is : 29.52

## median of student_temp
student_Temp.sort()

median_position = len(student_Temp)/2 

print(student_Temp)

print(median_position) #this gives the position of the median
print(f'The median of thhe student temprature is : {student_Temp[9]}')
output:[19, 20, 21, 22, 23, 25, 25, 27, 28, 29, 30, 31, 32, 33, 34, 36, 36, 37, 39, 40]
10.0
The median of thhe student temprature is : 29

## range = max(student_temp) - min(student_Temp)

range_std_temp = max(student_Temp) - min(student_Temp)

print(f'The range of the student temperature is : {range_std_temp}')
output:The range of the student temperature is : 21
## mode of stdnt_temp
a = (student_Temp); print(f'the mode of student temprature is: {max(set(a), key=a.count)}') 
output:the mode of student temprature is: 33

## variance
def variance(student_Temp):
    n = len(student_Temp)
    mean = sum(student_Temp) / n
    deviations = [(x - mean_temp)**2  for x in data]
    variance = sum(deviations) / n
    return round(variance,2)
variance(student_Temp)
output:143.63

## standard dev
def stdev(student_Temp):
    import math
    var = variance(student_Temp)
    std_dev = math.sqrt(var)
    return round(std_dev,2)
stdev(student_Temp)
output:11.98

