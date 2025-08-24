# PicBook Community Web App
A web platform for picture book enthusiasts to share, explore, and connect through illustrated stories. This project aims to promote engagement in the picture book community by providing a modern, interactive, and secure web experience.

# Project Overview
Objective:
* To build a picture book–themed community platform where users can:
  * Share and upload picture books.
  * Explore curated collections with category and search features.
  * Exchange ideas and reading experiences through interactive discussions.

# Features
* 🔑 User Management
  * Register, login, update profile
  * Delete account
  * Forgot password with email verification
* 📖 Picture Book Management
  * Upload, browse, and delete picture books
  * Built-in picture book viewer
* 🔍 Explore & Discover
  * Category & search filtering (by theme, year, author, language, etc.)
* 💬 Community Interaction
  * Comment section for sharing thoughts and experiences
  * Users can edit or delete their comments

# Installation:
## macOS:

#### Installing Node.js:

1. Download the rebuilt version of Node.js from [Node.js official website](https://nodejs.org/en/download/prebuilt-installer/current).

2. Follow the installation instructions provided for macOS.

#### Installing MySQL:

1. Download MySQL from the [official website](https://dev.mysql.com/downloads/installer/).

2. Follow the installation instructions provided for macOS.

3. Must download MYSQL from the version 8.0 or higher.

#### Configuring MySQL:

1. Navigate to MySQL bin directory:
   ```bash
   cd /usr/local/mysql/bin
   ```

2. Start the MySQL server:
   ```bash
   sudo /usr/local/mysql/support-files/mysql.server start
   ```

3. Execute setup script:
   ```bash
   ./mysql -u root -p < /path/to/directory/WebApp_Project/database/setup.sql
   ```

4. Execute initialization script:
   ```bash
   mysql -u root -p < \path\to\directory\WebApp_Project\database\init.sql
   ```

#### Setting up Node.js dependencies:

Navigate to the corresponding directory (e.g. `cd /path/to/directory/WebApp_Project/server`): 

##### In `server` directory:

Initialize npm and install required packages:
```bash
npm init -y
npm install express mysql2 multer bcryptjs jsonwebtoken dotenv sequelize cors nodemailer
```

#### Change the `DB_PASSWORD`:

Change the `DB_PASSWORD` in `/path/to/directory/WebApp_Project/server/.env` to your MySQL password.

#### Running the website:

Start the server:
```bash
node server.js
```



## Windows:

#### Installing Node.js:

1. Download the rebuilt version of Node.js from [Node.js official website](https://nodejs.org/en/download/prebuilt-installer/current).

2. Follow the installation instructions provided for Windows.

#### Installing MySQL:

1. Download MySQL from the [official website](https://dev.mysql.com/downloads/installer/).

2. Follow the installation instructions provided for Windows.

3. Must download MYSQL from the version 8.0 or higher.

#### Configuring MySQL:

1. Navigate to MySQL bin directory:
   ```bash
   cd "C:\Program Files\MySQL\MySQL Server X.X\bin"
   ```

2. Execute setup script:
   ```bash
   mysql -u root -p < \path\to\directory\WebApp_Project\database\setup.sql
   ```

3. Execute initialization script:
   ```bash
   mysql -u root -p < \path\to\directory\WebApp_Project\database\init.sql
   ```

#### Setting up Node.js dependencies:

Navigate to the corresponding directory (e.g. `cd \path\to\directory\WebApp_Project\server`): 

##### In `server` directory:

Initialize npm and install required packages:
```bash
npm init -y
npm install express mysql2 multer bcryptjs jsonwebtoken dotenv sequelize cors nodemailer
```

#### Change the `DB_PASSWORD`:

Change the `DB_PASSWORD` in `\your\path\to\directory\WebApp_Project\server\.env` to your MySQL password.

#### Running the website:

Start the server:
```bash
node server.js
```
