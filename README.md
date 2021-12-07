# CS569 Homework 08
## Coding Exercise
* Use Express/MongoDB to create a web-server that implements `GET`, `POST`, `PUT`, `DELETE` HTTP verbs for an entity called `courses`. A course object has the following structure:
```javascript
{
  _id: ObjectId(), 
  name:'Web Application Development', 
  code:'CS569', 
  students: [
    {student_id: 123456, fullname: 'Asaad Saad'}
   ]
}
```  
**Implement 10 routes for a complete CRUD operations to control courses and students. (add/update/delete/get one/get all with pagination).**
* Use Angular to build a client app that has a lazy-loaded module `CourseModule` that offers: 
  * Showing list of courses
  * Showing list of students who are enrolled in the course


`GET /courses` => returns all courses (everything except students) - HERE easy skip-limit (Read or set default value)  
`POST /courses` => adds a new course `{name, code}`  
`GET /courses/:course_id` => returns info about a single course  
`PUT /courses/:course_id` => update the course name, code based on the _id  
`DELETE /courses/:course_id` => deletes a single course  
  
`GET /courses/:course_id/students` => returns all students belong to specific course - HERE hard array-projection (Advanced)  
`POST /courses/:course_id/students` => adds a new students to a course `{student_id, fullname}`  
`GET /courses/:course_id/students/:student_id` => returns info about a single student  
`PUT /courses/:course_id/students/:student_id` => update the student, code based on the student_id and course_id  
`DELETE /courses/:course_id/students/:student_id` => deletes a single student  

`GET /find/courses/:code` => finds if course code exists or not  
`GET /find/courses/:course_id/students/:student_id` => finds if a students already added to the course or not  
  
 - <course code, course name>(edit)(x) (add)  
 - <course code, course name>(edit)(x)  
 - <course code, course name>(edit)(x)   
  
  
- Course name and code  
 - <student ID, fullname> (edit)(x) (add)  
 - <student ID, fullname> (edit)(x)   
