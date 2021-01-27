![](assets/images/ga_log.png)

<br>
<br>
<br>
<h1> Project 3: Video Games rating by ESRB system rate </h1>

**Table of Contents:**

- [**Acknowledgment**](#Acknowledgment)
- [**Overview**](#overview)
- [**What is about?**](#what-is-about)
	- [Problem Statement:](#problem-statement)
- [**Requirement**](#Requirement)
- [**Dataset**](#datasets)
	- [Data dictionary](#Data-dictionary)

---

# Acknowledgment
- This data has been collected from [ESRB official website](https://www.esrb.org/).
- Rating explanation referenced to [IGN official website](https://www.ign.com/) and [ESRB official website](https://www.esrb.org/).
- This data has been collected for educational purposes and not for any other use.

# **Overview**
- This data contains the name for `1895 games` with `34 of ESRB rating content` as features for each game.<br>
- Also a test data with 500 games (Obserrvation) labeld.<br>
- A single datapoint is represented as a single number form `0-3` for `Console` and a `binary vector` for the `features of ESRB content`.

# **What is about?**

## Problem Statement
- Many parents are giving their children any game to play without thinking about what's the content of that game or what's the target age for it. and this is affecting the children specifically, because many games are not made for kids, either because of sexual content, drugs, and/or violence.
- ESRB works to empower parents to make informed decisions about the video games they purchase for their children and allow them to be played in their homes.
- The ESRB doesn’t aim to prohibit certain games from being purchased and played but rather hopes to provide concise and impartial information to parents and other consumers.

- ESRB rating: An assigned rating category that suggests the age-appropriateness of that particular game

---

# **Requirement**
- **`You need chrome driver for Selenium scraping.`**


# **Dataset**
- You can check the dataset on Kaggle: **[Click here](https://www.kaggle.com/imohtn/video-games-rating-by-esrb)**
<br><br>
-----

## **Data dictionary**

| Feature                 |   type     |                description                |  Keys  |
|:------------------------|:----------:|:------------------------------------------|:------:|
|title                    | **string** |Name of the game.                          |  ----  |
|console                  | **int** |The console on which the game was released.|0 = PS4<br> 1 = Xbox<br> 2 = Both<br>3 = other|
|Alcohol_Reference        | **int** |Reference to and/or images of alcoholic beverages.|0 = no<br>1 = yes
|Animated_Blood           | **int** |Discolored and/or unrealistic depictions of blood.|0 = no<br>1 = yes
|Blood                    | **int** |Depictions of blood.|0 = no<br>1 = yes
|Blood_and_Gore           | **int** |Depictions of blood or the mutilation of body parts.|0 = no<br>1 = yes
|Cartoon_Violence         | **int** |Violent actions involving cartoon-like situations and characters. May include violence where a character is unharmed after the action has been inflicted.|0 = no<br>1 = yes
|Crude_Humor              | **int** |Depictions or dialogue involving vulgar antics, including "bathroom" humor.|0 = no<br>1 = yes
|DrugRe_ference           | **int** |Reference to and/or images of illegal drugs.|0 = no<br>1 = yes
|Fantasy_Violence         | **int** |Violent actions of a fantasy nature, involving human or non-human characters in situations easily distinguishable from real life.|0 = no<br>1 = yes
|Intense_Violence         | **int** |Graphic and realistic-looking depictions of physical conflict. May involve extreme and/or realistic blood, gore, weapons, and depictions of human injury and death.|0 = no<br>1 = yes
|Language                 | **int** |Moderate use of profanity.|0 = no<br>1 = yes
|Lyrics                   | **int** |References to profanity, sexuality, violence, alcohol, or drug use in music.|0 = no<br>1 = yes
|Mature_Humor             | **int** |Depictions or dialogue involving "adult" humor, including sexual references.|0 = no<br>1 = yes
|Mild_Blood               | **int** |Some blood.|0 = no<br>1 = yes
|Mild_Cartoon_Violence    | **int** |Some violent actions involving cartoon.|0 = no<br>1 = yes
|Mild_Fantasy_Violence    | **int** |Some violent actions of a fantasy nature.|0 = no<br>1 = yes
|Mild_Language            | **int** |Mild to moderate use of profanity.|0 = no<br>1 = yes
|Mild_Lyrics              | **int** |Mild References to profanity, sexuality, violence, alcohol, or drug use in music.|0 = no<br>1 = yes
|Mild_Suggestive_Themes   | **int** |some provocative references or materials           |0 = no<br>1 = yes
|Mild_Violence            | **int** |Some scenes involving aggressive conflict.|0 = no<br>1 = yes
|No_Descriptors           | **int** |No content descriptors.|0 = no<br>1 = yes
|Nudity                   | **int** |Graphic or prolonged depictions of nudity.|0 = no<br>1 = yes
|Partial_Nudity           | **int** |Brief and/or mild depictions of nudity.|0 = no<br>1 = yes
|Sexual_Content           | **int** |Non-explicit depictions of sexual behavior, possibly including partial nudity.|0 = no<br>1 = yes
|Sexual_Themes            | **int** |References to sex or sexuality.|0 = no<br>1 = yes
|Simulated_Gambling       | **int** |Player can gamble without betting or wagering real cash or currency.|0 = no<br>1 = yes
|Strong_Language          | **int** |Explicit and/or frequent use of profanity.|0 = no<br>1 = yes
|Strong_Sexual_Content    | **int** |Explicit and/or frequent depictions of sexual behavior, possibly including nudity.|0 = no<br>1 = yes
|Suggestive_Themes        | **int** |Provocative references or materials.|0 = no<br>1 = yes
|Use_of_Alcohol           | **int** |The consumption of alcoholic beverages.|0 = no<br>1 = yes
|Use_of_Drugs_and_Alcohol | **int** |The consumption of alcoholic and drugs beverages.|0 = no<br>1 = yes
|Violence                 | **int** |Scenes involving aggressive conflict. May contain bloodless dismemberment.|0 = no<br>1 = yes
|ESRB_rating              | **string** |rating: RP - EC - E - E+10 - T - M - A    | RP , EC , E , ET , T , M , A|


<br>

---

**ESRB rating description:**

|ESRB_rating|Description      |
|-----------|-----------------|
|RP         | Rating Pending  |
|EC         | Early Childhood |
|E          | Everyone        |
|E 10+      | Everyone 10+    |
|T          | Teen            |
|M          | Mature          |
|A          | Adult           |
