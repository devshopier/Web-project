# Contribute by translating lessons

We welcome translations for the lessons in this curriculum!

## Guidelines

There are [**translations**](https://github.com/microsoft/Web-Dev-For-Beginners/tree/main/1-getting-started-lessons/1-intro-to-programming-languages/translations) folders which contain the translated markdown files.

Translated lessons should follow this naming convention:

**README._[language]_.md**

where _[language]_ is a two letter language abbreviation following the ISO 639-1 standard (e.g. `README.es.md` for Spanish and `README.nl.md` for Dutch).

**Quizzes**

1. Add your translation to the quiz-app by adding a file here: https://github.com/microsoft/Web-Dev-For-Beginners/tree/main/quiz-app/src/assets/translations, with proper naming convention (en.json, fr.json). **Please don't localize the words 'true' or 'false' however. thanks!**

2. Add your language code to the dropdown in the quiz-app's App.vue file.

3. Edit the quiz-app's [translations index.js file](https://github.com/microsoft/Web-Dev-For-Beginners/blob/main/quiz-app/src/assets/translations/index.js) to add your language.

4. Finally, edit ALL the quiz links in your translated README.md files to point directly to your translated quiz: https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/1 becomes https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/1?loc=id

**THANK YOU**

We truly appreciate your efforts!
