DailyTask ✅

Plan your day. Complete your tasks. Stay productive.

DailyTask is a clean, modern, fully responsive daily task manager that runs entirely in your web browser — no backend, no database, no build tools, and no sign-up required. All of your data is stored locally on your own device using localStorage, and it's ready to deploy for free on GitHub Pages.

1. What is DailyTask?

DailyTask is a static website (just HTML, CSS, and JavaScript) that helps you:

Add tasks for the day with a category, priority, and optional time
Track each task's status: 🟢 Done, 🟡 Doing, or 🔴 Not Done
See your daily progress with a live progress bar and stats
Filter and search your task list
Browse a simple history of previous days
Switch between a light and dark theme

Because it's a static site, you can host it for free using GitHub Pages, open it on your phone, or even just double-click index.html to run it offline on your computer.

2. Features
✅ Add, edit, and delete tasks
✅ Three task statuses with clear color coding and text labels (Done, Doing, Not Done) — never color alone
✅ Categories: Study, Work, Personal, Exercise, Other
✅ Priorities: Low, Medium, High
✅ Optional task time, shown in 12-hour format
✅ Live progress bar + percentage (completed ÷ total × 100)
✅ Statistics cards: Total, Completed, Doing, Not Done
✅ Filter tasks by status (All / Done / Doing / Not Done)
✅ Instant search-as-you-type
✅ Friendly empty state when you have no tasks yet
✅ Tasks automatically saved with localStorage — nothing is lost on refresh or after closing the browser
✅ Tasks are grouped by date, so a new day starts with a fresh, empty list without deleting older tasks
✅ History panel to look back at any previous day
✅ Light / Dark mode toggle (saved as a preference)
✅ Fully responsive — works on desktop, tablet, and mobile
✅ Smooth, subtle animations
✅ Accessible: labeled form fields, keyboard-friendly controls, visible focus states, and status is always shown as text (not just color)
✅ No external servers — your data never leaves your browser
✅ Zero dependencies — plain HTML, CSS, and JavaScript only
3. Project files
text
DailyTask/
│
├── index.html      → Page structure/content
├── style.css        → All styling, theme, and layout
├── script.js        → App logic (tasks, storage, filters, history, theme)
└── README.md         → This file
4. How to run it locally

You don't need to install anything.

Option A — Just open it

Download/unzip the DailyTask folder.
Double-click index.html.
It opens in your default browser and works immediately.

Option B — Use a simple local server (optional, but nice for development)

If you have Python installed, you can serve the folder so it behaves exactly like it will on GitHub Pages:

bash
cd DailyTask
python3 -m http.server 8000

Then open http://localhost:8000 in your browser.

No Node.js, npm, or build step is required at any point.

5. How to upload it to GitHub
Go to github.com and log in (or create a free account).
Click the + icon in the top-right corner → New repository.
Name it something like daily-task (any name is fine), then click Create repository.
On the new repository page, click uploading an existing file (or use Add file → Upload files).
Drag and drop all four files — index.html, style.css, script.js, and README.md — directly into the repository (not inside a subfolder).
Scroll down and click Commit changes.

(If you prefer the command line and have Git installed, you can instead run git init, git add ., git commit -m "Initial commit", and git push to your new repository — but the drag-and-drop method above works just as well and needs no installation.)

6. How to enable GitHub Pages
In your repository, click the Settings tab.
In the left sidebar, click Pages.
Under Build and deployment → Source, choose Deploy from a branch.
Under Branch, select main (or master) and folder / (root), then click Save.
Wait about 30–60 seconds, then refresh the page. GitHub will show a green banner with your live site URL, something like:
text
   https://your-username.github.io/daily-task/
Open that link — your DailyTask website is now live! 🎉

Any time you edit and re-upload index.html, style.css, or script.js, GitHub Pages will automatically update your live site within a minute or two.

7. How localStorage works (and what it means for your data)
localStorage is a small storage space built into every web browser, tied to the specific website (domain) you're visiting.
When you add, edit, complete, or delete a task, DailyTask immediately saves your entire task list into localStorage on your device.
The next time you open the site — even after closing the tab, closing the browser, or restarting your computer — your tasks are read back from localStorage and reappear exactly as you left them.
Tasks are stored per calendar date, so when a new day starts you get a fresh, empty task list automatically, while yesterday's tasks are kept and viewable in the History panel — nothing is deleted automatically.
Your theme preference (light/dark) is saved the same way.
Important: localStorage is specific to one browser on one device. It does not sync between your phone and your computer, and it is not sent to any server — DailyTask has no backend at all. If you clear your browser's site data/cache for this page, your saved tasks will be erased.
8. Customizing

Everything is plain HTML/CSS/JS, so feel free to open the files in any code editor and tweak things:

Colors and theme: edit the CSS variables at the top of style.css (:root and :root[data-theme="dark"])
Categories or priorities: edit the <select> options in index.html (both the "Add Task" form and the "Edit Task" modal)
Behavior/logic: edit script.js — functions are commented to explain what each part does

No build step is required after making changes — just save the file and refresh your browser (or re-upload to GitHub for the live site to update).

Enjoy staying on top of your day with DailyTask! ✅
