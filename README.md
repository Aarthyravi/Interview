# Interview Practice (Full Stack)

  * What is the most influential book or blog post you’ve read regarding web development?
    - I haven't read a book or blog about the Web Development. I have read only Udacity Documentation. Before I have started this udacity course, I have done some projects using HTML,PHP with MYSQL. While working on that project I got struggle to design the frond end and to store the data on the back end. Hopefully Now I am familiar with HTML, CSS, js and database.
    - Now I can able to design a web application using python/front-end frameworks like webapp2, flask/Bootstrap and jinja is one of the most used templates for python.
 
 * Tell me about a web application you have built. Why did you choose to build it? What did you learn? What challenges did you face and how did you overcome them? 
   - I have built a web blog application using Google App Engine. In this project, First Signup the new user. After a successful signup,a user can be able to create, edit and delete their own post on blog and user can comment on others post and they can be able to edit/delete thier own comment on blog. Multi User Blog web application is one of the project in Udacity full stack Nanodegree Course. 
   - As well as I have learnt how to handle the input from the user, how to use the jinja template engine for python and how to use SQL databases in python. Finally, how to build a complete login system to authenticate the users. 
   - The challenges that I have faced how to use the cookies for authentication and how to use jinja2 template and webapp2 framwwork. All concepts in this project are very new. One more thing is how to deploy my web app in gcloud. Read the Google App engine Documentation and I have solved the problems in my code using google search engine and have seen many solutions in other discussion sites like Stack Overflow, Quora. 
   
* Write a function in Python that takes a list of strings and returns a single string that is an HTML unordered list\(\<ul\>..\<\/ul\>\) of those strings. You should include a brief explanation of your code. Then, what would you have to consider if the original list was provided by user input?
   
      # HTML unordered list in python
      def list(strlst):
          output = ""
          output += "List of Food\n"
          output += "\n<ul>"
          for i in strlst:
              output += "\n <li>" + i + "</li>"
        
          output += "\n</ul>"
    
          return output

      foodlist = ["Pizza", "Burger", "Noodles", "Soup"]
      print list(foodlist)
       
  
         
