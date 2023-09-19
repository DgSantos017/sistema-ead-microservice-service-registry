# System EAD Microservice Service Registry

## baseUrl
http://localhost:8761/

![image](https://github.com/DgSantos017/sistema-ead-microservice-service-registry/assets/62971277/c3dd5d9b-e75b-440d-8c52-42cf243f5d6a)

# API Rest Features 
## baseUrl Api Gateway
http://localhost:8080/

# AUTHUSER
## baseUrl
http://localhost:8080/ead-authuser/

### registerUser -> auth/signup

#### getAllUsers -> users
getOneUser -> users/userId
updateUser -> users/userId
deleteUser -> users/userId
updateImage -> users/userId/image
updatePassword -> users/userId/password
turnUserIntoInstructor-> users/turn-user-into-instructor
getAllCoursesByUser -> user/userId/courses

### COURSE
#### baseUrl
http://localhost:8080/ead-course/
  
saveCourse -> courses
getAllCourses -> courses
getOneCourse -> courses/courseId
updateCourse -> courses/courseId
deleteCourse -> courses/courseId

saveModule-> modules/course/courseId
getAllModules -> modules/course/courseId
getOneModule -> modules/course/courseId/module/moduleId
updateModule -> modules/course/courseId/module/moduleId
deleteModule -> modules/course/courseId/module/moduleId

saveLesson-> lessons/module/moduleId
getAllLessons -> lessons/module/moduleId
getOneLesson -> lessons/module/moduleId/lesson/lessonId
updateLesson -> lessons/module/moduleId/lesson/lessonId
deleteLesson -> lessons/module/moduleId/lesson/lessonId

getAllUsersByCourse -> course/courseId/users
subscribeUserToCourse -> course/courseId/subscribe-user

## Requirements to Run Locally
- Java: Version 11 or higher

## Stacks
- Java 11
- Spring Boot 2.5.4
- spring cloud netflix eureka

# Tools
- Linux
- IntelliJ IDE

# How to Run?
- Fork and clone this repository
- Download dependencies; if using IntelliJ, you can trigger Maven to handle this process automatically
- From the ``ServiceregistryApplication`` file, execute the project; if everything is correct, the API will run on port 8761

Developed by [Diogo Ferreira](https://www.linkedin.com/in/diogo-santos01/)
