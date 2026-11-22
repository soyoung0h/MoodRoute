# MoodRoute

Music genre recommendations for mental wellness. You rate how you feel on four states (anxiety, depression, insomnia, panic) from 1 to 5, and it recommends your top 3 genres.

A self-initiated project that started from my interest in both music and psychology. Placed 3rd of 63 teams at the 2024 INFORMS Analytics Poster Competition.

## What's in it

- **Survey data:** cleaned and wrangled survey data on how music genres relate to these four states in Excel
- **Recommendation model:** Python (`Music_and_Mental_Health.ipynb`). Each state has a top 3 genre list. A genre gets 3, 2, or 1 points depending on its rank for that state, multiplied by your rating, and the genres with the highest total are recommended
- **Website:** HTML site hosted on AWS S3, opened via QR code
- **Visualization:** general statistics in Tableau
- **Automation:** survey result processing with UiPath
- Poster and presentation are in the PDFs

Not medical advice, just a starting point for finding music that might help.

## Nov 2026 updates

- genre list is stored once in the class instead of copied into two functions
- typing a letter or a number outside 1–5 no longer crashes it, it just asks again
- removed the duplicated recommend/print code in the retake loop
- fixed comment typos
