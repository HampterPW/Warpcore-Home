<script>
import { onMount } from "svelte";

// Components
import NavigationBar from "$lib/NavigationBar/NavigationBar.svelte";
import NavigationMargin from "$lib/NavigationBar/NavMargin.svelte";
// translations
import LocalizedText from "$lib/LocalizedText/Node.svelte";
import Language from "../../resources/language.js";

// Static values
import LINK from "../../resources/urls.js";

let currentLang = "en";
onMount(() => {
    Language.forceUpdate();
});
Language.onChange((lang) => {
    currentLang = lang;
});
</script>

<svelte:head>
    <title>PenguinMod - Privacy Policy</title>
    <meta name="title" content="PenguinMod - Privacy Policy" />
    <meta property="og:title" content="PenguinMod - Privacy Policy" />
    <meta property="twitter:title" content="PenguinMod - Privacy Policy">
    <meta name="description" content="The status of your privacy while using PenguinMod.">
    <meta property="twitter:description" content="The status of your privacy while using PenguinMod.">
    <meta property="og:url" content="https://penguinmod.com/privacy">
    <meta property="twitter:url" content="https://penguinmod.com/privacy">
</svelte:head>

<NavigationBar />

<div class="main">
    <NavigationMargin />

    <div class="section-info">
        <h1>Privacy Policy</h1>
    </div>

    <main>
        <!-- UPDATE THIS WHEN MAKING CONTENT CHANGES -->
        <p><i>Updated January 13th, 2024 (Mountain Time)</i></p>

        <!-- some things are intentionally not formatted as they are in the HTML file on the website -->
        <p>
            This document applies to
            <a href="https://penguinmod.com">https://penguinmod.com</a>,
            <a href="https://studio.penguinmod.com">https://studio.penguinmod.com</a>,
            <a href="https://extensions.penguinmod.com">https://extensions.penguinmod.com</a>,
            <a href="https://projects.penguinmod.com">https://projects.penguinmod.com</a>,
            and any other penguinmod.com subdomains.
        </p>
        <p>
            You may see websites such as <a href="https://scratch.mit.edu/">"Scratch"</a>,
            <a href="https://turbowarp.org/">"TurboWarp"</a>, and <a href="https://auth.itinerary.eu.org/">"Scratch Auth"</a>
            referenced in multiple places.
        </p>
        <p>
            A "Service Administrator", "Admin", "Moderator", "Mod" or "Administrator" is a person who can either
            directly access the server files for PenguinMod,
            or a person who can contact the server host that is able to access the server files and server process.
            "Host" may also refer to the server host of PenguinMod's project sharing.
        </p>
        <p>
            A "Project Moderator" is a person who has the ability to remove projects or content from those projects,
            and reply or send messages to users who had moderation actions happen towards their project or account.
            These users may also be able to edit profile information about another user.
            <br><br>
            These people can contact Administrators aswell, and may have extra permissions such as banning users.
        </p>

        <h2>General</h2>
        <p>
            We may log anonymous aggregated data such as
                how many people use the site,
                how often a feature is used,
                what operating system and browser is used,
                how much user content is on the site,
                and diagnostic information such as cache hit ratios.
        </p>
        <p>
            When using the website, your IP will be logged and stored to your account's name if you log in.
            This is to help us identify users who may be spamming or attacking the site.
            <br>
            Your IP will also be stored temporarily when viewing a project, along with information about the project you viewed being logged temporarily.
            <br>
            <br>
            This temporary amount of time will be around 1 week, and this applies to all "temporarily stored" content listed here.
        </p>

        <h2>Advertisments</h2>
        <p>
            When advertisements are served on any PenguinMod page, third parties may be placing and reading cookies on your browser,
            or using web beacons to collect information. PenguinMod itself does not do this, and you may be able to find more information here:
        </p>
        <ul>
            <li><a href="https://support.google.com/publisherpolicies/answer/10437794">What we must disclose in our privacy policy</a></li>
            <li><a href="http://www.google.com/policies/privacy/partners/">How Google uses data when you use our partners' sites or apps</a></li>
        </ul>
        
        <h2>Project Sharing & Accounts/Profiles</h2>
        <p>
            Accounts are logged into using <a href="https://auth.itinerary.eu.org/">Scratch Auth</a>,
            which requires you to have a <a href="https://scratch.mit.edu/">Scratch</a> account.
        </p>
        <p>When you use Scratch Auth, it can access:</p>
            <ul>
                <li>your IP address</li>
                <li>your general location (using your IP address)</li>
                <li>your public <a href="https://scratch.mit.edu/">Scratch</a> Account information</li>
            </ul>
        <p>
            Accounts do not actually exist on PenguinMod, but instead PenguinMod stores data that is attached to a certain username.
            When you "log-in" to an account, you are actually only gaining access to perform actions to data that is attached to a certain username,
            or create data to be attached to your username.
        </p>
        <p>
            When using our Services:
        </p>
        <ul>
            <li>any projects uploaded will have their project name logged</li>
            <li>any projects uploaded are publicly viewable (including unapproved projects if you have the URL to them)</li>
            <li>any profile info you set (bio/about me, featured project) is publicly viewable to all users, unless stated otherwise</li>
            <li>any projects uploaded can be modified by admins or hosts of the service in any way (project image, project name, project code, etc.)</li>
            <li>any profile info you set can be modified by admins or hosts of the service in any way (profile about me, etc.)</li>
        </ul>
        <p>
            Uploaded projects will be publicly visible to all users on the website.
            Any user may report a project or report another user to Project Moderators if they believe the <a href="https://penguinmod.com/guidelines/uploading">Uploading Guidelines</a> have been violated.
        </p>
            Project Information available to users, Project Moderators and Service Administrators include:
            <ul>
                <li>the project name, project instructions & notes, project thumbnail, project data, uploader's name, uploader's <a href="https://scratch.mit.edu/">Scratch</a> account and uploader's profile picture for any project</li>
                <li>the date any project was uploaded, updated or featured</li>
                <li>the likes, votes, favorites and views attached to that project</li>
                <li>whether or not the project has been updated</li>
                <li>any other internal information about the project</li>
            </ul>
            Information available only to Project Moderators and Service Administrators include:
            <ul>
                <li>the date a project was removed</li>
                <li>the date, contents, and type of any moderator message or response to a moderator message</li>
                <li>any above information users can access</li>
            </ul>
            Information available only to Service Administrators include:
            <ul>
                <li>the indiviudal users who liked, favorited or voted a project</li>
                <li>the IP of users who viewed a project (until server reset)
                <li>any above information users or Project Moderators can access</li>
            </ul>
        <p>
            Your IP will temporarily be saved in the server when you view a project.
            This is used to make sure you are not the same user reloading the page to gain multiple views.
        </p>
        <p>Account Usernames are saved in the server when that user liked, favorited or "voted to feature" a project.</p>
        <p>
            Account Usernames and project info will also be logged when a project is liked, favorited or voted for.
            This is for debugging purposes for the developers.
        </p>
        
        <h2>Other services</h2>
        <p>When using cloud variables, the project ID and your username may be logged for up to 14 days.</p>
        <p>Your randomly generated or chosen username is stored in your browser's local storage. To mitigate the potential to track users with this feature, all randomly generated usernames are anonymized before the server receives them. However, usernames explicitly set by a user may be logged to help prevent abuse.</p>
        <p>Built-in Scratch extensions that require Wi-Fi (such as Translate, Text to Speech, LEGO, micro:bit, etc.) may connect to the Scratch API to implement these features. <a href="https://scratch.mit.edu/privacy_policy/">Refer to the Scratch privacy policy for more information</a>. The Translate extension may instead make requests to a TurboWarp API, which may then forward your request to the Scratch API and log the message being translated and the result for caching and performance.</p>
        <p>In rare circumstances, connections that are appear to be spam may have their IP logged for up to 24 hours. This happens very infrequently and only in cases of extreme abuse.</p>
        <p>
            Built-in PenguinMod and Custom extensions that require Wi-Fi or use Wi-Fi to get online data (HTTP, Website Requests, Extended Audio, CloudLink, HTML iframes, Storage, etc.) may connect to any user-specified API, which will grant the owner of the website being connected to:
        </p>
        <ul>
            <li>your full IP address (and possibly general location using your IP address)</li>
            <li>the ability to show or display anything (if the extension is showing the info returned to the user)</li>
            <li>any other things public APIs can do or access</li>
        </ul>
        <p>This document does not apply to third-parties, including other users or bots connected to cloud variables, links to external websites, custom extensions, or some advanced URL parameters.</p>

        <h2>Editor extensions</h2>
        <h4>Core - HTML iframes (referred to as "iframes" here)</h4>
        <p>
            "iframes" may connect to user-specified websites. These websites may be allowed to access:
        </p>
            <ul>
                <li>your IP address</li>
                <li>your general location (using your IP address)</li>
                <li>any web API</li>
            </ul>
        <p>
            The websites specified may also display any content, however PenguinMod will attempt to automatically scan the website
            for any potential viruses or vulnerabilities. Major adult websites are also blocked, and most others are blocked aswell.
        </p>
        <p>
            PenguinMod does not allow projects uploaded to only display content from other websites.
            Uploaded projects must contain content of their own, and certain websites may cause the uploaded project to be deleted or rejected.
        </p>
        <h4>Core - Scratch Authentication (referred to as "Scratch Auth Extension" here)</h4>
        <p>
            The "Scratch Auth Extension" will connect to <a href="https://auth.itinerary.eu.org/">Scratch Auth</a> for Log-In. Scratch Auth can access:
            </p>
            <ul>
                <li>your IP address</li>
                <li>your general location (using your IP address)</li>
                <li>your public <a href="https://scratch.mit.edu/">Scratch</a> Account information</li>
            </ul>
            <p>
            The "Scratch Auth Extension" also allows your public Scratch account information to be accessible to the PenguinMod project,
            however other tools, extensions or APIs are required to get information past your Scratch username.
        </p>
        <h4>User-submitted (G1nX) - Better Storage</h4>
        <p>
            Better Storage will connect to <a href="https://auth.itinerary.eu.org/">Scratch Auth</a> for Log-In. Scratch Auth can access:</p>
            <ul>
                <li>your IP address</li>
                <li>your general location (using your IP address)</li>
                <li>your public <a href="https://scratch.mit.edu/">Scratch</a> Account information</li>
            </ul>
            <p>
            Better Storage can also access any info that Scratch Auth can.
            The owner of Better Storage may also view any saved data using their keys for security and safety.
        </p>
        <h4>User-submitted (RubyDevs) - TurboWeather</h4>
        <p>
            TurboWeather uses Browser APIs to geolocate the user.
            <br>
            PenguinMod will ask the user to confirm this action before the extension attempts to do this.
            <br>
            <br>
            PenguinMod will not ask the user to confirm this action if the project is compiled using
            <a href="https://studio.penguinmod.com/PenguinMod-Packager/">the PenguinMod packager.</a>
            <br>
            In this case it is up to the user's browser to prompt the user if they would like to allow the website
            to access their location.
        </p>
        <p>
            The Ruby Developer team promises that they do not store or keep your location data in any way when using the extension.
            <br>
            TurboWeather does however connect to third-party services to get user information that may store your info:
        </p>
        <ul>
            <li><a href="https://open-meteo.com/en/terms">OpenMeteo - Terms of Service</a></li>
            <li><a href="https://osmfoundation.org/wiki/Privacy_Policy">OpenStreetMap - Privacy Policy</a></li>
        </ul>
        <p>
            When using the extension, third-party services may be able to access:</p>
            <ul>
                <li>your IP address</li>
                <li>your general location</li>
                <li>info about your location (weather, temperature)</li>
            </ul>
            <p>
            TurboWeather does make efforts to avoid returning private info, such as:
        </p>
        <ul>
            <li>latitude and longitude</li>
            <li>specifically chosen or user coordinates (provided for geolocation)</li>
            <li>any other info returned by the third-party services that may be used to find the user in real life</li>
        </ul>

        <h2>Contact</h2>

        <p>Email us at <a href="mailto:penguinmodhelp@gmail.com">penguinmodhelp@gmail.com</a></p>
        <p>Join <a href="https://discord.gg/NZ9MBMYTZh">our Discord Server</a></p>
    </main>
</div>

<style>
    * {
        font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    }

    .main {
        position: absolute;
        left: 0px;
        top: 0px;
        width: 100%;
        min-width: 1000px;
    }

    main {
        margin: 0 20%;
        width: 60%;
    }

    .small {
        font-size: 12px;
    }

    .detail-card {
        width: calc(100% - 24px);
        padding: 48px 12px;
        background: dodgerblue;
        color: white;
        text-align: center;
    }
    .detail-card p,
    .detail-card h1 {
        margin-block: 0;
    }
    .detail-card h1 {
        font-size: 48px;
    }

    .section-info {
        background: #00c3ffad;
        height: 12rem;
        color: white;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        width: 100%;
        margin: 0;
    }
    .section-info h1 {
        margin-block: 0;
        margin-left: 32px;
    }
    .section-info p {
        margin-block-end: 0;
        margin-left: 32px;
    }

    :global(body.dark-mode) a {
        color: dodgerblue;
    }
</style>
