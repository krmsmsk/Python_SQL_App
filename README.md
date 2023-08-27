<div align="center">
  <img height="300" src="https://media1.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif?cid=ecf05e477nfy3cs4ufmdpspwzxlk03sqdm6wwxagyef5dfz7&ep=v1_gifs_related&rid=giphy.gif&ct=g"  />
</div>

###

<h1 align="center">Report App</h1>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/microsoftsqlserver/microsoftsqlserver-plain.svg" height="40" alt="microsoftsqlserver logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" height="40" alt="flask logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" height="40" alt="django logo"  />
</div>

###

<p align="center">A report program which we have to meet request from our business lines.</p>

###

<h2 align="left">My Aim</h2>

###

<p align="left">Unfortunately, reporting requests coming from various business units are not always satisfactorily met using the tools sanctioned by the bank. In relation to a reporting request that the team has examined but hasn't been able to find a solution for, I will introduce a program that I have developed on my personal computer (as a preliminary effort). The purpose of this program is to address a reporting issue that we have been attempting to resolve using SSRS but have consistently encountered errors.</p>

###

<h2 align="left">Summary</h2>

###

<p align="left">I have created three separate functions for essentially the same request that comes from the same business unit but at three different stages. In each query, I retrieve certain parameters (following the logic of SSRS) that need to be used in the SQL query and embed them within the query. Subsequently, I establish a connection to the MSSQL Server and execute the query. I place the output of the query into a dataframe, display the first ten rows (top 10) to the user, and inquire whether they would like to download the entire output as an Excel file. If the user is satisfied with the output and wishes to download it as an Excel file, I upload the file to the bank's shared folder. This way, the business unit can obtain the same result as the report they intend to generate using SSRS.</p>

###

<h3 align="left">- Why we need this program?</h3>

###

<p align="left">Because the result of the requested query resides within a significantly large table, and unfortunately, the server hosting this table has been poorly designed. Consequently, fetching information for just one DK_NO takes around half an hour for approximately 200 thousand rows of data. Given this scenario, even a direct SSRS connection struggles to retrieve the results for a single DK_NO. Our team lacks the authorization to intervene with the server, database, or table in question. Therefore, we needed to devise a solution based on the prepared report. Thanks to the program I developed, we can input 4-5 specific DK_NO values into the program all at once and, after approximately 3 hours, obtain the results without encountering any issues.</p>

###

<h3 align="left">NOTE :</h3>

###

<p align="left">- The program can only be utilized by our own team.<br>- The outputs I will show you below are different from those at my workplace. The outputs here are preliminary results developed while creating this program.<br>- At my workplace, the program is used with an appealing front-end design, incorporating the DJANGO library. I will soon adjust and update my write-up to include the same front-end design for these outputs.<br><br>You can review the program's outputs from the images below:</p>

###

<div align="center">
  <img height="500" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/%C3%B6rneklem.png?raw=true"  />
</div>

###

<p align="center">Sample Code</p>

###

<div align="center">
  <img height="100" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/1.png?raw=true"  />
</div>

###

<div align="center">
  <img height="80" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/2.png?raw=true"  />
</div>

###

<div align="center">
  <img height="99" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/3.png?raw=true"  />
</div>

###

<div align="center">
  <img height="80" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/4.png?raw=true"  />
</div>

###

<div align="center">
  <img height="20" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/%C3%A7%C4%B1kt%C4%B1.png?raw=true"  />
</div>

###

<div align="center">
  <img height="400" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/%C3%A7%C4%B1kt%C4%B1%201.png?raw=true"  />
</div>

###

<p align="center">Place where I downloaded that excel</p>

###

<div align="center">
  <img height="150" src="https://github.com/krmsmsk/Resimler/blob/main/Rapor%20Uygulamas%C4%B1/%C3%A7%C4%B1kt%C4%B1%202.png?raw=true"  />
</div>

###

<p align="center">It is purely coincidental that only 10 rows have arrived. It normally returns all matching data.</p>

###
