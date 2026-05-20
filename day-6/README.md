Day 6

-> 1. What is SOQL?
SOQL (Salesforce Object Query Language) is used to retrieve data from Salesforce objects and database tables. It helps developers search, filter, and fetch records from Salesforce.
Example:
- Find all students in Course A
- Find students with attendance below 75%

## 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that runs automatically when records are inserted, updated, deleted, or undeleted in Salesforce.

Triggers help automate business processes based on events.

Example:
- Send notification after student registration
- Update seat count after course enrollment

---

# 3. Difference Between Flow and Trigger

| Flow | Apex Trigger |
|------|---------------|
| No-code automation | Coding-based automation |
| Easy to build | More powerful |
| Best for simple logic | Best for complex logic |
| Faster development | Better flexibility |
| Limited for advanced cases | Handles advanced business rules |

---

# 4. Difference Between Before and After Trigger

| Before Trigger | After Trigger |
|----------------|----------------|
| Runs before saving record | Runs after saving record |
| Used for validation | Used for notifications |
| Can modify values before save | Used for related actions |

---

# 5. Trigger Use Cases

## Case 1
After student registration → Send welcome email

Event:
After Insert on Student object

## Case 2
After course becomes full → Notify faculty

Event:
After Update on Course object

## Case 3
After attendance drops below 75% → Send warning notification

Event:
After Update on Attendance object

## Case 4
After fee payment → Generate receipt automatically

Event:
After Update on Payment object

## Case 5
After exam results published → Notify students

Event:
After Insert on Result object


# 6. Query Examples

- Find all students in Course A
- Find all courses handled by Faculty X
- Find students with attendance below 75%
- Find students who did not pay fees
- Find courses with no available seats


# 7. Reflection

Enterprise systems need event-driven behavior because actions must happen automatically when data changes.

Triggers help systems react instantly to important business events such as registrations, payments, attendance updates, and notifications.

This improves automation, accuracy, and efficiency in large systems.
