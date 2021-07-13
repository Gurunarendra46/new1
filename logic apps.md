#Use Case
<h3>Scenario</h3>
<p> Customer has Newly Created a Website which is having Paid Courses for microsoft azure conducted exams and some certified Exams conducted by reputated organizations.
  Indeed Customer want to get more users to buy the courses. so whenever user sign up to the website ,customer want to contact the user through e mail for the reason if 
  the user left the website without buying any course. if user does,store the course name and user detail in storage and send a mail for thanking the user.  <p>
    
<h3>Solution</h3>
<p> By Using <b> Logic Apps </b>with No/Less code ,we can implement the UseCase ,we will try to use pre-built Connector to implement it. </p>

<h5>Steps to implement Logic App</h5>
<ol>
<li>Create a logic app resource that runs in the multi-tenant Logic Apps service environment.</li>
<li>Select the blank logic app template.</li>
<li>Add a trigger that specifies when to run the workflow.</li>
<li>Add an action that performs a task after the trigger fires.</li>
<li>Run your workflow.</li>
</ol>

<b>step1</b><br><h4>Create a logic app resource that runs in the multi-tenant Logic Apps service environment.</h4>
<ol>
<li>Sign in to the Azure portal with  Azure account.</li>
<li>In the Azure search box, enter logic apps, and select Logic Apps.</li>
<li>On the Logic Apps page, select Add > Consumption.
<br>
This step creates a logic app resource that runs in the multi-tenant Logic Apps service environment</li>
<li>On the Logic App pane, provide basic details and settings for your logic app. Create a new resource group for this example logic app.</li>
  <img src="">
<li>When you're ready, select Review + Create. On the validation page, confirm the details that you provided, and select Create.</li>
</ol>
<b>step2</b><br><h4>Select the blank template</h4>
<ol>
  <li>After  deploying logic app, select Go to resource. Or, find and select your logic app by typing the name in the Azure search box.</li>
  <li>The Logic Apps Designer opens and shows a page with an introduction video and commonly used triggers.</li>
  <li>Under Templates, select Blank Logic App</li>
  </ol>
  
  <b>step3</b><br><h4>Add the Trigger</h4>
  <ol>
  <li><b>In the Logic Apps Designer, under the search box, select Select HTTP request<b></li>
    </ol>
  <b>step4</b><br><h4>Add the Action</h4>
  <ol>
  <li><b>We need to implement the Signup/SignIn Connector ,This comes Under<b> <b>Action<b></li>
</ol>
    
<b>step5</b><br><h4>Add the Control</h4>
    
<ol>
    <li>add  the if Connector ,and in if we need to mention <b>User Enrolled the Course or Not</b> This comes Under <b>Control<b></li>
</ol>
      
 <b>step6</b><br><h4>Add the Actions</h4>
      
<ol>
    <li>If Yes :add an Blob Storage to save the user Details and course that the user enrolled.<br>take the user's e-Mail and send the Thanking Mail. </li><br>
    <li>If No :Send the e-mail to the User and in mail add the Feedback template that the reason to not interested to enrolled the Course. </li>
    
</ol>    
  
  
  
  
 









