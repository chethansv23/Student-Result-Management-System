# Student-Result-Management-System  

An individual Student result is displayed. An important aid for students to judge their performance. Student performance in all the Subjects will be displayed.  

Language used: **SQL**,**Java**.  
Software used: **Apache Netbeans**, **MySQL**.  

In this project I have created totally eight JFrames.

### 1) HomePage

In this jframe there is two botton   
  * Staff  - redirect to staff login page(frame).  
  * Student - redirect to student portal(frame).  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/homepage.png)
  
### 2)StaffLoginPage  

  * In this jframe staff need to provide UserID and Password inorder to login into staff Home Page.  
  * As per this project I have kept the userID "admin" and password "admin" to login.  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/stafflogin1.png)  

### 3)Staff Home Page  
  As soon as the staff click on login it redirect to Staff Home Page where staff can perform following operation.  
  a) Add New Student     
  b) Insert New Result  
  c) Registered Student  
  d) All Student Result  
  
  The above all bottons will be present in StaffHomepage, InsertNewResult, RegisteredStudent and AllStudentResult jFrames.  
  
  Add New Student:  
  * By default the staff home page has this frame where staff can enter student basic detail like roll number(this should be unique), name, class, date of birth, gender,father name.  
  * As soon as we click on add all the details will be stored in mysql database of table name "student" inside school databaser with respect to "rollnumber" as a primary key.  
  * Before adding the data in student table please create a table "student" inside "school" database.  
   **create table student(rollnumber varchar(255) primary key, name varchar(255), studentclass int, dob varchar(255), gender char(4), fathername varchar(255));**
    ![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/student1.png)
  * Note: In these project I have used user name as "root" and password as "root". Please enter your MySQL password inside all the jframe where ever database is used.                         
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/staffhomepage.png)
  
### 4) Insert New Result  
   * Inorder to add the marks of student. Staff need to click on "Insert New Result" botton.  
   * First need to enter the student roll number and click on search button so that student name will be displayed to verify.  
   * Now Staff can enter the student marks 
   * Before adding the data in student table please create a table "result" inside "school" database.  
     **create table result(rollnumber varchar(255) primary key, kannada int, english int, hindi int, mathematics int,science int, social int);**
     ![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/result.png)
   * Once the staff click on add. The marks of the students in all the subject will be saved in school database in table name "result" with respect to "rollnumber" as a primary key.  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/insertmarks.png)
   * When the invalid roll number is entered "Invalid Roll Number" message will popup as shown in below image.  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/insertmakserror.png)
* When valid roll number is entered student name will be displayed and can verify the name to whom marks has to be entered.
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/insertMarksStudentName.png)

  
### 5) Registered Student  
  * As the staff click on Registered Student. All the details of Students will be fetched from database and displayed. As shown below.  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/studentdetails.png)
  
### 6) All Student Result  
  * Similarly as the staff click on All Student Result. All the subject marks of Students will be fetched from database and displayed. As shown below.  
   ![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/studentmarks.png)

### 7) Student Portal
   * Student will be redirected to Student portal when clicked on Student botton in Home page.  
   * Student need to enter the valid rollnumber to fetch the result else "Invalid Roll Number" message will popup.  
   * If Students enters the valid roll number then it will be redirected to StudentResult page.  
   ![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/studentportal.png)  

### 8) Student Result
  * This is the frame where the result of student will be displayed.  
  * Below is the two example where one student is passed and other student is failed.  
  ![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/pass.png)  
![This is an image](https://github.com/chethansv23/Student-Result-Management-System/blob/main/fail.png)


Thank You 
