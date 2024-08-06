# Face-Recognition-Attendance-System-Using-Opencv
Download Visual studio
Download mysql Workbench
Download Python 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
libraries to install
pip install opencv-python
pip install mysql-connector-python
pip install pillow
pip install numpy
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
keep the source code in C:\
"conn = mysql.connector.connect(username='root', password='root',host='localhost',database='face_recognition',port=3306)
                mycursor = conn.cursor()"   
find this code and change the password and port number as per your system
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
create schema "face_recognition"
create tables ->"regteach" , "stdattendance", "student"

CREATE TABLE regteach (
    fname VARCHAR(45) NOT NULL,
    lname VARCHAR(45) NOT NULL,
    cnum VARCHAR(45),
    email VARCHAR(45) NOT NULL,
    ssq VARCHAR(45),
    sa VARCHAR(45),
    pwd VARCHAR(45),
    PRIMARY KEY (email)
);

CREATE TABLE stdattendance (
    std_id VARCHAR(45) NOT NULL,
    std_roll_no VARCHAR(45) PRIMARY KEY NOT NULL,
    std_name VARCHAR(45),
    std_time TIME,
    std_date VARCHAR(45),
    std_attendance VARCHAR(45)
);


CREATE TABLE student (
    Student_ID VARCHAR(45) PRIMARY KEY NOT NULL,
    Name VARCHAR(45) NOT NULL,
    Department VARCHAR(45),
    Course VARCHAR(45),
    Year VARCHAR(45),
    Semester VARCHAR(45),
    Division VARCHAR(45),
    Gender VARCHAR(45),
    DOB VARCHAR(45),
    Mobile_No VARCHAR(45),
    Address VARCHAR(45),
    Roll_No VARCHAR(45),
    Email VARCHAR(45),
    Teacher_Name VARCHAR(45),
    PhotoSample VARCHAR(45)
);

