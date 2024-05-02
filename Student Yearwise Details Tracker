class Student:
    rollnos = []
    names = []

    def __init__(self, no, name):
        self.rollno = no
        self.name = name
        Student.rollnos.append(no)
        Student.names.append(name)

    @classmethod
    def y1details(cls):
        return cls.rollnos, cls.names

    @classmethod
    def y2details(cls):
        return cls.rollnos, cls.names

    @classmethod
    def y3details(cls):
        return cls.rollnos, cls.names

studentcount = int(input("How many students are there: "))
y1info = {'rollnos': [], 'names': []}
y2info = {'rollnos': [], 'names': []}
y3info = {'rollnos': [], 'names': []}
while studentcount != 0:
    year = int(input("\n-Enter a year-: "))
    no = int(input("\nEnter a roll number: "))
    name = input("Enter a name: ")
    if year == 1:
        y1 = Student(no, name)
        y1info['rollnos'].append(no)
        y1info['names'].append(name)
    elif year == 2:
        y2 = Student(no, name)
        y2info['rollnos'].append(no)
        y2info['names'].append(name)
    else:
        y3 = Student(no, name)
        y3info['rollnos'].append(no)
        y3info['names'].append(name)
    studentcount -= 1

x = 'Y'
while x == 'Y' or x == 'y':
    print("\n1. year one, 2. year two, 3. year three\n")
    key = int(input('''which year information 
    you like to see?: '''))
    dict = {1: y1info, 2: y2info, 3: y3info}
    print(dict[key])
    print("\nyou want to continue see info?")
    x = input("Yes (Y) / No (N)\n")