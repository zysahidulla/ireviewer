# iReviewer

iReviewer is a browser-based study and quiz platform for practicing technical, science, history, gaming, and other subjects. It supports configurable review sessions, custom question decks, PDF-based study materials, and multiple visual themes.

## Features

- Classic Review mode with configurable question counts
- Sudden Death mode that ends after the first incorrect answer
- 60s Speedrun mode with a global countdown
- Curated question categories and randomized question order
- Optional per-question timer
- 50:50, Freeze, and Skip assists
- PDF import with extracted notes, flashcards, and generated quiz questions
- Custom deck editor with JSON import and export support
- Results summary, answer review, streak tracking, and achievements
- Animo Dark, Pure OLED, Emerald Glow, and Animo Light themes
- Optional synthesized audio feedback

## Requirements

- A modern web browser with JavaScript enabled
- Internet access for the Tailwind CSS CDN, PDF.js, and Google Fonts

No PHP server, database, Composer installation, or build step is required.

## Getting Started

1. Clone or download this repository.

   ```bash
   git clone <repository-url>
   cd iReviewer
   ```

2. Open `index.html` directly in a browser.

   A local web server is recommended for the most consistent browser behavior:

   ```bash
   python -m http.server 8000
   ```

3. Visit [http://localhost:8000](http://localhost:8000).

## How to Use

1. Choose an evaluation mode and subject.
2. Select the deck size and optional timer settings.
3. Start the evaluation session.
4. Use available assists while answering questions.
5. Review your score, streak, timing, and itemized answers when the session ends.

To study from your own materials, use the PDF Reviewer button and select a PDF file. Files are processed in the browser and are not uploaded to an external server by this app.

## Project Structure

```text
iReviewer/
├── index.html
├── LICENSE
└── README.md
```

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Tailwind CSS via CDN
- PDF.js for client-side PDF parsing

## Notes

- User preferences, including the selected theme and sound setting, are stored in the browser's local storage.
- The application depends on CDN resources, so those resources must be available when the page loads.
- Do not upload sensitive documents to the PDF Reviewer.

## License

This project is released under the MIT License. See [LICENSE](LICENSE) for the full license text.
