---
layout: project
type: project
image: img/studybuddy.png
title: "Study Buddy"
date: 2019
published: true
labels:
  - Python
  - MongoDB
  - Flask
summary: "A web app that my team built to aid college students find study groups in their campus for specific courses."
---

<div class="text-center p-4">
  <img width="200px" src="../img/studdybuddy-1.png" class="img-thumbnail" >
</div>

Study Buddy is a web application I created with my team to help college students find study groups based on their major or class. It will prompt the user to enter their information, like their college and class, and connect them to study groups. In order to develop the web app, we used Flask to provide us with the tools and libraries we needed. I was in charge of creating the function to get user data, store it in a database, and post it once the user is matched with a group. I linked it to MongoDB, where the info can be stored so that it can print out a confirmation in the next page.

Here is some code that illustrates how we show study group times:

```cpp
@app.route('/results', methods = ['GET', 'POST'])
def results():
    if request.method == "GET":
        return render_template('index.html')
    else:
        name_name = request.form['name'] 
        college_name = request.form['college']
        email_name = request.form['email']
        major_name = request.form['major']
        course_name = request.form['course']
        classes_name = request.form['classes']
        print('name')

        callcourse = model.search(college_name,course_name)
        date = callcourse['date']
        time = callcourse['time'] 
        time2 = callcourse['time2']
        time3 = callcourse['time3']
        time4 = callcourse['time4']
        time5 = callcourse['time5']
        location = callcourse ['location']
        print(callcourse)
        collection = mongo.db.Form
        collection.insert({'name': name_name, 'college': college_name, 'email':email_name, 'major': major_name, 'course': course_name, 'classes': classes_name})
        userInfo = collection.find_one({"name" : name_name})
        return render_template("results.html", userInfo = userInfo, date= date, time = time, time2 = time2, time3 = time3, time4 = time4, time5 = time5, location = location)
  
```


