Use case 2: Image describer and CSV builder

Takes a folder of about 4 images and produces alt text, keywords and file details, all collected in one CSV.

Step 1. Inventory (Plan mode)
List every image in images/ with filename, format, width, height and size. Flag any file that won't open. Save outputs/inventory.csv and summarize in 3 lines.
Step 2. Captions and alt text
Write scripts/describe.py that sends each image to the vision model through the configured provider and asks for a one-sentence caption, alt text under 125 characters, and 5 keywords. Save outputs/descriptions.csv with a review_status column set to "unreviewed". Skip images already done, and log failures. Test on 3 images first.
Step 3. Get the data into one CSV
Combine outputs/inventory.csv and outputs/descriptions.csv into one file, outputs/images.csv, with one row per image: filename, format, width, height, size, caption, alt text, keywords and review_status.
Step 4. Do something simple with it
Take outputs/images.csv and do something simple and useful with it. Suggest one idea first, then do it.
