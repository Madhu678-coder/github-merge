## Assignment-3;Branching Strategies & Merge Conflicts
## Objective
work with branches an resolving the merge conflicts usinf github flow

## Tasks Completed

1. Created a new GitHub repository and followed **GitHub Flow**:
   - Work on feature branches.
   - Open pull requests early and frequently.
   - Merge only after review/conflict resolution.

2. Created a simple HTML page (`index.html`).

## Branches Created

- **Branch A**: `feature/update-styling`  
  Modified styles in `index.html`.

- **Branch B**: `feature/add-content`  
  Modified the paragraph text in 'index.html'.

## Merge Conflict Simulated

- Both branches modified `index.html` — different sections, but same file.
- Merged `feature/update-styling` first.
- Encountered a **merge conflict** while merging `feature/add-content`.

##  Conflict Resolution Steps

1. Switched to conflict branch and pulled updates from `main`:
   git checkout feature/add-content
   git pull origin main

2. Conflict appeared in `index.html`:
   ```html
   <<<<<<< HEAD
   <p>This is a simple website created using HTML, CSS, and JavaScript.</p>
            <button id="toggleButton">Paragraph</button>
   =======
   <p>This website is built to showcase my portfolio and projects</p>
   >>>>>>> feature/add-content
   ```

3. Manually resolved by combining both:
   <p>This is a simple website created using HTML, CSS, and JavaScript.</p>
            <button id="toggleButton">Paragraph</button>

            <p>This website is built to showcase my portfolio and projects</p>
            <button id="toggleButton">Toggle Paragraph</button>

4. Finalized resolution:
   git add index.html
   git commit -m "fix: resolve merge conflict in index.html"
   git push origin feature/add-content

5. Successfully merged the pull request.
## ✅ GitHub Repository

[🔗 GitHub Repository Link] https://github.com/Madhu678-coder/github-merge

---

## 📸 Merge Conflict & Resolution Screenshots
![Screenshot 2025-05-07 010951](https://github.com/user-attachments/assets/0821ed61-3f2c-4235-bb73-712da417eef1)
![Screenshot 2025-05-07 014112](https://github.com/user-attachments/assets/ddc0cdcb-83be-4e82-8be4-49a9a61a78f0)
![Screenshot 2025-05-07 014144](https://github.com/user-attachments/assets/d1de880b-3d48-4230-b2b0-8df2fc73fdfe)
![Screenshot 2025-05-07 014310](https://github.com/user-attachments/assets/b1b76ceb-85a2-4b23-9630-480ebd3c74f2)
![Screenshot 2025-05-07 015023](https://github.com/user-attachments/assets/57732694-1a4f-46dd-ab7d-50547aa7e60f)






- ![Conflict Screenshot](screenshots/merge-conflict.png)
- ![Resolved Screenshot](screenshots/conflict-resolved.png)

---
