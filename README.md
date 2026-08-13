# Access-Certification-Campaign
a small, realistic "who has access to what" dataset, followed by a completed access review where you personally play the role of reviewer, plus a written SoD conflict report — exactly like what a junior IGA analyst produces in a real job. Basically, it is an Access review campaign, usually done in a sailpoint or other IGA platforms. But I'm planning on zero-cost projects, and this is what in an organisation does every time for an Access review campaign. 

# Step 1 — Open a blank spreadsheet:
- Open your browser and go to sheets.google.com (or open Excel if you have it installed)
- If using Google Sheets: click the big blank spreadsheet button (the plus sign) to start a new one
- Rename it by clicking the "Untitled spreadsheet" text at the top-left, and type: "Access Review " or which suits yourselves

# Step 2 — Build your sample data:
- You're going to create a fake but realistic dataset of 12 employees and their access. You can ask to any AI for this fake realistic employee datasheet based on this type of column of header. Ask specifically for IGA access review campaign project, including the SoD conflicts, stale/leftover access etc. I'll give paste my datasheet which i've used for this project

  " Employee Name | Department | Job Title | System | Access Level | Date Granted "

- After getting the data sheet, paste it in the sheets and makes sure the data are arranged in the correct column header

# Step 3 — Spot the SoD conflict: 
- Look carefully at the "System" and "Access Level" columns for each person. Somewhere in this data is a classic Segregation of Duties violation — one person who can both create a vendor and approve payments to vendors.
- Add a new column G, header it: SoD Flag
- Find the employee(s) who have both "Create Vendor" and "Approve Payments" rows, and type SOD CONFLICT in column G on both of their rows
- Leave column G blank for everyone else

# Step 4 — Spot the stale/leftover access:
- Look at the "Date Granted" column. Notice that a role that has no obvious reason to need another role visibility.
- Add another column H, header it: Review Note
- On the review note, type: " Access doesn't match job function - investigate " or anything that suits yourselves.

# Step 5 — Run your own "certification campaign":
- Now put yourself in the role of reviewer.
- Add column I, header it: Decision
- Go through each row one at a time, and type either Approve or Revoke in column I, based on:

     Does the access level make sense for that person's job title?

     Is it flagged as an SoD conflict? (If yes, at least one of the two conflicting accesses should be Revoke)

     Is it flagged as a stale/mismatched review note? (If yes, lean toward Revoke or write a justification)
# Step 6 — Write your findings summary:
- At the bottom of the sheet, or in a new tab, write 3–4 sentences summarizing what you found — for example: "Found 1 SoD conflict between vendor creation and payment approval held by the same employee. Found 1 case of stale access inconsistent with the employee's current job title. Recommended revoking [X] and [Y]."

- This short write-up is exactly the kind of summary a real IGA analyst attaches to a completed certification campaign for the compliance/audit record.

# What this proves i understand:

By the end, i'll have hands-on proof that i can: read raw access data the way an IGA platform presents it, identify an SoD conflict manually (the same logic SailPoint automates), recognize privilege creep from the JML lifecycle, and make and justify real access review decisions — the core daily judgment work of an IGA/IAM analyst.


