---
layout: page
permalink: /posts/
title: posts
description: life and work environment
nav: true
cateogry: work
nav_order: 3
---

<html>

<head>
    <title>Posts</title>
        <style>
            .horizontal-nav {
                display: inherit;
                justify-content: space-between;
                align-items: center;
                list-style: flex;
                padding: 0;
                margin: 10;
                }

                .horizontal-nav li {
                margin: 0 15px;
                }

                .horizontal-nav li a {
                background-color: white;
                text-decoration: none;
                color: #333;
                }
    </style>

</head>


<body>
    <div class="navbar">
        <ul class="horizontal-nav">
            <li><a href="#cognitive-bias">Cognitive Bias</a></li>
            <li><a href="#what-is-a-phd">What is a PhD</a></li>
            <li><a href="#research-tools">Research Tools</a></li>
            <li><a href="#working-hours">Working Hours Tracker</a></li>
            <li><a href="#charity-foundation">MasieraDay</a></li>    
        </ul>
    </div>
    
<p id="charity-foundation"></p>
<h4>#5 MasieraDay</h4>
<h7>Masieraday is an association established for charitable purposes in memory of Livio Romare, a <a href="https://en.wikipedia.org/wiki/Schio">Schio</a> volleyball champion who always had a thought for the community and young people, leading him to work personally for the good of those less fortunate. <br>Masieraday is under the patronage of the Italian Ministry of Education, University and Research.<br><br></h7>
<h5><a href="https://www.masieraday.it/en/">MasieraDay (ENG)</a> - <a href="https://www.masieraday.it/">MasieraDay (IT)</a>   <img src="https://pieroromare.github.io/assets/img/masieraday.png" alt="MasieraDay Icon" width="200"></h5>
<ul>
<li>Since 2015, organization of volleyball matches with MasieraDay.</li>
<li>Since 2017, organization of volleyball tournaments with MasieraCup.</li> 
<li>Since 2018, donation of 5 scholarships each year with MasieraAcademy.</li>
</ul>
Thanks to your <a href="https://www.masieraday.it/dona/">donations</a>, aid has been devolved to Adwa Ethiopia, Vita Onlus project, AViLL (association against leukemia and lymphomas), Burundi Chiama (long distance adoptions). <br>
On 5th December 2015 the Schio sports hall was named <a href="https://it.wikipedia.org/wiki/Palasport_Livio_Romare">Palasport Livio Romare</a>. <br>
You can relive the association's events organised via the <a href="https://www.youtube.com/@masieradaylivioromare7060">YouTube channel</a>.<br>
Testimonials: <em>Andrea Lucchetta, Maurizia Cacciatori, Marco Berry, Robert Grabert, Eugenio Finardi, Giancarlo Caselli, Tina Montinaro, Roberto Baggio, Jury Chechi, Paolo Simoncelli, Simona Atzori, Maxime Mbandà, Javier Zanetti, Sammy Basso, Federica Pellegrini, Roberto Vecchioni, Sandrine Gruda, Laura Roveri, Carlo Nordio, Manuel Bortuzzo, Erika Stefani, Ferdinando De Giorgi, Daniele Cassioli, Roberto Mancini.</em><br><br>
"I have always believed in team spirit, both in sport and in life. You young people are the future... be a team! And you will overcome all of life's obstacles" Livio (1963-2014).

<hr class="section-divider">

<p id="working hours"></p>
<h4>#4 Working Hours Tracker</h4>
<h7>This AppleScript is designed exclusively for MacBooks and is not compatible with iPhones. It leverages iOS Shortcuts to streamline time tracking effortlessly.</h7><br>
<em>Start Time: Click the shortcut once, and it will automatically update your "Working Time" note with the current start time. This marks the beginning of your work session.<br>
Finish Time: When your work session is complete, click the shortcut again. This action will generate the finish time, indicating the end of your work session.</em><br><br>
<h5>Tracker with iOS Notes</h5>
    <ol>
        <li>Open the Notes app on your iOS device.</li>
        <li>Create a new note and give it the title "Working time." You can do this by tapping the "+" button to create a new note and then giving it a title.</li>
        <li>Open the Shortcuts app on your iOS device.</li>
        <li>Tap the "+" button to create a new shortcut.</li>
        <li>In the Shortcuts app, on the right-hand side, you'll see a search bar.</li>
        <li>Type "Execute with AppleScript" in the search bar to find the corresponding action.</li>
        <li>Once you find the "Execute with AppleScript" action, tap on it to add it to your shortcut.</li>
        <li>After adding the action, you can tap on it to configure it.</li>
        <li>Copy and paste the AppleScript code that follows. This code should perform the specific task you want to automate.</li>
        <li>After adding the AppleScript code, you can tap the play button (usually a triangle or "Run" button) at the top right of the Shortcuts app to simulate or test your shortcut.</li>
        <li>Once you've tested your shortcut and it works as expected, you can close it by tapping the "Done" button in the top right corner.</li>
        <li>Your shortcut should now appear in the list of available shortcuts in the Shortcuts app.</li>
        <li>To add the shortcut to your Dock for easy access, you can long-press (or right-click, depending on your device) on the shortcut's icon in the Shortcuts app.</li>
        <li>From the context menu that appears, select the option to "Add to the Dock." This will place the shortcut on your device's Dock for quick access.</li>
    </ol>

<pre style="background-color: #f0f0f0;">
on run {input, parameters}
    tell application "Notes"
        set currentDate to current date
        set currentTime to time string of currentDate
        set currentDateTime to date string of currentDate & " " & currentTime
        
        set workingTimeNote to note "Working time"
        set noteContent to body of workingTimeNote
        
        if noteContent does not contain "start " & (date string of currentDate) then
            set newContent to noteContent & return & "start " & currentDateTime
        else
            set newContent to noteContent & return & "finish " & currentDateTime
        end if
        
        set body of workingTimeNote to newContent
        quit
    end tell
</pre>
<br><br>
<h5>Tracker with a txt file</h5>
<h7>Another version is using the AppleScript + a Python script.</h7>
    <ol>
        <li>Open the terminal and type the following command: pip install datetime</li>
        <li>Create in a folder (that we call yourpath) a Python script that we call (yourpythonscript.py) and copy and paste the following</li>
<pre style="background-color: #f0f0f0;">
import os
import datetime

current_date = datetime.datetime.now()
current_date_string = current_date.strftime('%A, %d %B %Y %H:%M:%S')

desktop_path = os.path.expanduser("yourpath")
text_file_name = "working_hours.txt"
file_path = os.path.join(desktop_path, text_file_name)
if not os.path.isfile(file_path):
    open(file_path, 'w').close()

with open(file_path, 'r') as file:
    file_content = file.read()

if "start" not in file_content.split('\n')[-1]:
    new_content = file_content + f"\nstart {current_date_string}"
else:
    new_content = file_content + f"\nfinish {current_date_string}"

with open(file_path, 'w') as file:
    file.write(new_content)
</pre>
        <li>Now start from the point 3 of the previous version Track with Notes</li>
        <li>In this version, the only difference is that in the AppleScript code in your shortcut add just the following</li>
<pre style="background-color: #f0f0f0;">
do shell script "python3 yourpath/yourpythonscript.py"
</pre>

<hr class="section-divider">

<p id="research-tools"></p>
<h4>#3 Research Tools</h4>
<h7>This is my collection of research tools for academic and scholarly pursuits. These tools enhance my productivity and help me stay organized throughout my journey of discovery.</h7><br><br>
        <h5><a href="https://notion.so">Notion</a><img src="https://pieroromare.github.io/assets/img/notion-icon.png" alt="Notion Icon" width="100"></h5>
        <p>Notion is a versatile tool for task management, project organization, and collaboration.</p>
    <br>
        <h5><a href="https://obsidian.md">Obsidian  </a><img src="https://pieroromare.github.io/assets/img/obsidian-icon.png" alt="Obsidian Icon" width="50"></h5>
        <p>Obsidian is a note-taking app that helps build interconnected knowledge bases.</p>
    <br>
        <h5><a href="https://www.zotero.org">Zotero    </a><img src="https://pieroromare.github.io/assets/img/zotero-icon.png" alt="Zotero Icon" width="50"></h5>
        <p>Zotero is a free and open-source reference management software and research tool.</p>
    <br>
        <h5><a href="https://app.diagrams.net">Draw.io    </a><img src="https://pieroromare.github.io/assets/img/drawio-icon.png" alt="draw.io Icon" width="50"></h5>
        <p>draw.io is a diagramming tool for creating visual representations of data and concepts.</p>
    <br>
        <h5><a href="http://connectedpapers.com">ConnectedPapers    </a><img src="https://pieroromare.github.io/assets/img/connectedpapers-icon.png" alt="ConnectedPapers Icon" width="100"></h5>
        <p>ConnectedPapers.com visualizes citation networks to help researchers explore related academic papers.</p>
    <br>
        <h5><a href="https://researchrabbitapp.com/">ResearchRabbit   </a><img src="https://pieroromare.github.io/assets/img/researchrabbit-icon.png" alt="ResearchRabbit Icon" width="100"></h5>
        <p>ResearchRabbitApp.com provides personalized paper recommendations based on research interests.</p>
    <br>
        <h5><a href="http://elicit.org">Elicit      </a><img src="https://pieroromare.github.io/assets/img/elicit-icon.png" alt="Elicit Icon" width="50"></h5>
        <p>Elicit.org recommends research papers through community-driven curation.</p>
    <br>
        <h5><a href="http://consensus.app">Consensus   </a><img src="https://pieroromare.github.io/assets/img/consensus-icon.png" alt="Consensus Icon" width="100"></h5>
        <p>Consensus.app facilitates collaborative paper selection through group voting.</p>
    <br>
        <h5><a href="http://chatpdf.com">ChatPDF   </a><img src="https://pieroromare.github.io/assets/img/chatpdf-icon.png" alt="ChatPDF Icon" width="50"></h5>
        <p>ChatPDF.com transforms static PDFs into dynamic, collaborative spaces for annotation and discussion.</p>


<hr class="section-divider">

<p id="what-is-a-phd"></p>
<h4>#2 What is a PhD</h4>
<h7>An illustrated guide by Matt Might <a href="http://matt.might.net/articles/phd-school-in-pictures/">source</a><br> 
<div class="container">
    <div class="row">
        <div class="col">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__1.pdf" alt="What_is_a_PhD__1" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__2.pdf" alt="What_is_a_PhD__2" width="345"><br>
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__3.pdf" alt="What_is_a_PhD__3" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__4.pdf" alt="What_is_a_PhD__4" width="345"><br>
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__5.pdf" alt="What_is_a_PhD__5" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__6.pdf" alt="What_is_a_PhD__6" width="345"><br>
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__7.pdf" alt="What_is_a_PhD__7" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__8.pdf" alt="What_is_a_PhD__8" width="345"><br>
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__9.pdf" alt="What_is_a_PhD__9" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__10.pdf" alt="What_is_a_PhD__10" width="345"><br>
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__11.pdf" alt="What_is_a_PhD__11" width="345">
            <img src="https://pieroromare.github.io/assets/pdf/What_is_a_PhD__12.pdf" alt="What_is_a_PhD__12" width="345"><br>
        </div>
    </div>
</div>


<hr class="section-divider">

<p id="cognitive-bias"></p>
<h4>#1 Cognitive Bias</h4>
<h7>Cognitive biases and heuristics serve as mental shortcuts that enable individuals to simplify the complexity of tasks when making judgments and choices. Biases, in turn, arise as the disparities between expected or ideal behavior.</h7>
<p> I like this representation arranged and designed by John Manoogian III (jm3). Categories and descriptions originally by Buster Benson.</p>
<img src="https://pieroromare.github.io/assets/img/cognitive_bias_codex.svg" alt="Cognitive Bias Codex" width="770">