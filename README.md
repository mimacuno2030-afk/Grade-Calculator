# Grade-Calculator

print("=== Grade Calculator ===")

# Ask how many subjects
num_subjects = int(input("Enter number of subjects: "))

total = 0

# Get grades
for i in range(1, num_subjects + 1):
    grade = float(input(f"Enter grade for subject {i}: "))
    total += grade

# Calculate average
average = total / num_subjects

# Determine letter grade
if average >= 90:
    letter = "A"
elif average >= 80:
    letter = "B"
elif average >= 70:
    letter = "C"
elif average >= 60:
    letter = "D"
else:
    letter = "F"

# Display results
print("\n=== Results ===")
print(f"Average Grade: {average:.2f}")
print(f"Letter Grade: {letter}")
