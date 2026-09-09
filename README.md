index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EduNexa AI</title>

<link rel="stylesheet" href="css/style.css">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

</head>

<body>

<div class="container">

    <!-- Sidebar -->
    <div class="sidebar">

        <div class="logo">
            <h2>🎓 EduNexa AI</h2>
            <p>Student Assistant</p>
        </div>

        <button class="new-chat" onclick="newChat()">
    <i class="fa-solid fa-plus"></i>
    New Chat
</button>

        <ul>

            <li>
                <a href="askai.html">
                    <i class="fa-solid fa-robot"></i>
                    Ask AI
                </a>
            </li>

            <li>
                <a href="studyhelp.html">
                    <i class="fa-solid fa-book"></i>
                    Study Help
                </a>
            </li>

            <li>
                <a href="examhelp.html">
                    <i class="fa-solid fa-file-pen"></i>
                    Exam Help
                </a>
            </li>

            <li>
                <a href="technical.html">
                    <i class="fa-solid fa-laptop-code"></i>
                    Technical
                </a>
            </li>

        </ul>

        <div class="sidebar-footer">
            EduNexa AI v1.0
        </div>

    </div>

    <!-- Main Content -->

    <div class="main">

        <div class="header">

            <h1>Welcome to EduNexa AI</h1>

            <p>
                Your Intelligent College Learning Assistant
            </p>

        </div>

        <div class="hero">

            <div class="robot">
                🤖
            </div>

            <h2>Hello Student!</h2>

            <p>
                Ask questions, prepare for exams,
                improve technical skills and study smarter.
            </p>

        </div>

        <div class="cards">

            <a href="askai.html" class="card">
                <h3>🤖 Ask AI</h3>
                <p>Get instant answers.</p>
            </a>

            <a href="studyhelp.html" class="card">
                <h3>📚 Study Help</h3>
                <p>Study plans and tips.</p>
            </a>

            <a href="examhelp.html" class="card">
                <h3>📝 Exam Help</h3>
                <p>Exam preparation guide.</p>
            </a>

            <a href="technical.html" class="card">
                <h3>💻 Technical</h3>
                <p>Programming resources.</p>
            </a>

        </div>

    </div>

</div>
<script>
function newChat(){
    window.location.href = "askai.html";
}
</script>
</body>
</html>


style.css
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#0f172a;
color:white;
}

.container{
display:flex;
height:100vh;
}

/* SIDEBAR */

.sidebar{
width:260px;
background:#111827;
padding:20px;
display:flex;
flex-direction:column;
}

.logo h2{
margin-bottom:5px;
color:#06b6d4;
}

.logo p{
font-size:14px;
color:#ccc;
}

.new-chat{
margin-top:25px;
padding:12px;
border:none;
border-radius:10px;
background:#06b6d4;
color:white;
font-size:16px;
cursor:pointer;
}

.new-chat:hover{
background:#0891b2;
}

.sidebar ul{
list-style:none;
margin-top:25px;
}

.sidebar li{
margin-bottom:12px;
}

.sidebar a{
text-decoration:none;
color:white;
display:block;
padding:14px;
background:#1e293b;
border-radius:10px;
transition:0.3s;
}

.sidebar a:hover{
background:#06b6d4;
transform:translateX(5px);
}

.sidebar-footer{
margin-top:auto;
font-size:13px;
color:#aaa;
}

/* MAIN */

.main{
flex:1;
padding:30px;
overflow:auto;
}

.header{
text-align:center;
margin-top:20px;
}

.header h1{
font-size:38px;
}

.header p{
margin-top:10px;
color:#cbd5e1;
}

/* HERO */

.hero{
text-align:center;
margin-top:50px;
}

.robot{
font-size:80px;
}

.hero h2{
margin-top:15px;
font-size:30px;
}

.hero p{
margin-top:10px;
color:#cbd5e1;
}

/* CARDS */

.cards{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:25px;
margin-top:50px;
}

.card{
background:#1e293b;
padding:30px;
border-radius:15px;
text-decoration:none;
color:white;
transition:0.3s;
}

.card:hover{
transform:translateY(-8px);
box-shadow:0 10px 25px rgba(6,182,212,0.4);
}

.card h3{
margin-bottom:10px;
}

/* MOBILE */

@media(max-width:768px){

.container{
flex-direction:column;
}

.sidebar{
width:100%;
height:auto;
}

.cards{
grid-template-columns:1fr;
}

.header h1{
font-size:28px;
}

}
.chat-container{
width:100%;
height:100vh;
display:flex;
flex-direction:column;
background:#0f172a;
}

.chat-header{
padding:20px;
background:#111827;
text-align:center;
}

.chatbox{
flex:1;
padding:20px;
overflow-y:auto;
}

.user-message{
background:#06b6d4;
padding:12px;
margin:10px 0;
border-radius:12px;
max-width:70%;
margin-left:auto;
}

.bot-message{
background:#1e293b;
padding:12px;
margin:10px 0;
border-radius:12px;
max-width:70%;
}

.input-area{
display:flex;
padding:20px;
background:#111827;
}

.input-area input{
flex:1;
padding:14px;
border:none;
border-radius:10px;
outline:none;
}

.input-area button{
margin-left:10px;
padding:14px 20px;
border:none;
background:#06b6d4;
color:white;
border-radius:10px;
cursor:pointer;
}
.page-container{
padding:40px;
min-height:100vh;
background:#0f172a;
}

.page-header{
text-align:center;
margin-bottom:40px;
}

.page-header h1{
font-size:40px;
margin-bottom:10px;
}

.page-header p{
color:#cbd5e1;
font-size:18px;
}

.back-btn{
text-align:center;
margin-top:40px;
}

.back-btn a{
text-decoration:none;
background:#06b6d4;
color:white;
padding:12px 25px;
border-radius:10px;
}

.back-btn a:hover{
background:#0891b2;
}
.card{
cursor:pointer;
}

.instruction-box{
display:none;
max-width:800px;
margin:40px auto 20px;
padding:30px;
background:#1e293b;
border:1px solid #06b6d4;
border-radius:18px;
box-shadow:0 10px 30px rgba(0,0,0,0.4);
animation:slideUp 0.3s ease;
}

.instruction-box h2{
color:#06b6d4;
margin-bottom:15px;
}

.instruction-box p{
color:#e2e8f0;
font-size:16px;
line-height:1.8;
}

.instruction-box button{
margin-top:20px;
padding:10px 25px;
border:none;
border-radius:8px;
background:#06b6d4;
color:white;
cursor:pointer;
font-size:15px;
}

.instruction-box button:hover{
background:#0891b2;
}

@keyframes slideUp{

from{
opacity:0;
transform:translateY(20px);
}

to{
opacity:1;
transform:translateY(0);
}

}
.detail-container{
max-width:1000px;
margin:auto;
padding:40px 25px;
}

.detail-header{
text-align:center;
margin-bottom:35px;
}

.detail-icon{
font-size:70px;
margin-bottom:15px;
}

.detail-header h1{
font-size:38px;
color:#06b6d4;
}

.detail-header p{
margin-top:10px;
color:#cbd5e1;
font-size:17px;
}

.detail-card{
background:#1e293b;
padding:30px;
margin-bottom:20px;
border-radius:18px;
border:1px solid #334155;
}

.detail-card h2{
color:#06b6d4;
margin-bottom:18px;
}

.detail-card p{
color:#e2e8f0;
line-height:1.8;
margin-bottom:12px;
}

.detail-card ul{
padding-left:25px;
color:#e2e8f0;
line-height:2;
}

.steps div{
background:#0f172a;
padding:15px;
margin:10px 0;
border-radius:10px;
color:#e2e8f0;
}

.steps span{
display:inline-flex;
align-items:center;
justify-content:center;
width:30px;
height:30px;
background:#06b6d4;
border-radius:50%;
margin-right:12px;
font-weight:bold;
}

.back-buttons{
display:flex;
justify-content:center;
gap:15px;
margin-top:30px;
}

.back-buttons a{
text-decoration:none;
background:#06b6d4;
color:white;
padding:12px 20px;
border-radius:10px;
}

.back-buttons a:hover{
background:#0891b2;
}

data.js
const answers = {

"dbms":
`DBMS stands for Database Management System.
It is used to store and manage data.
It allows users to add, update and delete data.
Examples are MySQL, Oracle and MongoDB.`,

"sql":
`SQL stands for Structured Query Language.
It is used to communicate with databases.
We can insert, update, delete and retrieve data.
SQL is commonly used with relational databases.`,

"oops":
`OOPS stands for Object-Oriented Programming.
It is a programming concept based on objects and classes.
The main concepts are Inheritance and Polymorphism.
Encapsulation and Abstraction are also important concepts.`,

"java":
`Java is a popular object-oriented programming language.
It is used to develop web, mobile and desktop applications.
Java is platform independent.
It is widely used in software development.`,

"python":
`Python is a simple and high-level programming language.
It has easy and readable syntax.
Python is used in web development, AI and data science.
It is beginner-friendly and widely used.`,

"html":
`HTML stands for HyperText Markup Language.
It is used to create the structure of web pages.
HTML uses tags to display text, images and links.
It is the basic technology of web development.`,

"css":
`CSS stands for Cascading Style Sheets.
It is used to design and style web pages.
CSS controls colors, fonts, spacing and layouts.
It makes websites attractive and responsive.`,

"javascript":
`JavaScript is a programming language used on websites.
It makes web pages interactive and dynamic.
It can handle buttons, forms and user actions.
JavaScript is widely used in frontend development.`,

"react":
`React is a JavaScript library for building user interfaces.
It is mainly used to create modern web applications.
React uses reusable components.
It is developed and maintained by Meta.`,

"nodejs":
`Node.js is a JavaScript runtime environment.
It allows JavaScript to run outside the browser.
It is commonly used for backend development.
Node.js can be used to build fast web servers.`,

"mongodb":
`MongoDB is a NoSQL database.
It stores data in document format.
It is flexible and easy to work with.
MongoDB is commonly used with Node.js applications.`,

"api":
`API stands for Application Programming Interface.
It allows different software applications to communicate.
APIs are commonly used to send and receive data.
They are important in modern web applications.`,

"interview":
`Prepare well before attending a technical interview.
Revise programming, DBMS, OOPS and project concepts.
Practice common HR and technical questions.
Stay confident and explain your answers clearly.`,

"exam":
`Start your exam preparation with a proper timetable.
Complete important topics before the exam.
Revise regularly and practice previous questions.
Take short breaks to maintain concentration.`,

"placement":
`For placement, improve coding and aptitude skills.
Revise important technical subjects like Java and DBMS.
Practice mock interviews and communication skills.
Keep your resume simple and project-focused.`,

"resume":
`A resume should be simple and professional.
Mention your education, technical skills and projects.
Add internships, certifications and achievements.
Try to keep your resume within one or two pages.`,

"who are you":
`I am EduNexa AI, your student learning assistant.
I can help you with study and technical questions.
You can ask me about exams, programming and placement.
I am here to make your learning easier.`,

"hello":
`Hello! 👋 Welcome to EduNexa AI.
I am your student learning assistant.
You can ask me about technical subjects or exams.
How can I help you today?`

};

script.js
function answerQuestion(){

let input =
document.getElementById("question");

let question = input.value.trim();

if(question === ""){
return;
}

let chatbox =
document.getElementById("chatbox");

chatbox.innerHTML +=
`
<div class="user-message">
${question}
</div>
`;

let reply =
getBotResponse(question);

chatbox.innerHTML +=
`
<div class="bot-message">
${reply}
</div>
`;

input.value="";

chatbox.scrollTop =
chatbox.scrollHeight;
}

document.addEventListener(
"keypress",
function(e){

if(e.key==="Enter"){
answerQuestion();
}

});
