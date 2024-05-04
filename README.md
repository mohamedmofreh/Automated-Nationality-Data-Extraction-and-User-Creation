
  <h1>✏ Project Title:</h1>
  <p>Automated Nationality Data Extraction and User Creation</p>
  <hr>

  <h1>📝 Summary:</h1>
  <dt>The project entails building an RPA (Robotic Process Automation) solution using UiPath Studio to automate several tasks:</dt>
    <dd><h5>1️⃣ Email Handling: <br><br>&emsp;✅The robot listens for a specific email titled 'any email title' reads its attached Excel file, and downloads it to an output folder.</h5></dd>
    <dd><h5>2️⃣ VPN Integration: <br><br>&emsp;✅Before processing data, the robot creates an account on hide.me VPN and enables it to ensure secure browsing.</h5></dd>
    <dd><h5>3️⃣ Configuration Management: <br><br>&emsp;✅Variables are configurable via a `config.csv` file, allowing for easy adjustments.</h5></dd>
    <dd><h5>4️⃣ Account Management: <br><br>&emsp;✅Handles account creation on hide.me website, including activation and password change if necessary.</h5></dd>
    <dd><h5>5️⃣ Data Processing: <br><br>&emsp;✅Reads and processes data tables from the downloaded Excel file.</h5></dd>
    <dd><h5>6️⃣ Information Extraction: <br><br>&emsp;✅Extracts user information from fakenamegenerator.com for each record in the data table.</h5></dd>
    <dd><h5>7️⃣ Account Creation:<br><br>&emsp;✅Signs up on automationexercise.com with extracted information.</h5></dd>
    <dd><h5>8️⃣ API Integration:<br><br>&emsp;✅Calls an API to add user info and retrieves the user ID.</h5></dd>
    <dd><h5>9️⃣ Result Reporting:<br><br>&emsp;✅Saves extracted data and transaction results in `result.xlsx` and `summary.csv` files, respectively.</h5></dd>
    <dd><h5>🔟 Email Notification:<br><br>&emsp;✅Sends `result.xlsx` and `summary.csv` files via email to specified recipients.</h5></dd>
    <dd><h5>1️⃣1️⃣ Process Automation: <br><br>&emsp;✅Initiates processing upon receiving the trigger email and stops if no new email is received within 5 minutes.</h5></dd>
    <dd><h5>1️⃣2️⃣ Development: <br><br>&emsp;✅Developed using UiPath Studio, with no dependency on Orchestrator.</h5></dd>
  <hr>

  <h1>💻 Technologies Used:</h1>
  <ul>
    <li>UiPath</li>
  </ul>
  <hr>

  <h1>♻ Workflow:</h1>
  <ol>
    <dt><h4>1️⃣ Initialization</h4></dt>
      <dd>&emsp; ✅ Load configuration variables from `config.csv`</dd>
      <dd>&emsp; ✅ Open the email inbox</dd>
    <dt><h4>2️⃣ Check for Trigger Email:</h4></dt>
      <dd>&emsp; ✅ Continuously monitor the inbox for an email with the subject "any email title".</dd>
      <dd>&emsp; ✅ If received, proceed; if not, continue checking.</dd>
    <dt><h4>3️⃣ Email Processing:</h4></dt>
      <dd>&emsp; ✅ Read the email and download the attached Excel file ('test.xlsx').</dd>
      <dd>&emsp; ✅ Save the file to the output folder.</dd>
    <dt><h4>4️⃣ VPN Setup:</h4></dt>
      <dd>&emsp; ✅  Open hide.me VPN website.</dd>
      <dd>&emsp; ✅  Create an account if necessary (handle activation or password change emails).</dd>
      <dd>&emsp; ✅  Enable the VPN desktop application.</dd>
    <dt><h4>5️⃣ Data Extraction:</h4></dt>
      <dd>&emsp; ✅  Read data table from the downloaded Excel file.</dd>
    <dt><h4>6️⃣ Data Processing Loop:</h4></dt>
      <dd>&emsp; ✅  Extract user information from fakenamegenerator.com.</dd>
      <dd>&emsp; ✅  Save the extracted data to `result.xlsx`</dd>
      <dd>&emsp; ✅  Sign up on automationexercise.com with the extracted information.</dd>
      <dd>&emsp; ✅  Call the API to add user info and retrieve the user ID.</dd>
      <dd>&emsp; ✅  Save transaction results to `summary.csv`</dd>
    <dt><h4>7️⃣ Email Reporting:</h4></dt>
      <dd>&emsp; ✅  Send `result.xlsx` and `summary.csv` files via email to specified recipients.</dd>
    <dt><h4>8️⃣ Wait for New Email:</h4></dt>
      <dd>&emsp; ✅  Continue checking the inbox for new emails.</dd>
      <dd>&emsp; ✅  If no new email is received within 5 minutes, stop the process.</dd>
   </ol>
