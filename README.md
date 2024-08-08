# Ghost CMS Setup and Management

This guide covers the installation of Ghost CMS, starting the server, uploading a new theme, and restoring a backup.

## Prerequisites

- Node.js (v12.10.0 or later)
- npm (v6.0.0 or later)
- A supported version of Ghost CLI

## Installation

1. **Install Ghost CLI globally:**

   ```bash
   npm install -g ghost-cli
   ```

2. **Create a new directory for your Ghost installation and navigate into it:**

   ```bash
   mkdir my-ghost-blog
   cd my-ghost-blog
   ```

3. **Install Ghost:**

   ```bash
   ghost install local
   ```

## Starting Ghost

1. **Start Ghost:**

   ```bash
   ghost start
   ```

2. **Check Ghost status:**

   ```bash
   ghost ls
   ```

   You should see your Ghost instance running.

## Uploading a New Theme

3. **Upload the theme via the Ghost Admin:**

   - Navigate to `http://your-ghost-blog.com/ghost`.
   - Log in with your admin credentials.
   - Go to `Design` -> `Themes` -> `Upload a Theme`.
   - Zip all theme files with `npm run zip`, and upload it.
   - Activate the theme once it's uploaded.

## Restoring  Backup Settings

1. **Access the Ghost Admin:**

   - Navigate to `http://your-ghost-blog.com/ghost`.
   - Log in with your admin credentials.

2. **Navigate to the Imports section:**

   - Go to `Dashboard` -> `Settings` -> `Import/Export` -> `Migration Tools` -> `Import`.

3. **Import your backup:**

   - In the `Import Export` section, find the `Import` section.
   - Choose your backup file (usually a `.json` file,uploaded in `settings_backup folder`) and upload it.
   - Follow the prompts to complete the restoration.

4. **Copy image assets:**

   - Copy And Paste all `images` from images folder to `\content\images`.

   ```

   ```

## Conclusion

You now have a basic setup for managing a Ghost CMS instance, including installation, starting the server, uploading themes, and restoring backups. For more detailed information, visit the [official Ghost documentation](https://ghost.org/docs/).
