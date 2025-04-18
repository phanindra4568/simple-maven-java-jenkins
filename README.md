A simple Java Hello World project built with Maven and integrated with Jenkins.

## 📁 Project Structure

hello-java-maven/ ├── pom.xml └── src/ └── main/ └── java/ └── HelloWorld.java

---

## 🧑‍💻 Prerequisites

- Java JDK 8 or 11
- Maven
- Jenkins
- Git 

---

## 🚀 Steps to Run Maven Build Job in Jenkins

### 1. Clone or Create the Project

Create the folder structure as shown above, and add the following files:

*HelloWorld.java*

**pom.xml**

### 2. Configure Maven in Jenkins
Go to Manage Jenkins → Global Tool Configuration

Under Maven, click Add Maven

Name: Maven 3.8.6

Check Install automatically

Save

### 3. Create Jenkins Freestyle Job
Go to Dashboard → New Item

Name: HelloJava

Select Freestyle project

Click OK

### 4. Configure the Job
Under Build → click Add build step

Choose: Invoke top-level Maven targets

Goals: clean package

### 5. Build the Project
Click Build Now

Open Console Output

Look for: ✅ BUILD SUCCESS
