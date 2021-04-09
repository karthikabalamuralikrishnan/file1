# file1
num_students = int(input("Please enter number of students:")) 
student_info = {} 
student_data = ['Math marks : ', 'Physics marks : ', 'Chemistry marks : '] 
for i in range(num_students): 
  student_name = input("Name :") 
  student_info[student_name] = {} 
  for entry in student_data: 
    student_info[student_name][entry] = float(input(entry)) 
#storing the marks entered as integers to perform arithmetic operations later on. 
#Now printing student_info
print("Please enter student name ?") 
name = input("Student name : ") 
if name in student_info.keys(): 
  print("Average student marks : ", sum(student_info[name].values())/3.0) 
else: 
  print("please enter valid name")
