# K-Means Clustering Tutorial

**A Hands-On Guide to Unsupervised Learning & Clustering**

This is an interactive tutorial designed to teach you **K-Means Clustering**—one of the most intuitive and widely-used unsupervised learning algorithms in machine learning. It moves at a teaching pace, with explanations, visualizations, and interactive exercises.

---

## 📚 Learning Path

**This tutorial is designed for anyone who wants to understand clustering**, from complete beginners to those brushing up on fundamentals. No advanced math required—just middle maths and curiosity!

### The K-Means Notebook (`Kmeans_Clustering.ipynb`)

This is the **first tutorial**. It walks you through:

1. **What is K-Means?** — The core question it answers: _"If I divide my data into K groups, where should the boundaries be?"_
2. **The Algorithm Step-by-Step** — How initialization, assignment, and update cycles work
3. **Why Standardization Matters** — Why scaling features equally affects clustering quality
4. **Implementing with Real Data** — Using the NCI60 cancer cell line dataset (60 samples, 6,144 gene expression features)
5. **Visualization Techniques** — How to visualize high-dimensional clusters using PCA
6. **Finding the Optimal K** — The Elbow Method: picking the right number of clusters
7. **Comparing Different K Values** — Side-by-side analysis of K=3, K=4, K=5
8. **When K-Means Fails** — Visual demonstration of limitations (non-spherical clusters, outliers, scaling issues)
9. **Interactive Exercise** — Hands-on practice for you to modify and experiment

**Open Tutorial** → [`Kmeans_Clustering.html`](./Kmeans_Clustering.html)
**Open Source Notebook** → [`Kmeans_Clustering.ipynb`](./Kmeans_Clustering.ipynb)

---

## 📚 Part 2: Hierarchical Clustering Tutorial

Once you understand K-Means, explore an alternative approach with hierarchical clustering.

### The Hierarchical Clustering Notebook (`Hierarchical_Clustering.ipynb`)

This is the **second tutorial**. It teaches you:

1. **What is Hierarchical Clustering?** — Building a tree of clusters instead of picking K upfront
2. **Dendrograms** — Visual representation of how clusters merge together
3. **Linkage Methods** — Different ways to measure distance between groups (single, complete, average, Ward)
4. **Reading the Dendrogram** — How to cut the tree and decide how many clusters you want
5. **Comparing Methods** — See how different linkage methods produce different results on the same data
6. **When to Use Hierarchical** — Advantages over K-Means (no K needed, shows full clustering process)
7. **When NOT to Use** — Understanding limitations (computationally expensive, hard to scale)

**Open Tutorial** → [`Hierarchical_Clustering.html`](./Hierarchical_Clustering.html)
**Open Source Notebook** → [`Hierarchical_Clustering.ipynb`](./Hierarchical_Clustering.ipynb)

---

## 🎯 The Big Ideas

### Problem: How Do We Group Similar Data Points?

Imagine you have:

- 60 cancer cell lines with 6,000 gene measurements each
- You want to find which cell lines are **naturally similar**
- But you **don't have labels** (that's why it's _unsupervised_ learning)

**K-Means answers:** _Group them into K clusters where points in the same cluster are close to each other._

### Solution: Find Cluster Centers (Centroids)

1. **Pick K random starting points** (centroids)
2. **Assign** each data point to its nearest centroid
3. **Update** each centroid to be the center of its assigned points
4. **Repeat** until nothing changes (convergence)

That's it! The algorithm then minimizes the distance within clusters.

### Why Learn This?

✅ **Intuitive** — The algorithm logic is simple and visual  
✅ **Practical** — Used in real production systems  
✅ **Fast** — Scales to millions of data points  
✅ **Foundational** — Understanding K-Means makes other algorithms clearer

---

## ✨ Why I Built This

I created this tutorial because K-Means is often taught in one of two extremes:

1. **Too theoretical** — Heavy on math, light on intuition
2. **Too code-heavy** — Just run the code, don't understand why

**This tutorial** sits in the middle: explaining the "why," showing the "how," and letting you experiment with the "what-ifs."

It's designed for someone like you—curious enough to dig in, but wanting clarity over complexity.

---

## 📂 Project Structure

```
Tutorial Class/
├── README.md                                      # You are here
├── KmeansClustering.ipynb                        #  First tutorial
├── Hierarchical_Clustering_Tutorial.ipynb        # Second tutorial
└── requirements.txt                              # Python dependencies
```

---

## 💡 Key Takeaways (The TL;DR)

1. **K-Means finds cluster centers** that minimize within-cluster distance
2. **Standardization is essential** — it makes all features equally important
3. **The Elbow Method helps you choose K** — look for the "bend" in the WCSS curve
4. **K-Means assumes spherical clusters** — it fails on crescent/ring shapes
5. **Use multiple initializations** (n_init > 1) to avoid local minima
6. **Visualization (PCA) is crucial** — you can't understand 6,144 dimensions without it
7. **Theory vs. Practice** — Perfect math ≠ best solution (sometimes pragmatism wins)

---

## 📜 Sources

This tutorial uses the **NCI60 dataset** from ISLP (Introduction to Statistical Learning with Python).

Dataset source: [ISLP Documentation](https://www.statlearning.com/)

---

_Last Updated: April 2026_
