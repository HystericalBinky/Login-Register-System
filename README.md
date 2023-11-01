# Login-Register-System
## 📖Information
This Repository is a [Login/Register System](https://en.wikipedia.org/wiki/Login) that can be used for a [User](https://en.wikipedia.org/wiki/User_(computing)) to make an account. Made with [HTML](https://en.wikipedia.org/wiki/HTML), [CSS](https://en.wikipedia.org/wiki/HTML) and [PHP](https://en.wikipedia.org/wiki/PHP) in [Visual Studio Code](https://code.visualstudio.com/) using [XAMPP](https://sourceforge.net/projects/xampp/).

Login/Register System is an easy-to-use, [open-source](https://en.wikipedia.org/wiki/Open_source) [Website](https://en.wikipedia.org/wiki/Website) allowing you to easily login to your account or register a new one. It requires minimal setup to be used, only requiring you to have [Visual Studio Code](https://code.visualstudio.com/), [XAMPP](https://sourceforge.net/projects/xampp/) and optionally [Git](https://git-scm.com/) to easily [clone this project]().

## 🛡️Security
I have ran all the files through VirusTotal to ensure you that there are no viruses injected into this application. You can always run these files in the project through VirusTotal again if you wish.

In addition, your web browser might scan the file before downloading, and if you have an anti-virus on your computer, it will most likely also scan the files for viruses. They will 100% come out negative with a small chance of a false positive, it is recommended to use VirusTotal as your most trusted source. 

These regulations only apply for MY version, any modified versions from other people might contain viruses injected deliberetly.

## ⚙️Setup

### 📝Source Code/Visual Studio Code
1. Open Visual Studio Code
2. Clone the GitHub Repository
    * Select Clone Git Repository
    * Paste the following link in the Repository name: https://github.com/HystericalBinky/Conversion-System
    * Select the path as your XAMPP htdocs folder.
    * Click clone.
3. Open XAMPP and Run Services
    1. Open XAMPP as Administrator
    2. Run the Modules: Apache and MySQL
4. Create the Database
    1. Go to: http://localhost/phpmyadmin/
    2. Click the Databases tab at the top
    3. Under Create database, type in phplogin in the text box
    4. Select utf8_general_ci as the collation
    5. Click Create
    6. Click the database on the left side panel (phplogin) and execute the following 2 SQL statements:
       ```SQL
       CREATE TABLE IF NOT EXISTS `accounts` (
	        `id` int(11) NOT NULL AUTO_INCREMENT,
  	      `username` varchar(50) NOT NULL,
  	      `password` varchar(255) NOT NULL,
  	      `email` varchar(100) NOT NULL,
          PRIMARY KEY (`id`)
        ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;
       ```

       ```SQL
       ALTER TABLE accounts ADD activation_code varchar(50) DEFAULT ''
       ```
5. Go to: http://localhost/phplogin/ and test it!
