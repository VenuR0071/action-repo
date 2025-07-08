# action-repo

This repository serves as the source for demonstrating GitHub webhook functionality.
It is configured to send events (pushes, pull requests, and merges) to a webhook endpoint for processing and display.

## Purpose


The primary purpose of this repository is to trigger GitHub actions  that are then captured by a separate webhook receiver application likely your 
`webhook-repo`. This allows for real-time tracking and display of repository activity.

### How to Use (for Testing)

**1. Clone the repository:**

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/action-repo.git
cd action-repo
```
**2. Make changes and commit:**

```bash
echo "New content" >> new-file.txt
git add new-file.txt
git commit -m "Add new file to trigger push event"
```
**3. Push to GitHub:**

```bash
git push origin main
```
(Note: If you encounter a "rejected" error, run git pull origin main first to sync with the remote.)

**4.Create Pull Requests & Merges:**

```bash
You can also create new branches, push changes, and then open pull requests on GitHub.
Merging these pull requests will also trigger webhook events.
```
