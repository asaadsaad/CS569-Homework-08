# CS569 Homework 09
## Coding Exercise
* Your main `AppModule` supports Angular Router and has only one service: create a service that returns an array of JSON objects. 
```json
[{"id":1, "name": "Asaad Saad", "hobbies":["violin", "cooking", "hiking"]}, ...]
```
* Create a featured module called `Users` that is responsible for showing a list of users, your application should only load this module when navigating to `users` route. 
* Within `Users` module we have two components, both components will retrieve data using the service you created earlier in `AppModule`
  * `users` component 
  * `userdetails` component 
* When users click on `users/:id` you should display `userdetails` child component with full details about the user.
* If a user tried to visit `users/:id` page without passing an existing `id` param, then your app must redirect them to a friendly error page. (use Guards).  
**Note: Write this exercise with Lazy Loading in mind.**
