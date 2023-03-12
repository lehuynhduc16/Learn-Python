# Python_Exercises
This is my Python exercises


# Important Python methods

Định dạng:
    print("%f:%d" %(a, b))
___________________ 01 ___________________

capitalize()	-> Viết hoa chữ cái đầu
	string = "hello world"
	print(string.capitalize())
		-> Hello world"
___________________ 02 ___________________

+) Chuyển str thành lst:
	str = [*str]

+) Chuyển lst thành int:
	q = [str(integer) for integer in p]		#p là list các số nguyên
	k = int("".join(q))	

+) eval()	->	Chuyển lst char thành list int:
	res = [eval(i) for i in lis]			#lis là list các số dạng '0', '1', ...
___________________ 03 ___________________

Random: 
	from random import randrange
	while True:
		x = randrange(-100, 100)
		print(x, end =',')
		if x==50:
			break
print("End")
""" Bài toán trên in ngẫu nhiên các số từ [-100] đến [99] cho đến khi gặp [50] thì dừng """
___________________ 04 ___________________

KEYWORD key = function	-> Sắp xếp theo function
Ví dụ:
Sắp xếp số gần 50 nhất:
	def myfunc(n):
		return abs(n - 50)
	thislist = [100, 50, 65, 82, 23]
	thislist.sort(key = myfunc)
	print(thislist)
		=> [50, 65, 23, 82, 100]
___________________ 05 ___________________

+) Đảo ngược list:
	lst.reverse()

+) Đảo ngược str:
	print(''.join(reversed(str)))
___________________ 06 ___________________

insert (Thêm phần tử vào VỊ TRÍ trong danh sách):
Cách 1:
	lst = [1,2,3,5,-100]
	lst.insert(0, 100)
	lst.insert(4, -10)
	print(lst)
		-> [100],1,2,3,[-10],5,-100

Cách 2:
VD1:	thislist = ["apple", "banana", "cherry"]
	thislist[1:1] = ["blackcurrant", "watermelon"]
	print(thislist)
		-> ['apple', 'blackcurrant', 'watermelon', 'banana', 'cherry']

VD2:	thislist = ["apple", "banana", "cherry"]
	thislist[1:2] = ["blackcurrant", "watermelon"]
	print(thislist)
		-> ['apple', 'blackcurrant', 'watermelon', 'cherry']
___________________ 07 ___________________

Loại bỏ khỏi danh sách
Cách 1: pop
	thislist = ["apple", "banana", "cherry"]
	thislist.pop(1)
	print(thislist)
		-> ['apple', 'cherry']

Cách 2: delete
	thislist = ["apple", "banana", "cherry"]
	del thislist[0]
	print(thislist)
		-> ['banana', 'cherry']
___________________ 08 ___________________

enumerate()
	arr = [1, 3, 8]
	for index, value in enumerate(arr):
		print("index " + str(index) + ": " + str(value))
	->	index 0: 1
		index 1: 3
		index 2: 8
___________________ 09 ___________________

strip	=> Trả về str không có dấu cách
	txt = " Hello World "
	x = txt.strip()
		=> "HelloWorld"
___________________ 10 ___________________

extend - Nối 2 list
	thislist = ["apple", "banana", "cherry"]
	tropical = ["mango", "pineapple", "papaya", 1]
	thislist.extend(tropical)
	print(thislist)
		-> ['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya', 1]
___________________ 11 ___________________

Permutations
	from itertools import permutations
	perm = permutations([1, 2, 3])
	for i in list(perm):
	print (i)
___________________ 12 ___________________

Phương thức split
	s = "Welcome to Codelearn.io!"
	print(s.split(" "))
		-> ['Welcome', 'to', 'Codelearn.io!']

	s = "A1B1C1D1E1"
	print(s.split("1"))
		-> ['A', 'B', 'C', 'D', 'E', '']
___________________ 12 ___________________

Phương thức join (Ngược lại với split)
	lst = ["Welcome", "to", "Codelearn.io!"]
	print(" ".join(lst))
		-> Welcome to Codelearn.io!
	lst = ["A", "B", "C"]
	print("-".join(lst))
		-> A-B-C
___________________ 13 ___________________

Kết hợp join và split
	message = "   Welcome   to Codelearn.io!   "
	print(" ".join(message.split()))
		-> Welcome to Codelearn.io!
___________________ 14 ___________________

Chuyển nhị phân sang thập phân:
	y = input()
	x = int(y, 2)
___________________ 15 ___________________

SET
+) remove///discard đều loại phần từ ra khỏi set
	remove sẽ gây ra lỗi nếu không tồn tại phần tử còn discard thì không
+) update
	s1.updates(s2)	=> Nối s2 vào s1 (s1 là set, s2 là set hoặc list)
+) union	=> Cũng giống update nhưng sẽ gán vào 1 set khác
	s3 = s1.union(s2)
+) z = x.intersection(y)				=> 3 set
	z = x giao y
+) x.symmetric_difference_update(y)	=> 2 set
	x = x hợp y
+) z = x.symmetric_difference(y)		=> 3 set
	z = x + y - (x giao y)
___________________ 16 ___________________






