# Academic Workshop Poster Template (HTML/CSS)

This is a responsive HTML/CSS template designed for creating a professional A3 Landscape academic workshop or conference poster. It's structured as a clean, two-column layout that is easy to edit and print-ready.

## Features

  * **A3 Landscape Format:** Designed for the standard large-format poster size.
  * **Two-Column Layout:** A common, easy-to-read layout with a distinct sidebar for key info and a main area for content.
  * **Print-Ready:** When exported correctly, this produces a high-quality PDF ready for printing.
  * **Self-Contained:** All styles are embedded in the HTML file, so you only need to manage one file (plus your images).
  * **Easy to Edit:** No complex frameworks; just plain HTML.

-----

## 🚀 How to Use

Follow these three steps to create your poster.

### Step 1: Download and Prepare

1.  Save the HTML file as `index.html`.
2.  Create a folder for your poster.
3.  Place the `index.html` file inside this folder.
4.  Create an `images` subfolder (or just put all your images in the same folder) to hold your headshots, logos, and QR code.

### Step 2: Edit the HTML Content

Open the `index.html` file in any code editor (like Visual Studio Code, Sublime Text, or even a basic text editor like Notepad). Find the sections below and replace the placeholder content with your own.

#### 1\. Page Title

This is what appears in the browser tab.

```html
<head>
    ...
    <title>YOUR WORKSHOP TITLE HERE</title>
    ...
</head>
```

#### 2\. Left Column (Blue Sidebar)

**Main Title & Logo:**

  * `<h1>`: Your main workshop title.
  * `.logo-badge img`: Your conference or university logo.
  * `.subtitle`: The workshop's subtitle or theme.

<!-- end list -->

```html
<div class="title-container"> 
    <h1>4th Workshop on Intelligent Vehicle Meets Urban</h1>
    <div class="logo-badge">
        <img src="ITSClogo.png" alt="ITSC 2025 Logo" class="header-logo">
    </div>
</div>
<p class="subtitle">Safe And Certifiable Navigation...</p>
```

**Event Details & QR Code:**
Update the date, website, venue, and Zoom info. Most importantly, update the `img.dth-qr` to point to your own QR code image.

```html
<div class="date-time-highlight">
    <div class="dth-text">
        <b>Date:</b> Tuesday, 18 November 2025...<br>
        <b>Website:</b> [https://your-website.com](https://your-website.com)<br>
        <b>Venue:</b> Your Venue Here<br>
        <b>Zoom Webinar:</b> 123 4567 8901 <b> Code:</b> 123456 <br>
    </div>
    <img class="dth-qr" src="my_qr_code.png" alt="QR code">
</div>
```

**Workshop Overview:**
Edit the text inside the `<p>` tags.

```html
<h2>Workshop Overview</h2>
<p class="overview-text text-justify">
    Your overview text goes here...
</p>
```

**Organizing Committee:**
There is one card for the "Host" and a grid for other organizers. To add/remove organizers, copy/paste one of the `.organizer-card` blocks.

```html
<div class="organizer-host-card">
    <img src="headshot_host.png" alt="Host: Prof. Name">
    <div>
        <p class="role">Host</p>
        <p class="name">Prof. Your Name</p>
        <p>Your University</p>
    </div>
</div>

<div class="organizer-grid">
    <div class="organizer-card" role="listitem">
        <img src="headshot_person1.png" alt="Dr. Person One">
        <p class="name">Dr. Person One</p>
        <p class="affil">Affiliation</p>
    </div>
    </div>
```

#### 3\. Right Column (White Content Area)

**Invited Speakers:**
To add/remove speakers, copy/paste one of the `.speaker-card` blocks.

```html
<div class="speaker-grid">
    <div class="speaker-card">
        <img src="speaker_headshot.png" alt="Prof. Speaker Name">
        <p class="name">Prof. Speaker Name</p>
        <p class="affiliation">Speaker University</p>
    </div>
    </div>
```

**Program / Agenda:**
Edit the `<tbody>` section of the table. Each `<tr>` is a new row.

```html
<table class="agenda-table">
T    <thead>...</thead>
    <tbody>
        <tr>
            <td>08:30-09:00</td>
            <td>Prof. Li-Ta Hsu**</td>
            <td>Urban GNSS RTK/INS Integrated System...</td>
T        </tr>
        <tr>
            <td>10:00-10:30</td>
            <td></td>
            <td class="session-title" colspan="2">Short Break</td>
        </tr>
    </tbody>
</table>
```

**Contact Info:**
Update the contact person and email at the very bottom.

```html
<div class="contact-info">
    <b>Contact:</b> Dr. Your Name | your.email@connect.polyu.hk
</div>
```

### Step 3: Export to PDF

The easiest way to get a high-quality PDF is to print from your web browser.

1.  **Open the File:** Open your saved `index.html` file in a browser (like Google Chrome, Firefox, or Microsoft Edge).
2.  **Open Print Dialog:** Press `Ctrl+P` (Windows/Linux) or `Cmd+P` (Mac).
3.  **Set PDF Options:**
      * **Destination:** `Save as PDF`
      * **Layout:** `Landscape`
      * **Paper size:** `A3`
      * **Margins:** `None` (or "Minimum" if "None" is not available).
      * **IMPORTANT:** Click on **"More settings"** and ensure that **"Background graphics"** is **CHECKED**. If you don't, the blue sidebar will be white.
4.  **Save:** Click "Save" and choose a name for your PDF file.

You now have a high-resolution, print-ready PDF of your poster\!

-----

## 🎨 Advanced Customization (Optional)

All colors, fonts, and layout styles are defined in the `<style>...</style>` block in the `<head>` of the HTML file.

You can change the main theme colors by finding and replacing these values in the CSS:

  * **Dark Blue:** `#003366`
  * **Medium Blue:** `#023e8a`
  * **Lighter Blue:** `#0077b6`
  * **Highlight Cyan:** `#0096c7`

-----

## Acknowledgements

Special thanks to **Dr. Haoming Zhang**, **Dr. Feng Huang**, and **Prof. Weisong Wen** for their contributions to this template.

For any questions or issues, please contact **Yixin Gao**.
