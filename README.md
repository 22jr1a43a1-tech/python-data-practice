# python-data-practice
employees = [
    {"name": "Ashok", "department": "IT", "salary": 45000},
    {"name": "Ravi", "department": "HR", "salary": 35000},
    {"name": "Kiran", "department": "IT", "salary": 60000},
    {"name": "Suresh", "department": "Sales", "salary": 40000},
]

# Filter employees with salary above 40000
def filter_high_salary(employees):
    for emp in employees:
        if emp["salary"] > 40000:
            print(emp["name"], emp["salary"])

# Find the highest-paid employee
def highest_salary_employee(employees):
    highest = max(employees, key=lambda emp: emp["salary"])
    print("Highest paid:", highest["name"], highest["salary"])

filter_high_salary(employees)
highest_salary_employee(employees)
