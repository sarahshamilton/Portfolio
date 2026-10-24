<script>
    import '@fontsource-variable/source-code-pro';
    import '@fontsource/gugi';

    import github from '$lib/assets/icons/github.svg';

    import showcase0 from '$lib/assets/projects/laserIs/1.png';
    import showcase1 from '$lib/assets/projects/laserIs/2.png';

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
        padding: 20px;
        margin: 10px auto;
    }

    .buttons img {
        filter: invert(1);
        height: 10vh;
        color: #ffffff;
        border: none;
        transition: all 0.3s ease;
        cursor: pointer;
        margin: 0 10px;
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
        margin: 20px auto;
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
        <h1>LASER Inventory System (LASERIS)</h1>
        <h2>Dec 2024 - Present | C# · SQLite · ASP.NET Core · GitHub - Open source</h2>
        <div class="buttons">
            <a href="https://github.com/sarahshamilton/LASERIs">
                <img src="{github}" />
            </a>
            <a href="https://github.com/sarahshamilton/LASERIsAPI">
                <img src="{github}" />
            </a>
        </div>
    </div>
    <div class="content-row">
        <h1>Project overview</h1>
        <p style="text-align: center;">
            Worked on developing and deploying a lab inventory system to facilitate tracking part numbers, quantities and what items teams have borrowed.
        </p>
        <ul>
            <li>This project consisted of two components:</li>
            <li><strong>LASERIS</strong> – Front-end UI written in C# with AvaloniaUI, designed with the MVVM design pattern to ensure clean separation of UI from logic.</li>
            <li><strong>LASERISAPI</strong> – Web API written in C# ASP.NET Core, provides appropriate endpoints for HTTP request methods for the front-end and allows access and storage to a relational SQLite database.</li>
        </ul>
    </div>
    <div class="content-row">
    <h1>Project showcase</h1>
    <p style="text-align: center;"> 
        The demonstration images below display:
    </p>
    <ul>
        <li>
            The main page where the user can input and search through the lab's database for specific parts using filters, along with displaying a table of queried parts which the user can make direct updates to attributes on entries. The "Entry Add/Remove" page allows for removal and additions of part as required on the back-end database.
        </li>
        <li>
            The Swagger UI displays the data model for each database part entry. SQLite is accessed via a WebAPI that supports the front-end application.
        </li>
    </ul>
    <div class="separator"></div>
    <div class="image-container">
        <img src="{showcase1}"/>
        <img src="{showcase0}"/>
    </div>
    </div>
</div>
