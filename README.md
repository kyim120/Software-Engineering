# Software Engineering
## Assigment 1.
# **Task 1: Software Understanding (4 Marks)**

### **a. Four Characteristics of Software in SCMS**

| Software Characteristic                    | Explanation in Context of SCMS                                                                                                                                                                                      |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Software is intangible (non-physical)**  | SCMS cannot be physically touched like hardware. This makes testing and visualizing its functionality more complex. Stakeholders may misunderstand progress because they cannot “see” the system until late stages. |
| **Software is continually evolving**       | As faculty and students change their needs, SCMS must be updated frequently. New academic policies or semester structures may require feature modifications.                                                        |
| **Software is complex**                    | SCMS integrates multiple modules (attendance, grades, fees, announcements). Managing interactions between these modules increases development complexity.                                                           |
| **Software is subject to frequent change** | Requirements will keep changing based on feedback from faculty, students, and administration. The system must be flexible to support updates without breaking existing features.                                    |

---

### **b. Two Software Myths and Their Impact**

| Myth                                                                          | Category            | Real-World Impact if Not Corrected                                                                                                          |
| ----------------------------------------------------------------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **“General objectives are enough; detailed requirements are not necessary.”** | **Customer Myth**   | Leads to misunderstood expectations, missing features, and rework. SCMS may fail to meet actual campus needs.                               |
| **“Adding more developers will help meet tight deadlines.”**                  | **Management Myth** | In reality, adding developers increases communication overhead and delays. New members need training, which may further slow SCMS delivery. |

---

# **Task 2: Requirement Engineering Process (4 Marks)**

| RE Task              | How It Applies to SCMS                                                                                                                               |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Inception**     | Identify stakeholders: administration, faculty, students, and IT staff. Define the main goals like attendance automation and communication platform. |
| **2. Elicitation**   | Conduct interviews, surveys, and observation sessions to gather requirements about attendance, fee records, and result uploads.                      |
| **3. Elaboration**   | Create detailed use cases and workflow diagrams for processes like “Mark Attendance” and “View Grades.”                                              |
| **4. Negotiation**   | Resolve conflicting requirements between faculty and administration (e.g., level of detail in attendance reports). Prioritize core features.         |
| **5. Specification** | Document functional and non-functional requirements clearly in SRS (Software Requirement Specification).                                             |
| **6. Validation**    | Review SRS with stakeholders, conduct demos & prototypes to confirm requirements meet needs.                                                         |
| **7. Management**    | Track changes in requirements as policies change (e.g., new grading system). Maintain version control.                                               |

---

# **Task 3: Requirement Identification (8 Marks)**

### **1. Functional Requirements (What system should do)**

1. Students can **view attendance records**.
2. Students can **check fee status and dues**.
3. Faculty can **mark attendance** for their assigned classes.
4. Faculty can **upload grades/results**.
5. Administrators can **generate reports and send notifications**.

### **2. Non-Functional Requirements**

| Type                | Requirement                                                                             |
| ------------------- | --------------------------------------------------------------------------------------- |
| **Performance**     | The system should respond to user actions within **3 seconds**.                         |
| **Security**        | Only authenticated users should access personal data (role-based access control).       |
| **Maintainability** | The system should be modular so updates can be made without affecting the whole system. |

---

# **Task 4: Use Case Diagram (4 Marks)**

### **Actors**

* **Student**
* **Faculty**
* **Administrator**

### **Use Case Diagram (Text Form)**

```
                +--------------------+
                | Smart Campus (SCMS)|
                +--------------------+
            /             |               \
           /              |                \
   (Student)        (Faculty)           (Administrator)
       |                 |                   |
       |                 |                   |
   [View Attendance]  [Mark Attendance]   [Generate Reports]
   [View Grades]      [Upload Grades]     [Send Notifications]
   [View Fee Status]  [Share Announcements] [Manage System]
```

Or, if you want a UML-style representation:

```
Student --------> (View Attendance)
Student --------> (View Grades)
Student --------> (View Fee Status)

Faculty --------> (Mark Attendance)
Faculty --------> (Upload Grades)
Faculty --------> (Post Announcements)

Administrator --> (Generate Reports)
Administrator --> (Send Notifications)
Administrator --> (Manage Users)
```

---
