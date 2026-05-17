# Student Future Predictor (No external libraries)

name = input("Enter student name: ")
study_hours = int(input("Enter daily study hours: "))
attendance = int(input("Enter attendance percentage: "))

# Prediction formula
future_score = (study_hours * 10) + (attendance * 0.6)

# Limit score to 100
if future_score > 100:
    future_score = 100

# Output
print("\n----- RESULT -----")
print("Student Name:", name)
print("Study Hours:", study_hours)
print("Attendance:", attendance, "%")
print("Predicted Future Score:", future_score)

# ---------------- TEXT GRAPH ----------------
print("\n----- GRAPH VIEW -----")

print("Study Hours   :", "*" * study_hours)
print("Attendance    :", "*" * int(attendance / 2))
print("Future Score  :", "*" * int(future_score / 5))