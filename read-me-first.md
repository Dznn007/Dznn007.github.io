# Peter Duong portfolio - simple version

1. Extract the whole ZIP.
2. Open `website/index.html` in your browser.
3. Open the HTML files and `website/css/custom.css` in your code editor.
4. Save after each change, refresh the browser and check the result.

## Add your own images

Put photos inside `website/images`. Use lowercase filenames without spaces, such as `profile.jpg` or `project-1.jpg`. The extension in the code must match the file.

| Change | Where | What to edit |
| --- | --- | --- |
| Home photo | `website/index.html` | Find the PHOTO comment. Change the image `src` and `alt` text. |
| Portfolio photo | `website/portfolio.html` | Change the card image and the matching FULL PHOTO image in its modal. |
| Project wording | `website/portfolio.html` | Edit the heading and paragraph in the card and its matching modal. |
| Browser-tab picture | `website/favicon/favicon-32x32.png` | Replace this file with your small square PNG. The four pages already link to it. |
| Browser-tab name | All four HTML pages | Change the words between `<title>` and `</title>`. |
| Résumé PDF | `website/pdf/peter-duong-resume.pdf` | Replace this file, keeping the same filename. |
| Colours and fonts | `website/css/custom.css` | Edit the clearly labelled CSS sections. |
| Contact details | `website/contact.html` and each footer | Update both the visible words and the link address. |

For example, the Home photo can become:

```html
<img class="img-fluid home-image" src="images/profile.jpg" alt="Portrait of Peter Duong">
```

No special cropping code needs to be changed. Your original résumé image is currently used as the Home image so the page has a real supplied asset until you choose a separate photo.

To change a project, keep its modal ID and button target matched. For example, `data-bs-target="#resume-preview"` opens the section with `id="resume-preview"`. Updating image paths does not require JavaScript.

If the browser-tab picture looks unchanged, try a hard refresh with Ctrl+F5.

## How the code is organised

The website is four ordinary HTML files and one short custom stylesheet. Bootstrap provides the responsive columns, mobile menu and modal previews. There is no custom JavaScript file, build command or package installation. The supplied Bootstrap JavaScript is still needed for the menu and previews.

The `vendor` folder contains supplied Bootstrap styles, icon files and font copies. You do not need to edit those files to customise the website.

Read `assessment-notes/code-guide.md` for the main HTML and Bootstrap concepts. Read `assessment-notes/submission-guide.md` for the remaining assessment requirements.
