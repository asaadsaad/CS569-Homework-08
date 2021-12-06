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
