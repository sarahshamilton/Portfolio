<script>
    import '@fontsource-variable/source-code-pro';
    import '@fontsource/gugi';

    import presentation from '$lib/assets/projects/laserSafetyCompliance/stfcPresentation.pdf';
    import github from '$lib/assets/icons/github.svg';

    import showcase0 from '$lib/assets/projects/mailLobbyer/1.png';
    import showcase1 from '$lib/assets/projects/mailLobbyer/2.png';



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
        height: 80vh;
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

    .separator {
        content: "";
        display: block;
        height: 2px;
        background-color: rgb(255, 255, 255);
        border-radius: 1px; 
        width: 80%; 
        margin: 20px auto;
    }

    .image-container {
        display: flex; 
        flex-direction: row; 
        justify-content: center; 
        gap: 20px; 
        margin-top: 20px;
    }

    .image-container img {
        max-width: 45%; 
        height: auto; 
        border-radius: 5px;
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

    .image-container {
            flex-direction: column; 
            align-items: center; 
        }

        .image-container img {
            max-width: 80%; 
            margin-bottom: 20px; 
        }
    
    
}
</style>

<div class="body">
<div class="header">
<h1>MailLobbyer</h1>
<h2>Jul 2023 - Aug 2024 | C#/HTML/CSS/JAVASCRIPT/RAZOR/ASP.NET
    CORE/ELECTRON.NET · GitHub - Open source </h2>
    <div class="buttons">
        <a href="https://github.com/sarahshamilton/MailLobbyer">
            <img src="{github}"/>
        </a>
    </div>
</div>
<div class="content-row">
    <h1>Project overview</h1>
    <p style="text-align: center;"> 
        Built with ASP.NET Core Blazor with an Electron.Net wrapper, MailLobbyer is a CSV-based emailing program with SMTP server integration. 
        Utilises CSV files with lists of contacts (First name, Surname, Email address, Prefix) and provides personalised emails and emailing lists 
        for batch email sending through the SMTP protocol.
    </p>
    <ul>
        <li>
            Demonstrated the ability to work through a Software Development Cycle in accordance with my client’s requirements through constant 
            communication and a UML design document, from the planning stage to the maintenance stage of the life-cycle.
        </li>
        <li>Cross-platform development, can be deployed to operating systems such as Windows, Linux, and MacOS.</li>
        <li>
            Implemented asynchronous programming and error handling to ensure the system is robust and has optimal performance.
        </li>
        <li>
            Utilised inline C# and HTML/CSS through the usage of Razor in ASP.Net Core, ensuring proper implementation of object-oriented programming 
            (OOP) principles, including encapsulation, inheritance, and abstraction.
        </li>
    </ul>
</div>
<div class="content-row">
    <h1>Project showcase</h1>
    <p style="text-align: center;"> 
        MailLobbyer is a client commissioned cross-platform tool for sending batch emails seamlessly through an SMTP server. Utilising CSV files containing recipient details, such as email addresses, full names, and prefixes, to dynamically personalise each email. Custom placeholders can be embedded within the subject line and body of the email in order to tailor the email to its recipient.
    </p>
    <p style="text-align: center;"> 
        The demonstration images below display:
    </p>
    <ul>
        <li>
            The main page where the user can input the email data, along with selection of a CSV emailing list. In addition the user selects a settings profile which contains the SMTP server information and the sender name and email address.
        </li>
        <li>
            The second stage of the main page allows exclusion of specific entries in the selected CSV emailing list.
        </li>
        <li>
            The settings profile page allows the user to input their sender details along with SMTP connection information such as Hostname and password.
        </li>
    </ul>
    <div class="separator"></div>
    <div class="image-container">
        <img src="{showcase0}"/>
        <img src="{showcase1}"/>
    </div>

</div>
</div>
