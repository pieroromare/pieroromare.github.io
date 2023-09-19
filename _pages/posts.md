---
layout: page
permalink: /posts/
title: posts
description: my academic environment
nav: true
nav_order: 3
---

<html>

<head>
    <title>Posts</title>
        <style>
        /* CSS for the navigation bar */
        .navbar {
            background-color: #333;
            overflow: hidden;
        }

        .navbar ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        .navbar li {
            display: inline;
            margin: 10px;
        }

        .navbar a {
            color: white;
            text-decoration: none;
        }

        .section-divider {
            border: 5px solid #FFF; /* Add a border */
            margin: 40px 0; /* Adjust spacing as needed */
        }
    </style>

</head>

<body>
    <div class="navbar">
        <ul>
            <li><a href="#cognitive-bias">#1 Cognitive Bias</a></li>
            <li><a href="#research-tools">#2 Research Tools</a></li>
            <li><a href="#working-hours">#3 Working Hours Tracker</a></li>            
        </ul>
    </div>

<hr>

<p id="working hours"></p>
<h4>#3 Working Hours Tracker</h4>
<h7>This AppleScript is designed exclusively for MacBooks and is not compatible with iPhones. It leverages iOS Shortcuts to streamline time tracking effortlessly.</h7><br>
<em>Start Time: Click the shortcut once, and it will automatically update your "Working Time" note with the current start time. This marks the beginning of your work session.<br>
Finish Time: When your work session is complete, click the shortcut again. This action will generate the finish time, indicating the end of your work session.</em><br><br>
    <ol>
        <li>Open the Notes app on your iOS device.</li>
        <li>Create a new note and give it the title "Working time." You can do this by tapping the "+" button to create a new note and then giving it a title.</li>
        <li>Open the Shortcuts app on your iOS device.</li>
        <li>Tap the "+" button to create a new shortcut.</li>
        <li>In the Shortcuts app, on the right-hand side, you'll see a search bar.</li>
        <li>Type "Execute with AppleScript" in the search bar to find the corresponding action.</li>
        <li>Once you find the "Execute with AppleScript" action, tap on it to add it to your shortcut.</li>
        <li>After adding the action, you can tap on it to configure it.</li>
        <li>Copy and paste the AppleScript code that you want to execute into the action. This code should perform the specific task you want to automate.</li>
        <li>After adding the AppleScript code, you can tap the play button (usually a triangle or "Run" button) at the top right of the Shortcuts app to simulate or test your shortcut.</li>
        <li>Once you've tested your shortcut and it works as expected, you can close it by tapping the "Done" button in the top right corner.</li>
        <li>Your shortcut should now appear in the list of available shortcuts in the Shortcuts app.</li>
        <li>To add the shortcut to your Dock for easy access, you can long-press (or right-click, depending on your device) on the shortcut's icon in the Shortcuts app.</li>
        <li>From the context menu that appears, select the option to "Add to the Dock." This will place the shortcut on your device's Dock for quick access.</li>
    </ol>

<pre>
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



<hr class="section-divider">

<p id="research-tools"></p>
<h4>#2 Research Tools</h4>
<h7>This is my collection of research tools for academic and scholarly pursuits. These tools enhance my productivity and help me stay organized throughout my journey of discovery.</h7><br><br>
        <h5><a href="https://notion.so">Notion</a><img src="https://pieroromare.github.io/assets/img/notion-icon.png" alt="Notion Icon" width="100"></h5>
        <p>Notion is a versatile tool for task management, project organization, and collaboration.</p>
    <br>
        <h5><a href="https://obsidian.md">Obsidian  </a><img src="https://pieroromare.github.io/assets/img/obsidian-icon.png" alt="Obsidian Icon" width="50"></h5>
        <p>Obsidian is a note-taking app that helps build interconnected knowledge bases.</p>
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
        <h5><a href="http://inciteful.xyz">Inciteful   </a><img src="https://pieroromare.github.io/assets/img/inciteful-icon.png" alt="Inciteful Icon" width="50"></h5>
        <p>Inciteful.xyz gamifies paper discovery by earning points for reading and reviewing papers.</p>
    <br>
        <h5><a href="http://chatpdf.com">ChatPDF   </a><img src="https://pieroromare.github.io/assets/img/chatpdf-icon.png" alt="ChatPDF Icon" width="50"></h5>
        <p>ChatPDF.com transforms static PDFs into dynamic, collaborative spaces for annotation and discussion.</p>


<hr class="section-divider">


<p id="cognitive-bias"></p>
<h4>#1 Cognitive Bias</h4>
<h7>Cognitive biases and heuristics serve as mental shortcuts that enable individuals to simplify the complexity of tasks when making judgments and choices. Biases, in turn, arise as the disparities between expected or ideal behavior.</h7>
<p> I like this representation arranged and designed by John Manoogian III (jm3). Categories and descriptions originally by Buster Benson.</p>
<img src="https://pieroromare.github.io/assets/img/cognitive_bias_codex.svg" alt="Cognitive Bias Codex" width="770">


</body>

</html>
