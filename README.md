# prismic-custom-types

JSON for the custom types we use to provision a new Prismic account

See https://prismic.io/docs/core-concepts/themes for instructions on what this does, and how to run it.

Essentially, this will speed up the process of creating a new account, and populating it with the custom types (course, syllabus, lesson_detail).

It will NOT create the instances of the Course and Syllabus types or download the API key. You will still have to do these steps.

### Running the scripts

`npm install -g prismic-cli`

From some folder (where you don't mind new folders being created), run:  
`prismic theme --theme-url https://github.com/didacticventures/prismic-custom-types --conf config.js`

Follow the prompts. You'll have to:
- Specify a repository name (`[schoolSlug]-maven`), and the same name for the folder that the project files will be downloaded into
- Create a new username/password (use the instructor's email, and save it into the Course Ops vault in 1Password)
- Once the script has run, log into Prismic with these credentials
- Create instances of the Course and Syllabus, and populate their UID fields
- Create the API app and save the information in the script.

<img width="1010" alt="Screen Shot 2021-06-22 at 4 43 28 PM" src="https://user-images.githubusercontent.com/256076/123013399-faab5200-d378-11eb-9bf8-fdd16bb86a56.png">
