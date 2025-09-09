# 📊 Netflix Data Visualizations with Amazon QuickSight

This project walks through **analyzing Netflix data** using **AWS S3** and **Amazon QuickSight**, turning raw datasets into interactive, insightful visualizations.

Whether you want to explore trends in movies vs. TV shows, release years, or genres, this project shows you **how to store, prepare, and visualize your dataset in the cloud**.

---

## 📂 Project Structure

```text
netflix-quicksight-project/
├── netflix_titles.csv      # Dataset CSV
├── manifest.json           # S3 manifest file for QuickSight
└── README.md               # Project instructions
```

> 🔗 [View Project Repo](#) (replace `#` with your repo link)

### Step 1: Store the Dataset in Amazon S3

Put your dataset in the cloud so QuickSight can access it easily.

1. **Create a new S3 bucket**

   * Example: `nextwork-quicksight-yourname`

I chose nextwork-quicksight-suleyman

2. **Upload your files**

   * Upload the CSV file.
   * Update the `manifest.json` with the S3 URL of your CSV file, then upload it.

3. **Take a screenshot**

   * Show your S3 bucket with both files.

<img width="454" height="266" alt="Screenshot 2025-09-09 at 14 20 42" src="https://github.com/user-attachments/assets/31e333b3-9624-44e5-8795-0b76dda44c95" />

---

### Step 2: Create Your Amazon QuickSight Account

Amazon QuickSight is where your data becomes **interactive visualizations**.

1. Sign up for the **free trial** of QuickSight Enterprise.

   * ⚠️ Uncheck any **optional add-ons** (like Paginated Reports) to avoid charges.
   * Enter your details for your QuickSight account - make sure the email you use is the same email for your AWS account. Or else you'll run into an error later!
   * Make sure you're setting up QuickSight in the correct region - it should be in the same region as the S3 bucket!

2. Give QuickSight **access to your S3 bucket**.

<img width="860" height="361" alt="Screenshot 2025-09-09 at 14 29 32" src="https://github.com/user-attachments/assets/fe501c02-0651-4b19-a500-c3a39701afe9" />

3. Complete account setup — it may take a minute for your account to be ready.

<img width="577" height="552" alt="Screenshot 2025-09-09 at 14 32 49" src="https://github.com/user-attachments/assets/149b08d8-3221-4305-8ef6-039fa81a726f" />

---

### Step 3: Connect S3 Bucket to QuickSight

Now it’s time to **link your data to QuickSight**.

1. Navigate to **Datasets → New dataset → S3**.

2. Enter:

   * Source name: `kaggle-netflix-data`

💡 What is the source name for?
This source name is just a label to remind you what this piece of data is about! In this case, we sourced the csv field from a database called Kaggle, and the file is all about Netflix TV shows and movies.

   * Manifest URL: S3 URL of your `manifest.json`

<img width="598" height="289" alt="Screenshot 2025-09-09 at 14 37 39" src="https://github.com/user-attachments/assets/c0c04a53-fcff-4486-a5f6-ca978d6af7ba" />

💡 So what does the manifest.json file do?
manifest.json tells QuickSight what your dataset looks like, so QuickSight knows how to understand the data and show it in charts or graphs. Without this map, QuickSight might get confused and not show your data correctly!

3. then Click visulize

<img width="590" height="287" alt="Screenshot 2025-09-09 at 14 40 20" src="https://github.com/user-attachments/assets/d5673c77-8853-4226-9a92-f8e8efef44fa" />

<img width="795" height="508" alt="Screenshot 2025-09-09 at 14 41 08" src="https://github.com/user-attachments/assets/88ce436d-1616-4b19-88b2-c6f819b3734f" />

4. Take a screenshot of your **dataset connection**.

<img width="815" height="651" alt="Screenshot 2025-09-09 at 14 41 52" src="https://github.com/user-attachments/assets/fc659cb3-6095-4ecd-b031-1fffdcfc0843" />

---

### Step 4: Create Your First QuickSight Visualization

Bring your Netflix data to life!

1. Explore fields and drag them into **visualizations**.

2. Start with:

   * **Pie chart**: e.g., `rating` distribution
   * **Horizontal bar chart**: e.g., `release_year` vs `type` (Movies/TV Shows)

3. Take a screenshot of your visualization.

<img width="810" height="405" alt="Screenshot 2025-09-09 at 14 48 29" src="https://github.com/user-attachments/assets/0df7f953-31d5-48ed-a4fb-11ac1b11da44" />

---

## 💡 What You’ll Learn

* Uploading datasets to **AWS S3**
* Preparing data with **manifest.json** for QuickSight
* Connecting S3 datasets to QuickSight
* Creating **interactive visualizations** and dashboards

---

## 📌 References

* [Amazon S3 Documentation](https://docs.aws.amazon.com/s3/index.html)
* [QuickSight Documentation](https://docs.aws.amazon.com/quicksight/index.html)
* [QuickSight S3 Dataset Integration](https://docs.aws.amazon.com/quicksight/latest/user/s3-data-sets.html)

Absolutely! Here’s your README rewritten in **first-person**, polished for clarity and flow while keeping all the instructions, screenshots, and explanations intact:

---

# 📊 Netflix Data Visualizations with Amazon QuickSight

In this project, I explore **Netflix data** using **AWS S3** and **Amazon QuickSight**, turning raw datasets into interactive, insightful visualizations.

I use this project to answer questions like:

* How do movies vs. TV shows compare over the years?
* What trends exist in release years and genres?
* How can I store, prepare, and visualize a dataset in the cloud?

---

## 📂 Project Structure

```text
netflix-quicksight-project/
├── netflix_titles.csv      # Dataset CSV
└── manifest.json           # S3 manifest file for QuickSight
```

> 🔗 [View Project Repo](#) *(replace `#` with your repo link)*

---

## Step 1: Store the Dataset in Amazon S3

I start by putting my dataset in the cloud so QuickSight can access it easily.

1. **Create a new S3 bucket**

   I named mine: `nextwork-quicksight-suleyman`

2. **Upload my files**

   * I uploaded the `netflix_titles.csv`.
   * I updated the `manifest.json` file with the S3 URL of my CSV file, then uploaded it to the bucket.

3. **Take a screenshot**

   Here’s my S3 bucket with both files uploaded:

<img width="454" height="266" alt="Screenshot of S3 bucket with CSV and manifest" src="https://github.com/user-attachments/assets/31e333b3-9624-44e5-8795-0b76dda44c95" />

---

## Step 2: Create My Amazon QuickSight Account

Next, I set up **QuickSight**, where my data becomes interactive visualizations.

1. I signed up for the **free trial** of QuickSight Enterprise.

   * ⚠️ I made sure to **uncheck optional add-ons** (like Paginated Reports) to avoid charges.
   * I used the **same email as my AWS account** to prevent access issues.
   * I selected the **same AWS region** as my S3 bucket.

2. I gave QuickSight **access to my S3 bucket**:

<img width="860" height="361" alt="QuickSight S3 access setup" src="https://github.com/user-attachments/assets/fe501c02-0651-4b19-a500-c3a39701afe9" />

3. QuickSight took a minute to be ready after setup:

<img width="577" height="552" alt="QuickSight account ready" src="https://github.com/user-attachments/assets/149b08d8-3221-4305-8ef6-039fa81a726f" />

---

## Step 3: Connect My S3 Bucket to QuickSight

Now it’s time to **link my dataset** to QuickSight.

1. I navigated to **Datasets → New dataset → S3**.

2. I entered the following:

   * **Source name**: `kaggle-netflix-data`

     > This is just a label to remind me what this dataset is about (Netflix titles from Kaggle).
   * **Manifest URL**: S3 URL of my `manifest.json`

<img width="598" height="289" alt="QuickSight dataset connection" src="https://github.com/user-attachments/assets/c0c04a53-fcff-4486-a5f6-ca978d6af7ba" />

💡 The `manifest.json` file acts like a **map**, telling QuickSight where my data lives and how to interpret it.

3. I clicked **Visualize** and confirmed the connection:

<img width="590" height="287" alt="QuickSight visualize" src="https://github.com/user-attachments/assets/d5673c77-8853-4226-9a92-f8e8efef44fa" />  

<img width="795" height="508" alt="QuickSight dataset fields" src="https://github.com/user-attachments/assets/88ce436d-1616-4b19-88b2-c6f819b3734f" />

4. I took a screenshot of the **dataset connection**:

<img width="815" height="651" alt="Screenshot of dataset connection panel" src="https://github.com/user-attachments/assets/fc659cb3-6095-4ecd-b031-1fffdcfc0843" />

---

## Step 4: Create My First QuickSight Visualization

Time to bring my Netflix data to life!

1. I explored the dataset fields and dragged them into **visualizations**.

2. I created my first visuals:

   * **Pie chart**: distribution of `rating`
   * **Horizontal bar chart**: `release_year` vs `type` (Movies/TV Shows)

3. Screenshot of my visualizations:

<img width="810" height="405" alt="QuickSight visualization example" src="https://github.com/user-attachments/assets/0df7f953-31d5-48ed-a4fb-11ac1b11da44" />

---

## 💡 What I Learned

* Uploading datasets to **AWS S3**
* Preparing data with **manifest.json** for QuickSight
* Connecting **S3 datasets to QuickSight**
* Creating **interactive visualizations** and dashboards

---

## 📌 References

* [Amazon S3 Documentation](https://docs.aws.amazon.com/s3/index.html)
* [QuickSight Documentation](https://docs.aws.amazon.com/quicksight/index.html)
* [QuickSight S3 Dataset Integration](https://docs.aws.amazon.com/quicksight/latest/user/s3-data-sets.html)
