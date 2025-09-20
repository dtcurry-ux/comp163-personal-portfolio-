# comp163-personal-portfolio-
# ------------------ Personal Academic & Life Portfolio ------------------

# ------------------ Personal Information (Strings) ------------------
full_name = "Darenell Curry"
student_email = "dtcurry@aggies.ncat.edu"
hometown = "Baltimore, MD"
graduation_semester = "Spring 2029"
major = "Computer Science"

# ------------------ Academic Data (Lists) ------------------
# Lists store ordered collections of related items
current_courses = ["COMP 163", "MATH 131", "ENG 100", "HIS 106", "COMP 121", "GEEN 111"]
completed_courses = ["NA"]
credit_hours = [3, 4, 3, 3, 1, 1]  # Corresponding credit hours for current courses
gpa_history = [3.2]

# ------------------ Contact Information (Tuples) ------------------
# Tuples store fixed collections of related data
emergency_contact = ("Mom", "Shawnelle", "704-555-0199")
home_address = ("456 Oak Street", "Charlotte", "NC", "28202")
instagram_info = ("Instagram", "@nell_capalot", 1032)
twitter_info = ("Twitter", "@nell", 127)
birthday = ("Birthday", 4, 28, 2007)

# ------------------ Interest Tracking (Sets) ------------------
# Sets store unordered collections of unique items
current_skills = {"Python basics", "HTML", "Problem solving", "Time management", "Photography"}
skills_to_learn = {"JavaScript", "C++", "Git", "Web design", "Public speaking"}
career_interests = {"Software development", "CyberSecurity", "Data science", "Game development"}
hobbies = {"Gaming", "Sleeping", "Reading manga", "Gym", "Music"}
entertainment_backlog = {"HellsingUltimate", "Barry", "Life", "Incantation", "Memento"}

# ------------------ Organizational Mapping (Dictionaries) ------------------
# Dictionaries store key-value pairs for fast lookup

# Dictionary mapping course codes to credit values
course_credits = {
    "COMP 163": 3,
    "MATH 131": 4,
    "ENG 100": 3,
    "HIS 106": 3,
    "COMP 121": 1,
    "GEEN 111": 1
}

# Dictionary mapping course codes to professors
course_professors = {
    "COMP 163": "Prof. Rhodes",
    "MATH 131": "Dr. R",
    "ENG 100": "Dr. Joeseph",
    "HIS 106": "Dr. Johneta",
    "COMP 121": "Prof. Rhodes",
    "GEEN 111": "Dr. Parish"
}

# Dictionary mapping course codes to room locations
course_rooms = {
    "COMP 163": "M-Eric 300",
    "MATH 131": "Marteena 201",
    "ENG 100": "Crosby 121",
    "HIS 106": "Crosby 210",
    "COMP 121": "Graham Hall 210",
    "GEEN 111": "McNair 110"
}

# Dictionary mapping budget categories to dollar amounts
monthly_budget = {
    "Food": 200,
    "Entertainment": 150,
    "Books": 0,
    "Transportation": 40
}

# Dictionary mapping subjects to weekly study hours
study_hours_per_subject = {
    "COMP 163": 4,
    "Math": 8,
    "English": 4,
    "History": 3,
    "GEEN": 2,
    "COMP 121": 2

}

# Dictionary mapping contact roles to phone numbers
contact_directory = {
    "Mom": "704-555-0199",
    "Roommate": "336-555-7821",
    "Academic Advisor": "336-334-5000"
}

# ------------------ Required Calculations ------------------

# Total current credits from credit hours list
total_current_credits = sum(credit_hours)

# Cumulative GPA from GPA history list
cumulative_gpa = round(sum(gpa_history) / len(gpa_history), 2)

# Count of completed courses
completed_course_count = len(completed_courses)

# Total weekly study hours from study hours dictionary
total_study_hours = sum(study_hours_per_subject.values())

# Academic load (credits + study hours combined)
academic_load = total_current_credits + total_study_hours

# Monthly budget total from all categories
monthly_budget_total = sum(monthly_budget.values())

# Daily food budget (food amount ÷ 30, rounded to 2 decimals)
daily_food_budget = round(monthly_budget["Food"] / 30, 2)

# Annual budget projection (monthly total × 12)
annual_budget_projection = monthly_budget_total * 12

# Study cost per hour (books budget ÷ total study hours, rounded to 2 decimals)
study_cost_per_hour = round(monthly_budget["Books"] / total_study_hours, 2)

# ------------------ Analytics Calculations ------------------

# Total social media followers from platform tuples
total_followers = instagram_info[2] + twitter_info[2]

# Skills count comparison (current vs. learning goals)
skills_have = len(current_skills)
skills_want = len(skills_to_learn)

# Contact directory size analysis
contact_count = len(contact_directory)

# Entertainment backlog management count
entertainment_backlog_count = len(entertainment_backlog)

# Academic workload assessment
academic_workload = len(current_courses) + total_study_hours

# ------------------ Formatted Output ------------------
print("========== PERSONAL ACADEMIC & LIFE PORTFOLIO ==========")
print(f"Name: {full_name}")
print(f"Email: {student_email}")
print(f"Hometown: {hometown}")
print(f"Graduation: {graduation_semester}")
print(f"Major: {major}")
print("\n--- Academic Summary ---")
print(f"Current Courses: {current_courses}")
print(f"Completed Courses: {completed_courses}")
print(f"Total Current Credits: {total_current_credits}")
print(f"Cumulative GPA: {cumulative_gpa}")
print(f"Completed Course Count: {completed_course_count}")
print("\n--- Study & Budget Overview ---")
print(f"Total Weekly Study Hours: {total_study_hours}")
print(f"Academic Load: {academic_load}")
print(f"Monthly Budget Total: ${monthly_budget_total}")
print(f"Daily Food Budget: ${daily_food_budget}")
print(f"Annual Budget Projection: ${annual_budget_projection}")
print(f"Study Cost per Hour: ${study_cost_per_hour}")
print("\n--- Analytics ---")
print(f"Total Social Media Followers: {total_followers}")
print(f"Skills Have vs Want: {skills_have} vs {skills_want}")
print(f"Contact Directory Size: {contact_count}")
print(f"Entertainment Backlog Count: {entertainment_backlog_count}")
print(f"Academic Workload Assessment: {academic_workload}")
print("========================================================")
