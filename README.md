# my personal conveter
print("Please enter name")
user_name=input()
print("Greetings "+user_name+" welcome to your personal unit conerter")
print("Please choose which conversion you would like to perform:")
_conversion_=("1.convert cm to inches\n"
             "2.convert height from feet and inches to cm\n"
             "3.convert cups to ml\n"
             "4.convert grams to ounces\n"
             "5.convert percentage into letter grade,")
print(_conversion_)
print("Choice:")
Choice=int(input())

if Choice ==1:

    print("convert cm to meters")
    def cm_m(a):
        return a/100
    print("meters = "+ str(cm_m(int(input("input in cm: ")))))

elif Choice==2:

        print("convert height from feet and inches to cm \n")
        feet = int(input("enter feet: "))
        inches = int(input("enter inches: "))
        def _height(feet=0,inches=0):
            inches_cm=inches*2.54
            feet_cm=feet*12*2.54
            return inches_cm + feet_cm
        print("height="+str(_height(feet, inches)))

elif Choice==3:

    print("convert cups to ml")
    def ml(b):
        return b*100
    print("milliliters = "+ str(ml(int(input("input in cups: ")))))

elif Choice==4:
    
    print("convert garms into ounces")
    def ounces(c):
        return c/28.35
    print("ounces = "+ str(ounces(float(input("input in grams: ")))))

elif Choice==5:

    print("convert percentage into letter grade")
    
mark = int(input("Enter Marks: "))

def final_grade(x):
    if (x >= 80 and x <= 100):
        grade = 'A'
    elif (x >= 70 and x < 80):
        grade = 'B'
    elif (x >= 60 and x < 70):
        grade = 'C'
    elif (x >= 50 and x < 60):
        grade = 'D'
    elif (x >= 20 and x < 50):
        grade = 'E'
    elif (x >= 0 and x < 20):
        grade = 'F'


    return grade


print('Grade: ' + final_grade(mark));
print('Goodbye')
