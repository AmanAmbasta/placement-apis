# DoraBhai.com 
## Placement APIs

 - ####  Users Table
    |sl no|***Path***|***Request Type***| ***Req***|***Res***|***Desc***|
    |---|---|---|---|---|---|
    |1|*/user/add*|**POST**|name,email_id,mobile,security_question,security_answer,student_id|test_id|Generate unique 8 digit alphanumeric test ID and send it as a response also set all the other parameters to 0|
    |2|*/user/marks*|**PUT**|test_id,response|english_comprehension,logical_ability,quantitative_ability,essay_writing,automata,|Calculate the marks according to the response|
    |3|*/user/show/:id*|**GET**|---|data|Uses data limited by id Parameter |

 - #### 