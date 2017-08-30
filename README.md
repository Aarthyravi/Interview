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
      
  - The python function 'list(foodlist)' that takes a list of strings and for loop iteration is used to returns the ordered list what I have given in the List array. Finally returns a single string that is an HTML unordered list. My output is :
        
        >>> 
        List of Food

        <ul>
         <li>Pizza</li>
         <li>Burger</li>
         <li>Noodles</li>
         <li>Soup</li>
        </ul>
        >>>    
  Have to consider if the original list was provided by user input? 
   - If we check whether the user input is string or not. And we would need to check the input is blank or not. 
     So we have to use If...else conditional statement for check and to display the proper error message.       
     
 * List 2-3 attacks that web applications are vulnerable to. How do these attacks work? How can we prevent those attacks?  
   
    1. SQL injection 
         - It is a code injection technique that might destroy our database.It is one of the most common web hacking techniques.
           SQL Injection Based on 1=1 is Always True
           For ex. Roll No. 12 OR 1 = 1 - This is the Hacker input.
           
         - SELECT * FROM Students WHERE rollno = 12 OR 1=1;
            * The SQL above is valid and will return ALL rows from the "Students" table, since OR 1=1 is always TRUE.
            A hacker might get access to all the student names and passwords in a database, by simply inserting 12 OR 1=1 into the input               field. 
       * how to prevent this SQL injection?
         - To protect a web site from SQL injection, we can use SQL parameters.
         - txtrollno = request.get("RollNo");
           txtSQL = "SELECT * FROM Students WHERE rno = @0";
           db.Execute(txtSQL,txtrollno);
