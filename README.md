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

> 🔗 [View Project Repo](https://github.com/1suleyman/-Netflix-Data-Visualizations-with-Amazon-QuickSight/tree/main/netflix-quicksight-project)

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
