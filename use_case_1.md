Use case 1: Social media impact explorer

Stages covered: data understanding, preprocessing, cleaning, analysis, visualization.

Step 1. Profile (Plan mode)
Look at the CSV in data/ or in the current directory. Do not change it. Write outputs/profile.md covering rows, columns, inferred types, missing values, duplicates, and which columns contain free text. Then tell me in 5 lines what kind of dataset this is and what questions it could answer.

Audience moment: they pick the question to investigate from the options it lists.

Step 2. Cleaning plan, then do it
Propose a cleaning plan as a short numbered list, with the trade-off of each step. Don't run anything yet.

Vote on the plan, switch to Build, then:

Run the approved steps. Save data/clean/clean.csv and log every change with row counts to outputs/changes.log.
Step 3. Analysis and visualization

Implement one of the use cases in detail. Example:

Take the cleaned CSV (data/clean/clean.csv) and plot some useful graphs. Decide which chart types fit the data, and build them with code. Save the graphs in outputs/graphs/.
Use case 2: Image describer and CSV builder

Takes a folder of about 4 images and produces alt text, keywords and file details, all collected in one CSV.

Step 1. Inventory (Plan mode)
List every image in images/ with filename, format, width, height and size. Flag any file that won't open. Save outputs/inventory.csv and summarize in 3 lines.
