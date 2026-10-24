<script>
    import '@fontsource-variable/source-code-pro';
    import '@fontsource/gugi';

    import presentation from '$lib/assets/projects/laserSafetyCompliance/stfcPresentation.pdf';
    import github from '$lib/assets/icons/github.svg';

    import activityDiagram from '$lib/assets/projects/laserSafetyCompliance/activityDiagram.png';

</script>

<style>
    .body {
        margin: 0;
        padding: 0;
    }
    
    .header {
        background-image: url('/src/lib/assets/background-2.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 50% 35%;
        text-align: center;
        padding: 40px;
        color: white;
        height: auto;
    }

    .header h1 {
      font-family: 'Gugi', system-ui;        
      font-size: 4vh;
      color: rgb(255, 255, 255);
      padding: 20px;
      margin: 10px auto;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); 
    }

    .header h2 {
      font-family: 'Source Code Pro Variable', monospace;
      font-size: 2vh;
      color: rgb(255, 255, 255);
      padding: 20px;
      margin: 10px auto;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); 
    }

    .buttons {
        display: flex;
        justify-content: center;
        padding: 10px;
        margin: 10px auto;
    }

    .buttons img {
        filter: invert(1);
        height: 10vh;
        color: #ffffff;
        border: none;
        transition: all 0.3s ease;
        cursor: pointer;
    }

    .buttons img:hover {
        filter: invert(0);
        transform: scale(1.1);
    }

    .content-row {
        padding: 20px;
        background-color: #ffffff;
        color: #ffffff;
        background: rgba(0, 0, 0, 0.6);
        border-radius: 5px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        margin: 10px 10px;
    }

    .pdfcontainer {
        background-color: #f1f1f1;
        border-radius: 10px;
        padding: 20px;
        margin: 10px auto;
        display: flexbox;
        justify-content: center;
        align-items: center;
        height: auto;
    }

    .pdfcontainer iframe {
        border: none;
        width: 100%;
        height: 50vh;
    }

    .content-row h1 {
        font-family: 'Gugi', system-ui;        
        font-size: 3vh;
        color: #ffffff;
        text-align: center;
        margin: 10px auto;
    }

    .content-row p {
        font-family: 'Source Code Pro Variable', monospace;
        font-size: 3vh;
        color: #ffffff;
        line-height: 1.6;
        padding: 20px;
        margin: 10px auto;
        text-align: center;
    }

    .content-row ul {
        margin-top: 10px;
        padding-left: 20px;
    }

    .content-row li {
        margin-bottom: 10px;
        font-family: 'Source Code Pro Variable', monospace;

    }

    .content-row img {
        display: block;
        margin: 0 auto; 
        max-width: 90%; 
        height: auto;
        background-color: rgba(255, 255, 255, 0.8); 
        border-radius: 5px; 
        padding: 5px; 
    }

    .separator {
        content: "";
        display: block;
        height: 2px;
        background-color: rgb(255, 255, 255);
        border-radius: 1px; 
        width: 80%; 
        margin: 20px auto;
    }

    @media (max-width: 768px) {

    .header h1 {
        padding: 10px;
        margin: 15px auto;
    }

    .header h2 {
        padding: 10px;
        margin: 5px auto;
    }


    .pdfcontainer {
        height: 60vh;
    }

    .pdfcontainer iframe {
        width: 100%;
        height: 50vh;
    }
    
    
}
</style>

<div class="body">
<div class="header">
<h1>LASER Safety Compliance Service</h1>
<h2>Nov 2023 - Present | PYTHON/C# · GitHub - Open source</h2>
<div class="buttons">
    <a href="https://github.com/sarahshamilton/LASERLabSafetyService_Archive">
        <img src="{github}"/>
    </a>
</div>
</div>
<div class="content-row">
    <h1>Project overview</h1>
    <p style="text-align: center;"> 
        Built to ensure the well-being of users, the system is designed to implement a safety compliance program that monitors LASER’s lab space. Upon signing in, users are required to verify their safety, with the program conducting regular check-ins every 30 minutes. Exhibited critical thinking, time management, and problem-solving skills during the initial cycle of this project.
    </p>
    <ul>
        <li>Demonstrated the ability to program with Python, utilising the language, external libraries, and API calls for initial rapid prototyping followed by usage during the development stage. Additionally offers flexibility for deployment across different configurations of hardware and operating systems.</li>
        <li>The application was built to support 20 - 30 users and was developed to meet the specifications outlined by both the department and the committee during the requirements gathering stage of the Software Development Cycle.</li>
        <li>Usage of Linux with systemd for deployment, utilising a unit file.</li>
        <li>Currently working on a new version for this academic year, utilising C# due to an enhanced feature set and changing requirements.</li>
    </ul>
</div>
<div class="content-row">
    <h1>System design and implementation presentation</h1>
    <p style="text-align: center;"> Enclosed below is a presentation of the software, displaying the use-case, system design and implementation along with the deployment of the project:</p>
    <div class="separator"></div>
        <div class="pdfcontainer">
            <iframe src="{presentation}" />
        </div>
</div>
<div class="content-row">
    <h1>System activity diagram</h1>
    <p style="text-align: center;"> Enclosed below is the system activity diagram, visually illustrating the workflow of the LASER Safety Compliance Service:</p>
    <div class="separator"></div>
        <img src="{activityDiagram}"/>
    </div>
</div>
