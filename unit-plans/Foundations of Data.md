Here is the complete unit plan in a single markdown file.

-----

# Unit Plan: Foundations of Data

## Unit Overview

  * **Unit Title**: Foundations of Data: Understanding File Formats
  * **Subject**: Introduction to Data Science, Programming with R
  * **Level**: Undergraduate (Introductory)
  * **Time**: One 90-Minute Block
  * **Goal**: Students will understand the basic concepts of data, learn how it's stored in a CSV, use Google Colab with an R runtime, and run an R script to load a CSV file.

-----

## Learning Objectives

By the end of this session, students will be able to:

1.  Define what a **variable** and a **value** are in the context of a dataset.
2.  Explain the purpose and structure of a **CSV file**.
3.  Create and navigate a **Google Colab notebook** that uses an R runtime.
4.  Use a provided R script to install the **`tidyverse`** package and import a CSV file into a **tibble**.

-----

## Key Vocabulary

  * **Data**: A collection of facts, such as numbers, words, measurements, or observations.
  * **Variable**: A characteristic being measured or counted (e.g., a 'column header' like `FirstName`).
  * **Value**: The specific measurement or observation for a variable (e.g., a 'cell entry' like `'Maria'`).
  * **CSV (Comma-Separated Values)**: A plain text file format used to store tabular data.
  * **R**: A programming language widely used for statistical computing and data analysis.
  * **Google Colab**: An interactive, cloud-based notebook environment for writing and running code.
  * **Runtime / Kernel**: The "engine" that Colab uses to execute your code. We will switch it from the default Python to R.
  * **Tidyverse**: A collection of R packages designed for data science that share a common philosophy.
  * **Tibble**: A modern, tidyverse-style data frame in R.

-----

## Materials & Preparation

1.  **Instructor Machine**: A computer with internet access and a web browser.
2.  **Student Machines**: Students will need a laptop or computer with a modern web browser and access to their Google account.
3.  **Slido Account**: Have a Slido event prepared with the polls listed in the teaching plan.
4.  **Dataset**: Select a simple, clean `.csv` file ahead of time. Download the file to your machine, ready to demo and share with students.
5.  **Colab R Notebook Link**: Create a new Colab notebook with an R runtime by visiting the following URL. Share this link with your students to save setup time.
      * `https://colab.research.google.com/#create=true&language=r`

-----

## Teaching Plan: 90-Minute Block

### Part 1: What Is Data and Where Does It Live? (25 minutes)

  * **(10 min) Introduction & Hook:**

      * Begin with an analogy: "Data is like the list of ingredients for a recipe. To understand the recipe (our analysis), you first need to understand the ingredients (our data)."
      * **Slido Engagement (Word Cloud)**:
        > **Poll Question:** "What one word comes to mind when you hear the word 'data'?"
        > *Display the resulting word cloud to the class to spark discussion.*
      * Introduce where to find data, framing them as "digital libraries for datasets." Briefly show the homepages of these sites:
          * **Kaggle** ([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets)): A community and platform for data science, great for interesting and unique datasets.
          * **Data.gov** ([https://www.data.gov/](https://www.data.gov/)): The home of the U.S. Government’s open data.
          * **Data.gov.tw** ([https://data.gov.tw/](https://data.gov.tw/)): The open data platform for Taiwan's government.
      * Briefly talk about common text file formats for storing this data. "Once you find data, it's stored in a file, often plain text. You'll commonly see formats like **CSV**, **JSON**, and **XML**. For today, we are focusing on **CSV**, because it's the simplest and most common format for the tables of data you'll work with."

  * **(15 min) Core Concepts & Demo Download:**

      * On a whiteboard or slide, clearly define **Variable**, **Value**, and **Variable Type**.
      * **Slido Engagement (Multiple Choice)**:
        > **Poll Question:** "In a dataset of student information, if `Major` is the variable, which of the following is a value?"
        > A) Student Name
        > B) 'Computer Science'
        > C) Grade Point Average
      * Transition to the demo: "Let's go to one of those data libraries, find a simple CSV file, and see these concepts in action."
      * Navigate to one of the sites (e.g., Kaggle), find a simple dataset, and **download the `.csv` file**.

### Part 2: Introducing the Workspace: R in Google Colab (20 minutes)

  * **(10 min) Setting up an R Notebook:**

      * Provide the direct link to the R Colab notebook.
      * Explain: "Google Colab usually speaks Python, but this special link tells it to create a notebook that speaks R. This is our workspace for today—no installation needed."

  * **(10 min) Getting Students Ready:**

      * Ensure all students have opened the link and have a new R notebook.
      * Guide them through uploading the `.csv` file: Click the **folder icon** on the left sidebar, then click the **"Upload to session storage"** button and select the file.

### Part 3: From Raw File to Tidy Data (35 minutes)

  * **(10 min) Demo: Deconstructing the CSV File:**

      * **Instructor Demo**: "Before we bring this into our coding environment, let's look at the file itself. It looks like a simple icon, but what's inside?"
      * **Open the downloaded `.csv` file using a plain text editor** (like Notepad on Windows or TextEdit on Mac). Point out the header row (the variables), the subsequent rows of data, and emphasize the commas that separate the values. State clearly: "This raw text is what the computer actually reads. The comma is the **delimiter** that tells it where one value ends and the next begins."
      * **Now, open the *same file* in spreadsheet software** (like Excel or Google Sheets). Show the class how the software interprets the raw text and commas to create a clean, organized table. This visual contrast is the key "aha\!" moment.

  * **(25 min) Guided R Coding in Colab:**

      * **Transition**: "Okay, we've seen the raw view and the spreadsheet view. Now, let's learn how to load this data the way a data scientist would—by writing code."
      * Guide students through the R script in Colab as previously outlined (installing and loading `tidyverse`, using `read_csv`, and printing the result).

    <!-- end list -->

    ```r
    # Step 1: Install the tidyverse package
    # We do this first because Colab provides a fresh, blank environment every time.
    install.packages("tidyverse")

    # Step 2: Load the tidyverse library into our session
    # This is like unlocking our toolkit after we've installed it.
    library(tidyverse)

    # Step 3: Read the CSV file into a tibble
    # The arrow <- assigns the data to a variable named 'df'.
    # Make sure the filename matches your uploaded file exactly!
    df <- read_csv("your_file_name.csv")

    # Step 4: Print the variable to see our imported data
    print(df)
    ```

### Part 4: Wrap-Up & Next Steps (10 minutes)

  * **(5 min) Review:**

      * Recap the session's narrative: "We started with the idea of data, looked at how it's stored in a raw CSV file, and then used a professional tool—Colab and R—to bring it to life as a structured table."

  * **(5 min) Exit Ticket & Independent Exploration:**

      * **Slido Engagement (Open Text)**:
        > **Poll Question:** "What is one question you still have, or what was the most interesting thing you learned today?"
        > *Review the anonymous answers on screen to address common questions.*
      * **Assign Independent Task:** "Before our next session, find one example of a JSON file online. In your notes, write one sentence describing how its structure (using `{}` and `[]`) looks different from the tabular structure of the CSV we used today."