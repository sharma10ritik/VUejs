# VUejs
Answeres
#1
list=[10,25,9,13,28,12,23,18,50,83]
for i in list:
    if i%2==0:
        print(i)
       
#2
def MaxLength(arr, n):
	count = 0
	result = 0

	for i in range(0, n):
		if (arr[i] == 0):
			count = 0
		else:
			count+= 1
			result = max(result, count)
		
	return result
arr=[1,0,0,0,0,1,0,0,0,1]
n = len(arr)
print(MaxLength(arr, n))


#3
def Repeat(x):
	ssize = len(x)
	repeated = []
	for i in range(ssize):
		k = i + 1
		for j in range(k, ssize):
			if x[i] == x[j] and x[i] not in repeated:
				repeated.append(x[i])
	return repeated


list1 = [0,1,2,3,4,5,6,7,7,8,9,10]
print (Repeat(list1))

#4


#5

lis = [{ "id" :4,"name" : "abc"},
{ "id" : 10, "name" : "ab2" },
{ "id" : 5, "name" : "abc3" },
{ "id" : 6, "name" : "abc5" }]

print ("sorted list id: ")
print (sorted(lis, key = lambda i: i['id']))

print ("sorted list name: ")
print (sorted(lis, key = lambda i: (i['name'], i['id'])))

print ("The list printed sorting by age in descending order: ")
print (sorted(lis, key = lambda i: i['name'],reverse=True))
