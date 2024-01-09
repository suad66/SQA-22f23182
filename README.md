def calculate_grade(d):
    if d > 90:
        return 'A'
    elif d > 80:
        return 'B'
    elif d > 70:
        return 'C'
    elif d > 60:
        return 'D'
    else:
        return 'F'

def predict_performance(d):
    # This function predicts performance based on scores
   if d > 75:
       performance = 'High'
   elif d > 50:
       performance = 'Medium'
   else:
       performance = 'Low'
   return performance
# Example student scores
d = 0

while (True):    
    print ("\tPlease Enter marks of Student Marks =")
    d = int (input ())
    grades = calculate_grade(d)
    performance_prediction = predict_performance(d)
# Output the results
    print("\tGrades:", grades)
    print("\tPerformance Predictions:", performance_prediction)
    print ("\tDo you want to Continue Pres Y/N")
    choice = str (input())
    if (choice == "N"):
        break
    
