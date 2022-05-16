# mock_repo_manager_apps
This is a mock repo for ECell IITM 2022-2023 managerial applications
<!DOCTYPE html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<head>
    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
    <script type="text/javascript">
        google.charts.load('current', {'packages':['corechart']});
        google.charts.setOnLoadCallback(drawAllChart);

      function drawAllChart() {

        var data = google.visualization.arrayToDataTable([
        ['Expenditure', 'Amount'],
          ['Food', 200],
          ['Savings', 350],
          ['Medical', 100],
          ['Coffee', 150],
          ['Study-related', 250],
          ['Phone bills', 180],
          ['Entertainment', 200]
        ]);

        var options = {
        title: 'BUDGET',
        height: 400,
        width: 500,
        legend: {'position': 'right'},
        titleTextStyle: {
                color: "black",               
                fontName: "Tempus sans ITC",    
                fontSize: 25,               
                bold: true,                 
            }
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart'));

        chart.draw(data, options);
      }
    </script>

<script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
<script type="text/javascript">
  google.charts.load("current", {packages:["corechart"]});
  google.charts.setOnLoadCallback(drawStudyChart);
  function drawStudyChart() {
    var data = google.visualization.arrayToDataTable([
      ['Items', 'Cost'],
      ['Printout', 50],
      ['Stationary', 120],
      ['Notebooks', 80]
    ]);

    var options = {
      title: 'STUDY BUDGET',
      pieHole: 0.4,
      width: 500,
      height: 400,
      titleTextStyle: {
                color: "black",               
                fontName: "Tempus sans ITC",    
                fontSize: 25,               
                bold: true,                 
            }
    };

    var chart = new google.visualization.PieChart(document.getElementById('donutchart'));
    chart.draw(data, options);
  }
</script>

    <title>
        WMO E-CELL
    </title>
</head>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
<style>

.navbar{
  height: 100%;
  width: 13%;
  position: fixed;
  z-index: 2;
  top: 0;
  left: 0;
  padding-top: 20px;
  padding-left: 10px;
  color:white;
  background-color: rgb(0, 51, 117);

  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  min-width: 200px;
  min-height: 500px;
}

.main{
  display: flex;
  flex-wrap: wrap; 
  flex-direction: column;
  z-index: 0;
}

.submain{
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  z-index: 1;
}
 
.user {
  height: 100%;
  width: 67%;
  position: fixed;
  z-index: 0;
  top: 0;

  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  min-width: 800px;
  min-height: 500px;

  background-color: white;
  color:midnightblue;
  margin-left: 1170px;
  margin-top: 20px;
}

.split3{
  height: 100%;
  width: 20%;
  z-index: 1;
  top: 0;
  overflow-x: hidden;
  margin-left: 230px;
  margin-top: 60px;

  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  min-width: 350px;
  min-height: 100px;
  max-height: 700px;
}

.right{
    right:0;
    background-color: rgb(255, 255, 255);
}

.graphs{
    margin-left: 518px;
    margin-top: -650px;
    background-color: white;
}

.calimg{
    margin-left: 580px;
    margin-top: -260px;
}

.text:hover{
  color: orange;
}

.text2:hover{
  color:darkcyan;
}

#p1{
  border: 3px solid orange;
  padding: 5%;
  font-family: "Algerian";
  font-size: 20px;
  margin-right: 20px;
  margin-left: 20px;
}

#p2{
  border: 3px solid orange;
  padding: 5%;
  width: 200px;
  height: 150px;
  margin-right: 30px;
  font-family: "Algerian";
}

.twoboxes{
  display: flex;
  flex-wrap: wrap;
}

.zoom{
  padding: 10px;
  transition: transform 0.2s;
}

.zoom:hover{
  transform: scale(1.1);
}

</style>

<link rel="stylesheet" href="https://maxst.icons8.com/vue-static/landings/line-awesome/line-awesome/1.3.0/css/line-awesome.min.css">
    <body>

        <div class="navbar" style="font-family:Bradley Hand ITC">   <!-- NavBar -->
            <h4><b>
            <span class="las la-home"></span>
            <span>Dashboard</span><br><br>
            <span class="las la-address-card"></span>
            <span>Contact details</span><br><br>
            <span class="las la-list-ul"></span>
            <span>Daily goals</span><br><br>
            <span class="las la-coins"></span>
            <span>Savings</span><br><br>
            <span class="las la-pen-nib"></span>
            <span>Projects</span><br><br>
            <span class="las la-clipboard"></span>
            <span>Deadlines</span><br><br><br><br><br><br><br><br><br><br><br>
            <span class="las la-power-off"></span>
            <span>Logout</span><br><br>
            </h4></b>
        </div>

        <div class="user text" style="font-family:Calibri"> <!-- User -->
          <h3>
              <span class="las la-bell"></span>
              <span>&nbsp; &nbsp; &nbsp; Prarthana Ganesh </span>
              <span class="las la-user"></span>
          </h3>
        </div>

        <div class="main">
          <div class="split3"> <!-- To-Do list -->
            <p><font face="Tempus sans ITC" size="20" color="darkblue"><b>TO-DO LIST</p></b></font>
              <textarea rows="1" cols="35"></textarea>
              <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
              &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
              &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
              <input class="btn btn-primary" type="Submit"/></p>
              <br><br>
              <h5>
        
              <span class="las la-circle"></span>
              <span>PH assignment</span><br><br>
              <span class="las la-circle"></span>
              <span>CFI applications</span><br><br>
              <span class="las la-circle"></span>
              <span>HS poster-making</span><br><br>
              <span class="las la-circle"></span>
              <span>CH1020 project</span><br><br>
              <span class="las la-check-circle"></span>
              <span>Trimester-3 registration</span><br><br>
              <span class="las la-check-circle"></span>
              <span>E-Cell WMO applications</span><br><br>
            </h5>

            <div class="text2 zoom">
            <p id="p1">8:00 AM IST<br>
            Day: Tuesday<br>
            Date: 3rd May 2022</p>
            </div>
          </div>
         <div class="submain">
          <div class="graphs"> <!-- Graphs -->
          <table class="columns">
              <tr>
                <td><div id="piechart"></div></td>
                <td><div id="donutchart"></div></td>
              </tr>
            </table>
          </div>

          <div class="calimg"> <!-- Calendar Image + Two boxes -->
            <img src="D:\VS Code\E-Cell WMO\project deadlines and assignment submissions.png" height="400px" width="680px">
            <div style="float:right">
              <br>
              <div id="p2">
                <p>
                  <h3><center>Completed:</center></h3>
                  <h1><center>2</center></h1> 
                </p>
              </div><br>
              <div id="p2">
                <p>
                  <h3><center>Pending:</center></h3> 
                  <h1><center>4</center></h1>
                </p>
              </div>
            </div>
          </div>
         </div>  
        </div>

    </body>
</html>
