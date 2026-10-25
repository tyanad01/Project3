# Project 3: Features, Personas, Scenarios, and User Stories

**Student:** Tyana Davis  
**Professor:** Wanjun Hu  
**Product:** School System Website  
**Sprint:** CSprint 3


## Section 1: Features

### Feature 1: Login Screen and User Entry
**Description:** Provide a login page with username or email and password fields and a Login button. The login screen is the entry point to the website.

**Purpose:** Give students, faculty members, and administrators a clear starting point and help keep school information intended for authorized users.

**Expected behavior / acceptance criteria:**
- The page displays labeled username/email and password fields.
- The Login button is easy to find and use.
- Empty required fields should be identified before a login attempt is submitted.
- Authentication must be connected and tested before the page is described as providing working account security.

### Feature 2: School Records Dashboard and Navigation
**Description:** Provide a dashboard with navigation to the website's main areas: Students, Courses, Faculty, Student-Course, Faculty-Course, and Buildings.

**Purpose:** Let users find the correct school-record section without having to search through separate pages.

**Expected behavior / acceptance criteria:**
- Each main section has a clear, consistent label.
- Navigation links lead to the corresponding section or prototype screen.
- The navigation style remains consistent across the pages.
- The dashboard uses the planned soft-pink and white visual design.

### Feature 3: Student Record Management
**Description:** Display student records with fields for student ID, first name, last name, address, email, phone number, and major.

**Purpose:** Help authorized staff review and maintain student information in one organized location.

**Expected behavior / acceptance criteria:**
- The student page identifies the fields shown for each record.
- Information is presented in a readable, consistent layout.
- Any create, edit, delete, or save action should only be described as working after it has been implemented and tested.
- Student personal information should be accessible only to authorized users in a production system.

### Feature 4: Course and Faculty Records
**Description:** Provide separate sections for course information and faculty information.

**Purpose:** Organize academic course details and faculty records so users can find the information relevant to their role.

**Expected behavior / acceptance criteria:**
- Courses and faculty have separate, clearly labeled sections.
- Each page uses the same general navigation and visual layout.
- Displayed fields are labeled and easy to read.
- Record changes should be validated and tested before being treated as complete functionality.

### Feature 5: Student-Course and Faculty-Course Relationships
**Description:** Provide sections that represent which students are associated with which courses and which faculty members are assigned to courses.

**Purpose:** Make relationships between school records easier to understand and review.

**Expected behavior / acceptance criteria:**
- The student-course page communicates the relationship between students and courses.
- The faculty-course page communicates faculty course assignments.
- Related records are presented in a consistent format.
- Any enrollment or assignment changes should be confirmed by the underlying system before being shown as saved.

### Feature 6: Building Records
**Description:** Provide a dedicated Buildings section for school-building information.

**Purpose:** Keep building records separate from student, course, and faculty records while making them accessible through the same navigation.

**Expected behavior / acceptance criteria:**
- The Buildings section is easy to locate.
- Building information is displayed in a clearly labeled layout.
- The page follows the site's shared colors, typography, and navigation pattern.

### Shared Visual Design and Usability
The proposed interface uses a soft-pink and white color scheme. The navigation bar uses pink (`#ff99cc`), the page background uses light pink (`#fef6fb`), and the Poppins font is planned for consistent typography. Forms should group related fields together, buttons should use understandable labels, and all database sections should have a consistent layout.

## Section 2: Personas

### Persona 1: School Administrator
- **Name:** Danielle Brooks (fictional)
- **Role:** School administrator
- **Primary goals:** Keep school records organized, review student and faculty information, and locate building and course records quickly.
- **Needs:** Clear navigation, consistent record layouts, accurate information, and appropriate access controls.
- **Frustrations:** Information scattered across different pages, confusing field names, and uncertainty about whether a record was saved.
- **How the website helps:** The dashboard links to the main record sections, while the separate management pages keep information organized.
- **Accessibility and security considerations:** The administrator should have only the permissions needed for assigned duties, and important changes should be confirmed.

### Persona 2: Faculty Member
- **Name:** Marcus Reed (fictional)
- **Role:** Faculty member
- **Primary goals:** Find course information and understand which courses are assigned to faculty.
- **Needs:** Readable course and faculty pages, simple navigation, and current assignment information.
- **Frustrations:** Having to browse unrelated school records to find course details.
- **How the website helps:** The Courses and Faculty-Course sections make academic information easier to locate.
- **Accessibility and security considerations:** Faculty members should see information appropriate to their role and should not automatically receive administrator-level permissions.

### Persona 3: Student
- **Name:** Aaliyah Carter (fictional)
- **Role:** Student
- **Primary goals:** Find relevant course information and understand which courses are associated with a student record.
- **Needs:** A clear login screen, understandable labels, and easy-to-use navigation.
- **Frustrations:** Unclear page names, difficult navigation, and not knowing where to find course information.
- **How the website helps:** The login page and dashboard provide a clear entry point, and the student-course section represents the connection between students and courses.
- **Accessibility and security considerations:** A student should only be able to access records and personal information permitted for student accounts.

## Section 3: Scenarios

### Scenario 1: An Administrator Reviews a Student Record
**Situation:** Danielle Brooks, a school administrator, needs to check a student's contact details and major.

**Action:**
1. Danielle opens the School System Website.
2. She enters her login details if authentication is available in the current build.
3. She selects Students from the dashboard navigation.
4. She locates the relevant student record and reviews the displayed fields.

**Expected outcome:** Danielle can find the student record and identify the contact and major information. If editing is supported, any change should be validated and confirmed as saved. This scenario describes the intended workflow; it does not assert that all record operations are implemented.

### Scenario 2: A Faculty Member Looks Up Course Information
**Situation:** Marcus Reed wants to review course information and understand faculty-course assignments.

**Action:**
1. Marcus opens the website.
2. He uses the dashboard navigation to open Courses.
3. He reviews the available course information.
4. He opens Faculty-Course to review the displayed relationship between faculty and courses.

**Expected outcome:** Marcus can navigate between the relevant sections and understand where course and assignment information is organized.

### Scenario 3: A Student Finds Their Course Relationship
**Situation:** Aaliyah Carter wants to understand which courses are associated with a student record.

**Action:**
1. Aaliyah opens the website's login screen.
2. She enters her credentials if working authentication is available.
3. She opens the Students or Student-Course section, depending on the access provided by the system.
4. She reviews the relevant information that her role is permitted to see.

**Expected outcome:** Aaliyah can identify the appropriate section for student-course information. In a production version, the system must restrict access to other students' private records.

## Section 4: User Stories

### User Story 1: Sign In
**As a** school website user, **I want** a login page with username/email and password fields, **so that** I have a clear entry point to the system.

**Acceptance criteria:**
- Username/email and password fields are labeled.
- The Login button is visible.
- Empty required fields are identified.
- Successful and unsuccessful authentication behavior is only considered complete after it has been implemented and tested.

### User Story 2: Navigate to School Records
**As a** school administrator, **I want** a dashboard with links to Students, Courses, Faculty, Student-Course, Faculty-Course, and Buildings, **so that** I can find the correct school-record section efficiently.

**Acceptance criteria:**
- All planned sections are clearly labeled in the navigation.
- Each link opens its corresponding page or prototype screen.
- Navigation remains consistent across pages.

### User Story 3: Review Student Information
**As a** school administrator, **I want** to view student ID, name, address, email, phone number, and major in an organized student page, **so that** I can review student information in one place.

**Acceptance criteria:**
- The student page presents the planned fields clearly.
- Field labels are understandable.
- Any record-editing capability is verified before being described as functional.
- Private student data is protected by role-based access in a production system.

### User Story 4: Review Course and Faculty Information
**As a** faculty member, **I want** separate Courses and Faculty-Course sections, **so that** I can locate course details and understand faculty-course assignments.

**Acceptance criteria:**
- Courses and Faculty-Course are separate, labeled sections.
- The layout is consistent and readable.
- The relationship between faculty and courses is clear.

### User Story 5: Review Building Information
**As a** school administrator, **I want** a dedicated Buildings section, **so that** I can find building records without searching through unrelated school information.

**Acceptance criteria:**
- Buildings is accessible from the dashboard navigation.
- Building information has clear labels.
- The page follows the shared visual design.

## Scope and Limitations
The supplied prototype screens include Login, Dashboard, Students, Courses, Faculty, Student-Course, Faculty-Course, and Buildings. These screens communicate the intended layout and navigation. The prototype should not be assumed to have a connected database, working authentication, fully implemented record editing, or production-grade security unless those capabilities have been separately built and tested.

## Conclusion
The School System Website prototype is intended to organize core school information in a single, consistent interface. The planned features focus on login, dashboard navigation, and school record sections. The personas, scenarios, and user stories describe how administrators, faculty members, and students could use the system and provide a basis for future design and testing.
