# Quran Viewer: Ayah-wise Display with Translation

## Overview

This project is a simple Quran viewer that displays each **ayah** (verse) of a surah along with its translation. It uses **HTML**, **CSS**, and **JavaScript (MVC architecture)** for displaying Quranic verses dynamically, along with API integration for fetching surah data, translations.

---

## Features

- **Surah Selection**: Select a surah from the dropdown menu.
- **Ayah Display**: Each ayah is displayed with its **Arabic text**, **translation**.
- **Responsive Design**: The app is responsive and works well on both desktop and mobile devices.
- **MVC Architecture**: The app is structured using the **Model-View-Controller (MVC)** design pattern for better code organization and maintainability.
  
---

## Technologies Used

- **HTML5**: Markup language for the structure of the web page.
- **CSS3**: For styling the webpage and making it visually appealing.
- **JavaScript**: For handling logic and interactions (using MVC architecture).
- **API**: Fetching surah data from a public API for Quranic verses.

---

## Project Structure

```plaintext
quran-app/
├── css/
│   └── style.css             # Stylesheet for the app
├── js/
│   ├── model.js              # Model: Fetches surah data
│   ├── view.js               # View: Renders surah content to the UI
│   └── controller.js         # Controller: Handles the app's logic and user interaction
├── index.html                # Main HTML file to load the app
```

---

## How to Run the Project Locally

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge).
- An internet connection (for fetching the surah data from the API).

### Steps to Run

1. **Clone or Download the Project**

   - If you are using Git, clone the repository:
     ```bash
     git clone https://github.com/your-username/quran-viewer.git
     ```

2. **Navigate to the Project Directory**

   Open the project folder on your local machine.

3. **Open `index.html` in Your Browser**

   Simply double-click on `index.html` or open it in your browser using the `file://` protocol.

   You should now see the Quran viewer in your browser, and you can interact with it.

---

## How It Works

1. **Model (data layer)**: The **model** fetches data from the API, including each surah's verses, translations.
   
2. **View (presentation layer)**: The **view** renders the surah's verses on the webpage, including each verse's Arabic text, translation.

3. **Controller (logic layer)**: The **controller** connects the model and view, processing the data and handling interactions such as selecting a surah and dynamically updating the page with the appropriate verses.

---

## Features in Detail

### 1. **Surah Selection**

   - The user can select a surah from the dropdown menu, and the page will update to show the corresponding verses of the selected surah.

### 2. **Displaying Each Ayah**

   - For each ayah, the Arabic text is displayed, along with a translation (in English).

---

## Example Surah Data

Each surah in the app displays:

- **Arabic text of the verse**.
- **Translation** of the verse (you can change or update the translation source).

Here’s a sample of how an ayah would appear in the app:

```
Verse 1: 
بِسْمِ اللَّهِ الرَّحْمَٰنِ الرَّحِيمِ
Translation: In the name of Allah, the Most Gracious, the Most Merciful.
```

---

## API Used

This app fetches the Quranic data (Arabic text, translation) from the public **Al-Quran API**. The endpoint used is:

```
https://api.alquran.cloud/v1/surah/{surahNumber}
```

Where `{surahNumber}` is the numeric ID of the surah (e.g., 1 for Al-Fatiha, 2 for Al-Baqarah, etc.).

---

## Future Enhancements

- Add **search functionality** for verses or surahs.
- Add **multiple translations** for each ayah.
- Implement **dark mode** for the UI.
- Add **bookmarking** feature to save favorite verses.

---

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit pull requests. Please make sure to follow the standard Git commit conventions.

---

## Acknowledgements

- Thanks to the **Al-Quran API** for providing free access to Quranic data.
---
