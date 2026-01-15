## About This Project

Welcome to **Project 3**! 🎉

In this project, I explore **web scraping and XML/HTML data extraction** in R. The goal is to practice real-world data collection from online sources and then organize, analyze, and visualize the data.

This project has **two main tasks**:

1.  Extracting episode information from the TV series *Friends* using an XML file.\
2.  Scraping data about Members of the European Parliament (MEPs) directly from their official website.

Throughout this project, I work with **R packages for web scraping, data wrangling, and visualization**, turning raw online data into structured insights.

------------------------------------------------------------------------

## Task 1 – Friends Episode Data

For this task, I use the XML file [`friends_info.xml`](https://raw.githubusercontent.com/intro-to-data-science-25/labs/main/data/friends_info.xml), which contains information about all episodes from *Friends*.

Here’s what I did:

-   Extracted the **season**, **episode number**, and **title** of all episodes into a data frame (`episode_df`).\
-   Identified all episodes **directed by Ross (David Schwimmer)** using XPath expressions.\
-   Created a **bar chart showing how often each main character (Ross, Rachel, Monica, Chandler, Joey, Phoebe) is mentioned in episode titles**.

This task helped me practice XML parsing and basic text analysis in R.

------------------------------------------------------------------------

## Task 2 – Scraping Members of the European Parliament

The European Parliament maintains a **full list of MEPs** on their website. For this task:

-   I scraped the MEP list and built a data frame (`meps_df`) with the following variables:

    | Variable         | Description                               |
    |------------------|-------------------------------------------|
    | `name`           | Full name of the MEP                      |
    | `ep_party_group` | European Parliament party group           |
    | `country`        | Country of the MEP                        |
    | `nat_party`      | National party of the MEP                 |
    | `profile_url`    | Link to the MEP's profile                 |
    | `mep_id`         | Numeric ID extracted from the profile URL |

-   I printed the **first 3 rows** and checked the **total number of MEPs** scraped.\

-   I also demonstrated **polite scraping** by showing how to download a few MEP profiles into a local folder without overwhelming the server.

This task allowed me to apply **HTML parsing, XPath, and good web scraping practices** in R.

------------------------------------------------------------------------

## Data Sources

-   Friends episodes XML: <https://raw.githubusercontent.com/intro-to-data-science-25/labs/main/data/friends_info.xml>\
-   European Parliament MEPs: <https://www.europarl.europa.eu/meps/en/full-list/all>

------------------------------------------------------------------------

## Tools & Packages

This project uses:

-   `rvest` & `xml2` – for web scraping and XML parsing\
-   `dplyr` & `stringr` – for data wrangling and string manipulation\
-   `ggplot2` – for visualization\
-   `knitr` – to render HTML tables

------------------------------------------------------------------------

## Project Summary

In my **third project**, I combined **web scraping, XML parsing, and visualization skills** to work with real online datasets. It shows how we can turn unstructured web data into **structured, meaningful insights** using R.
