# DoraBhai.com 
## Placement APIs

 - ####  Users Table
    |sl no|***Path***|***Request Type***| ***Req***|***Res***|***Desc***|
    |---|---|---|---|---|---|
    |1|*/user/add*|**POST**|name,email_id,mobile,security_question,security_answer,student_id|test_id|Generate unique 8 digit alphanumeric test ID and send it as a response also set all the other parameters to 0|
    |2|*/user/marks*|**POST**|test_id,response|english_comprehension,logical_ability,quantitative_ability,essay_writing,automata,|Calculate the marks according to the response|
    |3|*/admin/user/show/:id*|**GET**|---|data|Uses data limited by id Parameter. Where id is breadcrumb number |
    |4|*/admin/user/alter/:id*|**POST**|name,email_id,mobile,security_question,security_answer,student_id|data|Update the user data with given student id generate new test ID and respond with entire data set|
    |5|*/admin/user/delete/:id*|**GET**|---|***status:true***|Delete with given test ID|
    |6|*/admin/user/delete*|**GET**|---|***Status:true***|Delete the data of entire table|
---

 - #### Company 
   - ##### Admin
    |sl no|***Path***|***Request Type***| ***Req***|***Res***|***Desc***|
    |---|---|---|---|---|---|
    |1|*/admin/company*|**POST**|qtype,into,question,options,answer,company,link|qid|At the given question and return the question ID as a response|
