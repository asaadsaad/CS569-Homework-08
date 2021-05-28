# CS569 Homework 08
## Coding Exercise
* Use Express/MongoDB to create a web-server that implements `GET`, `POST`, `PUT`, `DELETE` HTTP verbs for an entity called `courses`. A course object has the following structure:
```javascript
{_id: 1, name:'Web Application Development', code:'CS569', topics: ['Angular', 'API design'] }
```  
* Use Angular to build a client app that has a lazy-loaded module `CourseModule` that offers: 
  * Showing list of courses
  * Add a new course (Reactive Form)
  * Update a course by ID (Reactive Form)
  * Delete a course by ID
