<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="survay.css">
<title>Save Web Form Data to Spreadsheets - Location eveluation Form</title>
<script
  src="https://code.jquery.com/jquery-3.4.1.js"
  integrity="sha256-WpOohJOqMqqyKL9FccASB9O0KwACQJpFTUBLTYOVvVU="
  crossorigin="anonymous"></script>
<script>
function SubForm (){
    $.ajax({
        url:'https://api.apispreadsheets.com/data/pyjjVR63gEC4qWT7/',
        type:'post',
        data:$("#myForm").serializeArray(),
        success: function(){
          alert("Location evaluation Submitted :)")
        },
        error: function(){
          alert("There was an error :(")
        }
    });
}
</script>
</head>
<body id="back">
  <form id="myForm">
    <label>Staff Name</label>
    <br/>
    <input name="staff_name" />
    <br/>
    <label>MRN</label>
    <br/>
    <input name="mrn" />
    <br/>
    <label>Location</label>
    <br/>
    <input type="radio" id="location" name="location" value="acc" /> ACC
    <input type="radio" id="location" name="location" value="oncology" /> ONCOLOGY
    <input type="radio" id="location" name="location" value="cardiac" /> CARDIAC<br/>
    <br/>
 <p>Please evaulate the following with 10 being the highest and 1 as the lowest</p>
    <li>Environment and Facilities</li>
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="1" /> 1 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="2" /> 2 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="3" /> 3 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="4" /> 4 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="5" /> 5 &nbsp; <br/>
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="6" /> 6 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="7" /> 7 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="8" /> 8 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="9" /> 9 &nbsp;
    <input type="radio" id="Environment and Facilities" name="Environment and Facilities" value="10" /> 10 <br/>
    <br/>
    <li>Time access to service</li>
    <input type="radio" id="Time access to service" name="Time access to service" value="1" /> 1 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="2" /> 2 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="3" /> 3 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="4" /> 4 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="5" /> 5 &nbsp; <br/>
    <input type="radio" id="Time access to service" name="Time access to service" value="6" /> 6 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="7" /> 7 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="8" /> 8 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="9" /> 9 &nbsp;
    <input type="radio" id="Time access to service" name="Time access to service" value="10" /> 10 <br/>
    <br/>
    <li>Staff experience and engagement</li>
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="1" /> 1 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="2" /> 2 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="3" /> 3 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="4" /> 4 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="5" /> 5 &nbsp;<br/>
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="6" /> 6 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="7" /> 7 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="8" /> 8 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="9" /> 9 &nbsp;
    <input type="radio" id="Staff experience and engagement" name="Staff experience and engagement" value="10" /> 10 <br/>
    <br/>
    <li>Information and communication</li>
    <input type="radio" id="Information and communication" name="Information and communication" value="1" /> 1 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="2" /> 2 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="3" /> 3 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="4" /> 4 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="5" /> 5 &nbsp;<br/>
    <input type="radio" id="Information and communication" name="Information and communication" value="6" /> 6 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="7" /> 7 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="8" /> 8 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="9" /> 9 &nbsp;
    <input type="radio" id="Information and communication" name="Information and communication" value="10" /> 10 <br/>
    <br/>
    <li>Patient voice and response </li>
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="1" /> 1 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="2" /> 2 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="3" /> 3 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="4" /> 4 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="5" /> 5 &nbsp;<br/>
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="6" /> 6 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="7" /> 7 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="8" /> 8 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="9" /> 9 &nbsp;
    <input type="radio" id="Patient voice and response" name="Patient voice and response" value="10" /> 10 <br/>
    <br/>
  </form>
  <button onclick="SubForm()">Submit</button>
</body>
</html>
