PASSING_GRADE = 60.0
MAX_ASSIGNMENT_SCORE = 100.0

# Weights for grade components
ASSIGNMENT_WEIGHT = 0.2
MIDTERM_WEIGHT = 0.3
FINAL_EXAM_WEIGHT = 0.5

# Prompt for student's name
student_name = input("rodneycabauatan")

# Prompt for scores
assignment_score = float(input("Enter the Assignment score (e.g., 85.5): "))
midterm_score = float(input("Enter the Midterm score (e.g., 78.0): "))
final_exam_score = float(input("Enter the Final Exam score (e.g., 92.5): "))


# Calculate final grade
final_grade = (
    assignment_score * ASSIGNMENT_WEIGHT +
    midterm_score * MIDTERM_WEIGHT +
    final_exam_score * FINAL_EXAM_WEIGHT
)

# Determine pass/fail status
status = "Passed" if final_grade >= PASSING_GRADE else "Failed"

# Display results
print(f"\nStudent Name: {rods}")
print(f"Assignment Score: {assignment_score:.1f}")
print(f"Midterm Score: {midterm_score:.1f}")
print(f"Final Exam Score: {final_exam_score:.1f}")
print(f"Final Grade: {final_grade:.1f}")
print(f"Status: {status}")
