# Google Colab and Google Drive Guide

**Course:** CSCI 171 — Introduction to Python  
**Instructor:** Proma Roy  
**Term:** Fall 2026

Google Colab is the standard Python notebook environment for this course. It runs in a web browser and does not require a local Python, Jupyter, or virtual-environment installation.

Useful official links:

- [Open Google Colab](https://colab.research.google.com/)
- [Open Google Drive](https://drive.google.com/)
- [Google's Welcome to Colab notebook](https://colab.research.google.com/notebooks/welcome.ipynb)
- [Google Colab FAQ](https://research.google.com/colaboratory/faq.html)

## 1. Required access

Before the first notebook lab, confirm access to:

- a working Google account;
- Google Drive in that account;
- Google Colab while signed in to the same account;
- a current web browser and reliable internet connection.

A personal laptop is optional. If one is brought to class, it should be charged before arrival. A student using a campus computer must still sign in to their own Google account. On a shared computer, never save the password in the browser and always sign out before leaving.

## 2. Create the course folder once

1. Open [Google Drive](https://drive.google.com/).
2. Select **New → New folder**.
3. Name the folder `CSCI 171 - Fall 2026`.
4. Open it and create:
   - `00_Course_Info`
   - `01_Class_Notebooks`
   - `02_Notebook_Labs`
   - `03_Assignments`
   - `04_Group_Project`
   - `05_Data`

Do not keep every course file in Drive's top level or in the automatic `Colab Notebooks` folder. Move each notebook into its course subfolder so it can be found later.

## 3. Create an in-class practice notebook

1. Open [Google Colab](https://colab.research.google.com/).
2. Select **File → New notebook**.
3. Rename the notebook with the assigned meeting number and topic. For the Day 1 setup notebook, use `M00_colab_practice_lastname_firstname.ipynb`.
4. Select **File → Save a copy in Drive** if a Drive copy has not already been created.
5. In Google Drive, move the notebook into `CSCI 171 - Fall 2026/01_Class_Notebooks`.
6. During class, add text and code cells as directed in the live lab. Enter, predict, run, repair, and annotate the code in this personal notebook.
7. Run code cells with the play button or **Shift+Enter** and keep the cells in the order used during class.
8. Confirm that Drive reports the notebook as saved before closing the tab. Reopen it later with **File → Open notebook → Google Drive**.

## 4. Open the post-class instructor notebook

Students work in their own blank Google Colab notebook during class. The completed instructor notebook is not published before or during class. It is released after the scheduled meeting ends, normally later that same day. Future notebook links remain unavailable so completed examples, intentional-error explanations, corrected code, and practice answers are not visible in advance. Weekly readings, graded activities, rubrics, and submission instructions are assigned separately in Brightspace.

1. Open the [course repository README](https://github.com/HeyPromaRoy/csci-171-introduction-to-python).
2. After class, select that meeting's released notebook from the linked meeting list or the repository's `notebooks/` folder.
3. On the notebook's GitHub page, select its **Open in Google Colab** badge.
4. Choose **File → Save a copy in Drive** if a personal reference copy is wanted.
5. Rename the reference copy and move it into the correct CSCI 171 Drive subfolder.
6. Keep the post-class reference separate from the personal notebook created during the live lab.

Suggested names:

- Class notebook: `M##_topic_lastname_firstname.ipynb`
- Notebook lab: `L##_topic_lastname_firstname.ipynb`
- Assignment: `A##_topic_lastname_firstname.ipynb`

## 5. Reopen personal work or obtain a fresh copy

- To open saved personal work: use **File → Open notebook → Google Drive** in Colab.
- To obtain a fresh post-class instructor notebook: return to the repository README, select a released notebook, and use that notebook's Colab badge.
- The notebooks do not include previous/next controls. The README's linked notebook list is the single course index.
- Never overwrite the clean instructor version; save a personal Drive copy first.

## 6. Understand what is and is not saved

The `.ipynb` notebook in Google Drive stores text cells, code cells, and saved outputs. Python variables and files created only inside the temporary remote runtime are not persistent. Colab may disconnect an idle runtime or replace it with a new one.

Therefore:

- confirm that the notebook itself is saved in Drive;
- rerun cells from the beginning after a new runtime connects;
- run any labeled **Colab runtime data setup** cell before a file-based lesson;
- do not treat `/content` or the Files panel as permanent storage;
- download or move any separately required output file before ending the session.

Mounting Google Drive gives notebook code access to Drive files and requires explicit authorization. It is not needed for the ordinary early-course notebooks. Use it only when the instructor's project or file instructions specifically require it.

## 7. Submit work

Follow the exact Brightspace instructions for each activity. Depending on the task, submission may require a downloaded `.ipynb` file or a permitted Drive link. Before submitting:

1. Run the notebook from the beginning.
2. Read every output and error message.
3. Confirm that all `TODO` items are complete.
4. Confirm that the student name and required reflection are present.
5. Confirm that Drive reports the latest changes as saved.

## 8. Common recovery steps

- **The notebook opened but edits are not being retained:** choose **File → Save a copy in Drive** and work in that copy.
- **A name existed earlier but is now undefined:** the runtime state was reset; run the notebook from the beginning.
- **A data file is missing:** run the notebook's labeled runtime data setup cell again.
- **A fresh post-class instructor notebook is needed:** return to the repository README, select the released notebook, and use its Colab badge.
- **The wrong Google account is active:** verify the account avatar before saving or submitting work.
- **Google account or device access prevents participation:** contact the instructor promptly so an appropriate course-access option can be discussed.
