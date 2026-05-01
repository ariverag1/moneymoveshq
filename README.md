# MoneyMovesHQ

Static website for MoneyMovesHQ.

## Project Structure

```text
.
|-- index.html
|-- images/
|   |-- confidence.jpg
|   |-- grad_parents.jpg
|   |-- grad_party.jpg
|   |-- grad_speech1.jpg
|   |-- grad_speech2.jpg
|   |-- guanajuato-mexico.jpg
|   |-- la-marathon.jpg
|   |-- video-thumb-1.jpg
|   `-- video-thumb-2.jpg
`-- README.md
```

Image paths in `index.html` use the deployable format:

```html
images/filename.jpg
```

## Run Locally

Open `index.html` directly in a browser, or run a simple local server from the project folder:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Push To GitHub

From the project folder:

```bash
git add index.html images README.md
git commit -m "Prepare site for GitHub and Netlify"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPOSITORY` with your GitHub account and repository name.

## Deploy On Netlify

1. Log in to Netlify.
2. Select **Add new site**.
3. Choose **Import an existing project**.
4. Connect the GitHub repository.
5. Use these settings:
   - Build command: leave blank
   - Publish directory: `.`
6. Deploy the site.
