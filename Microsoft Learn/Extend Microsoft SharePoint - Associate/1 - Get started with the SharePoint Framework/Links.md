# Course: Get started with the SharePoint Framework

<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/">Course Link</a>

<a href="https://www.youtube.com/watch?v=_Pt5cnU4MpU&list=PLR9nK3mnD-OV-RPXQ3Lco845qoEy7VJoc">Youtube Video</a>

## 1 - Introduction
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/1-introduction">Module Link</a>

## 2 - Overview of SharePoint Framework
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/2-sharepoint-framework-overview">Module Link</a>

## 3 - Create and configure your SharePoint Online developer tenant
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/3-exercise-configure-tenant">Module Link</a>

1. Where can SharePoint Framework client-side web parts be used?

    <strong>Modern pages in SharePoint Online and SharePoint Server 2019

    Classic pages in SharePoint Online, SharePoint Server 2019, and SharePoint Server 2016.

    Publishing pages in SharePoint Online, SharePoint Server 2019, and SharePoint Server 2016.</strong>

2. In order to deploy and test SharePoint Framework components, what must you first do in your SharePoint tenant?

    <strong>Create an app catalog site from the SharePoint Online admin center (or Central Administration site if on-premises).</strong>


## 4 - SharePoint Framework Environment
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/4-spfx-development-environment">Module Link</a>

<ul>
    <li>Build Process and Tooling
        <ul>
            <li>Yeoman is used to replace the new project experience that traditional server-side SharePoint developers are familiar with in Visual Studio.</li>
            <li>Gulp is a task runner that replaces the tool MSBuild used in .NET solutions. This is used to run various tasks, like transpiling TypeScript to JavaScript, creating JavaScript bundles and SharePoint packages.</li>
            <li>Node.js is the underlying runtime used by all applications. The tools we're covering in this section are all built on top of Node.js. Node.js is required to run them, just like the .NET Framework is required to run .NET apps.</li>
            <li>NPM is used as the package manager and you'll use it to install global tools and reusable code in your projects.</li>
            <li>Webpack is used to combine all the JavaScript and CSS files in your project into a single JavaScript bundle. Bundles are the recommended way to deploy client-side applications for performance reasons.</li>
        </ul>
    </li>
    <li>Web Frameworks
        <ul>
            <li>When building client-side applications, developers commonly use web frameworks. The SharePoint Framework doesn't limit you to any specific framework. You can use any of the popular web frameworks in your projects including React, Angular, Knockout, or Vue.js. You can even use the popular jQuery library in your custom apps.</li>
        </ul>
    </li>
    <li>Code Editor
        <ul>
            <li>Visual Studio Code</li>
        </ul>
    </li>
</ul>

## 5 - Configure your SharePoint Framework Development Environment
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/5-exercise-setup-development-environment">Module Link</a>
<ul>
    <li>Check Node Version: <strong>node -v</strong></li>
    <li>Install Yeoman: <strong>npm install --g yo</strong></li>
    <li>Install SharePoint Framework Yeoman generator: <strong>npm install --g @microsoft/generator-sharepoint</strong></li>
    <li>Install Gulp: <strong>npm install --g gulp</strong></li>
</ul>

1. What are the minimum tools you must install in your development environment to build SharePoint Framework components?

    <strong>Node.js, Gulp, Yeoman, and the Yeoman generator for the SharePoint Framework.</strong>

2. What purpose does Gulp serve in the build toolchain?

    <strong>Its used to run common build and development tasks, such as compiling the project and creating the deployment package.</strong>

## 6 - Interact with SharePoint Framework web parts on modern pages
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/6-interact-spfx-web-parts">Module Link</a>

## 7 - Exercise - Interact with SPFx client-side web parts in modern sites
<a href="https://docs.microsoft.com/en-us/learn/modules/sharepoint-spfx-get-started/7-exercise-client-side-web-parts">Module Link</a>

Run the SharePoint Yeoman generator by executing the following command:

yo @microsoft/sharepoint
Use the following to complete the prompt that is displayed:

What is your solution name?: HelloWorld
Which baseline packages do you want to target for your component(s)?: SharePoint Online only (latest)
Where do you want to place the files?: Use the current folder
Do you want to allow the tenant admin the choice of being able to deploy the solution to all sites immediately without running any feature deployment or adding apps in sites?: No
Will the components in the solution require permissions to access web APIs that are unique and not shared with other components in the tenant?: No
Which type of client-side component to create?: WebPart
What is your Web part name?: HelloWorld
What is your Web part description?: HelloWorld description
Which framework would you like to use?: No JavaScript framework

When NPM completes downloading all dependencies, install the developer certificate by executing the following command:

gulp trust-dev-cert

Run the project by executing the following command:

gulp serve

Close the browser and stop the local web server by pressing CTRL+C in the command prompt.

1. What purpose does Yeoman serve in the build toolchain?

    <strong>Its used to scaffold new projects after answering a few questions about the project.</strong>

2. What purpose does the Yeoman generator serve in the build toolchain?

    <strong>Its executed by Yeoman and used to scaffold new projects after answering a few questions about the project.</strong>