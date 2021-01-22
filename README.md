# tabular-structure



HTML FILE


<div class="header">

    <h3>Header</h3>
</div>


<body>
    <div id="container">
        <div id="nameDiv" class="input"> NAME:<input id="name" type="text" placeholder="K.Supraja"/></div>
    
        <div class="input"> AGE <input id="age" type ="text" placeholder="18"/></div>

        <div class="input" >EMAIL ID <input id="emailid" type="text" placeholder="suprajakurella73@gmail.com"/></div>
    
        <button id="entry"> INPUT ENTRY</button>
    
    </div>
    <table id="display">



        <tr>
       
           <th> NAME</th>
           
           <th> age</th> 
           <th>EMAIL ID</th>
           
           
       
       </table>
    <link  type="text/css" href="sup.css" media="screen"/>
    <script src="index.js" type="text/javascript">
    
</script>
   



<img src="C:\Users\theam\Downloads\Radha krishna Cute art Mobile Wallpaper.jpg" alt="related to web development"  width="200px" height="200px">
<video width="200px" height="200px" src="C:\Users\theam\Desktop\funny pics\new yr video.mp4" type="video/mp4" autoplay loop alt="New year wishes video">
</video> </br>


<div class ="footer">
<h3>  Footer</h3>
</div>
</body>










CSS FILE



<head> 
    <title> PAGE TITLE</title>
    <meta charset ="UTF-8">
    <meta name ="viewport" content =" width =device-width, initial-scale=1">
    <style>
        body 
        {
            font-family: Arial;
            
            margin:0;
        }
        input{
            {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    box-sizing: border-box;
} 
        }
        
        .header
        {
            padding: 60px;
            text-align:center;
            background:black;
            color : white;
            font-size: 20px;

        }
        .content
        {
            padding : 20px;

        }
    </style>
</head>


JS FILE



document.body.style.backgroundColor="green";
if (typeof document !== 'undefined')
{
    

var row=1;
var entry = document.getElementById("entry");
entry.addEventListener("click", displayDetails);

window.addEventListener('load',displayDetails,false)

function displayDetails()
{
    var name=document.getElementById("name").nodeValue;
    var age=document.getElementById("age").nodeValue;
    var emailid=document.getElementById("emailid").nodeValue;
   if(!name || !age || !emailid)
    {
        alert("please fill all the boxes"); 

    }
    var display = document.getElementById("display");
    var newRow= display.insertRow(row);
    var cell1= newRow.insertCell(0);
    var cell2= newRow.insertCell(1);
    var cell3=newRow.insertCell(2);

    cell1.innerHTML=name;
    cell2.innerHTML= age;
    cell2.innerHTML= age;
    row++;

}
}
