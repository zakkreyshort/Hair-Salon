# _Hair Salon!_

#### _MySQL & Entity Framework Core week 4 independent project for Epicodus_
#### _20 March 2020_

#### By _**Zakkrey Short**_

## Description

_This application will create a website where users can add stylists and keep track of their client details._

## Specifications: 

| Specification | Example Input | Example Output |
| ------------- |:-------------:| -------------------:|
| Application creates instance of an stylist object | stylist newstylist = new stylist(name, details) | new stylist object created |
| Application saves all new stylists in database table named stylists | new stylist object instantiated | new stylist object saved as row in database table |
| If user visits '/' root route, applications displays splash page with link to '/stylists' | user visits '/' route | displays homepage |
| If user visits '/stylists' route, applications displays all stylists in database, each with a link to view more details about the stylist and ordered alphabetically by type | user visits '/stylists' route | displays list of stylists |
| If user clicks "add new stylist" button, application redirects to new stylist form | user clicks "add new stylist" button | application redirects to new stylist form |
| If user visits '/stylists/new', application shows new stylist form | user visits '/stylists/new' | application displays form for adding new stylist |
| If user visits submits new stylist form, application adds new stylist to database and redirects to '/stylists' | user submits form | application adds new stylist to database and redirects to page showing all stylists in database |
| If user visits '/stylists/{id}', application displays details for that stylist | user clicks on specific stylist in stylists list | application redirects to display details about that stylist |

## Setup/Installation Requirements

### Install .NET Core

#### on macOS:
* _[Click here](https://dotnet.microsoft.com/download/thank-you/dotnet-sdk-2.2.106-macos-x64-installer) to download a .NET Core SDK from Microsoft Corp._
* _Open the file (this will launch an installer which will walk you through installation steps. Use the default settings the installer suggests.)_

#### on Windows:
* _[Click here](https://dotnet.microsoft.com/download/thank-you/dotnet-sdk-2.2.203-windows-x64-installer) to download the 64-bit .NET Core SDK from Microsoft Corp._
* _Open the .exe file and follow the steps provided by the installer for your OS._

#### Install dotnet script
_Enter the command ``dotnet tool install -g dotnet-script`` in Terminal (macOS) or PowerShell (Windows)._

### Clone this repository

_Enter the following commands in Terminal (macOS) or PowerShell (Windows):_
* ``cd desktop``
* ``git clone`` followed by the URL to this repository
* ``cd HairSalon``

_Confirm that you have navigated to the HairSalon directory (e.g., by entering the command_ ``pwd`` _in Terminal)._


_Build the database ``zakkrey_short`` using MySQL either manually, or through these MySQL commands in terminal/powershell:_

* _CREATE DATABASE zakkrey_short_;
* _Use zakkrey_short_;
* _CREATE TABLE stylists (StylistId INT NOT NULL AUTO_INCREMENT, Name VARCHAR(255) NULL, Details VARCHAR(255) NUll, PRIMARY KEY (StylistId));
* _CREATE TABLE clients (ClientId INT NOT NULL AUTO_INCREMENT, Name VARCHAR(255) NULL, StylistId INT NULL DEFAULT 0, PRIMARY KEY (ClientId));_


_Run this application by entering the following command in Terminal (macOS) or PowerShell (Windows):_
* ``cd HairSalon``
* ``dotnet restore``
* ``dotnet build``
* ``dotnet run`` or ``dotnet watch run``

_To view/edit the source code of this application, open the contents of this directory in a text editor or IDE of your choice (e.g., to open all contents of the directory in Visual Studio Code on macOS, enter the command_ ``code .`` _in Terminal)._


## Technologies Used
* _Git_
* _VSCode_
* _C#_
* _HTML_
* _Razor_
* _.NET Core 2.2_
* _ASP.NET Core MVC 2.2_
* _dotnet script_
* _MySQL_
* _MySQL Workbench_
* _Entity Framework Core 2.2_ 

### License

*This webpage is licensed under the MIT license.*

Copyright (c) 2020 **_Zakkrey Short_**