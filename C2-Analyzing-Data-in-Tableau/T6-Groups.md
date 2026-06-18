# 🗂️ Groups

---

## 1. Introduction

00:00 - 00:24

Welcome back! It's Lis again and I'll be your instructor for this chapter.

We've seen that there are many ways to slice and dice data.

So far, we've used:

- **Filters**
- **Calculated Fields**

These tools allow us to slice data and create different perspectives for analysis.

In this chapter, we'll expand our Tableau toolbox by learning about:

- **Groups**
- **Sets**
- **Parameters**

Let's begin with **Groups**.

---

## 2. What Are Groups?

00:24 - 00:59

### Definition

**Grouping** is the process of combining related rows within a field into a single category.

Groups allow analysts to create new categories that are not originally provided in the source data.

### Example: Countries and Continents

Imagine a dataset containing:

| Country |
|-----------|
| United States |
| Canada |
| Mexico |
| France |
| Germany |
| Japan |

The dataset contains a field called **Country**, where each row represents a different country.

Using groups, we can combine countries into larger categories such as continents.

### Example Grouping

| Country | Group (Continent) |
|-----------|------------------|
| United States | North America |
| Canada | North America |
| Mexico | North America |
| France | Europe |
| Germany | Europe |
| Japan | Asia |

This creates a new level of organization that is not explicitly stored in the original dataset.

---

## 3. Custom Groups

Groups can be customized to fit specific analytical needs.

Examples include:

### 🌍 Geographic Groups

- Continents
- Regions
- Trade zones

### 🌐 Economic Groups

- G20 countries
- OECD countries
- Developing economies

### 👥 Population-Based Groups

Countries can be grouped based on:

- High population
- Medium population
- Low population

### 📦 Product Groups

Products can be grouped into categories such as:

- Accessories
- Furniture
- Clothing
- Electronics

The goal is to create useful categories that make analysis easier and more meaningful.

---

## 4. When to Use Groups?

00:59 - 01:41

There are two primary use cases for groups in Tableau.

---

### Use Case 1: Create Consistency in Data

Groups can help standardize data when different values refer to the same thing.

#### Example: Country Names

Suppose users manually enter their country.

Different users may enter:

| User Input |
|-------------|
| United States |
| USA |
| U.S.A. |
| US |
| U.S. |

Although these values refer to the same country, Tableau sees them as separate values.

Using Groups, all of these entries can be combined into a single category:

| Original Value | Group |
|----------------|--------|
| United States | United States |
| USA | United States |
| U.S.A. | United States |
| US | United States |
| U.S. | United States |

### Benefits

- Improves data quality
- Reduces inconsistencies
- Simplifies analysis
- Creates cleaner visualizations

---

### Use Case 2: Create a New Level of Aggregation

Groups can also be used to summarize data at a higher level.

#### Example: Countries to Continents

Instead of analyzing individual countries:

| Country |
|-----------|
| France |
| Germany |
| Italy |

We can aggregate them into:

| Continent |
|-------------|
| Europe |

This allows analysts to compare broader categories rather than individual values.

#### Example: Products to Categories

Individual products:

| Product |
|-----------|
| Desk Lamp |
| Office Chair |
| T-Shirt |
| Backpack |

Can be grouped into:

| Category |
|-------------|
| Furniture |
| Clothing |
| Accessories |

This creates a higher-level view of the data.

### Benefits

- Simplifies reporting
- Reveals broader trends
- Reduces complexity
- Supports strategic analysis

---

## 5. Why Groups Are Useful

Groups help analysts:

- Create custom categories
- Improve data consistency
- Aggregate data into meaningful levels
- Simplify complex datasets
- Build clearer visualizations
- Discover patterns more easily

Groups are especially valuable when the source data does not already contain the categories needed for analysis.

---

## 6. Practice

01:41 - 01:47

Alright, now let's add some groups to our Divvy dataset!

---

# 📚 Key Takeaways

## What Is a Group?

A **Group** combines multiple related values into a single category.

---

## Main Purposes of Groups

### 1️⃣ Data Consistency

Used to combine different values that represent the same thing.

**Example:**

- USA
- US
- U.S.A.
- United States

→ Grouped as **United States**

---

### 2️⃣ Higher-Level Aggregation

Used to summarize detailed data into broader categories.

**Examples:**

- Countries → Continents
- Products → Categories
- Cities → Regions

---

## Benefits of Using Groups

✅ Cleaner data

✅ More consistent reporting

✅ Easier analysis

✅ Better visualizations

✅ Custom categories not available in source data

---

## Examples of Grouping

| Detailed Data | Group |
|---------------|--------|
| USA, Canada, Mexico | North America |
| France, Germany, Italy | Europe |
| Desk Lamp, Office Chair | Furniture |
| Backpack, Wallet | Accessories |

---

## Tableau Use Cases

Groups are useful when:

- Data contains inconsistent values
- You need broader categories
- Source data lacks the desired classification
- You want to simplify complex analyses
``` ````
