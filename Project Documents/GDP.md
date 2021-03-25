

# Geometric Deep Learning(GDL)
- History Of Geometric Deep Learning
- Brief Introdouction of Geometric Deep Learning
- Application of Geometric Deep Learning 
- Machine/Deep Learning vs Geometrict Deep Learning/Graph Representation Learning:
- Introduction; Structure of Graph

---
## **History of Geometric Deep Learning**
GDL History has been playing a very impact on the AI field. The vast majority of deep learning is performed on **Euclidean Data**. This includes datatypes in the 1-dimensional and 2-dimensional domain. But we don’t exist in a 1D or 2D world. All that we can observe exists in 3D, and our data should reflect that. Talking about existing Deep Learning-  Deep learning has applications in computer vision, natural language processing and audio analysis, requiring Euclidean or 2D data. To facilitate working with 3D data, researchers are exploring Geometric deep learning, an umbrella term for emerging techniques used to generalise (structured) deep neural models to **Non-Euclidean** domains such as graphs and manifolds.

The current deep learning algorithms such as Recurrent Neural Networks (RNN), Convolutional Neural Networks (CNN), and LSTM have seen tremendous growth in the last few years tackling problems in speech recognition, computer vision, image generation, language transition and more. Most of these deep learning algorithms work on Euclidean (1D or 2D) data. The researchers believe tapping 3D data will improve the accuracy of findings by leaps and bounds.

**Example:** Images, text, audio, and many others are all euclidean data.

![Euclidean data](https://i.imgur.com/vAQr3BO.png)

One of the challenges with traditional deep neural networks is that they cannot parse data. Also, most of these networks are based on convolutions, and convolution works better on Euclidean data. Especially in areas such as network science, physics, biology, computer graphics and recommender systems, researchers have to deal with non-Euclidean data such as manifolds and graphs — which cannot fit in the two-dimensional space. For instance, graphic specialisation or mesh in the computer graphics field is non-Euclidean data. **Non-euclidean** data can represent more complex data compared to 1D and 2D representation. 

Researchers believe, since the real world manifests in 3D, the data should reflect that. To make machine learning and deep learning achieve human-level efficiencies, researchers are now exploring the use of 3D data. 

![](https://i.imgur.com/ELfq5pc.png)

When we represent things in a non-euclidean way, we are giving it an **Inductive bias.** This is based on the intuition that, given data of an arbitrary type, format, and size, one can prioritize the model to learn certain patterns by changing the structure of that data. In the majority of current research pursuits and literature, the inductive bias that is used is relational. Building on this intuition, **Geometric Deep Learning (GDL)** is the niche field under the umbrella of deep learning that aims to build neural networks that can learn from non-euclidean data.

The prime example of a **Non-Euclidean datatype** is a graph. **Graphs** are a type of data structure that consists of nodes (entities) that are connected with edges (relationships). This abstract data structure can be used to model almost anything.

We want to be able to learn from graphs because:

> **Graphs** allow us to represent individual features, while also providing information regarding relationships and structure.

There are various types of graphs, each with a set of rules, properties, and possible actions. Graph theory is the study of graphs and what we can learn from them. This will be covered accorignl table of content.

---

## **GDL**
Geometric Deep Learning is the class of **Deep Learning** that can operate on the **non-euclidean domain** with the goal of teaching models how to perform predictions and classifications on relational datatypes

The difference between traditional Deep Learning and Geometric Deep Learning can be illustrated by imagining the accuracy between **scanning an image of a person versus scanning the surface of the person themselves.**

In traditional Deep Learning, dimensionality is directly correlated with the number of features in the data whereas in Geometric Deep Learning, **it refers to the type of the data itself, not the number of features it has.**

**Why Graph?**
Graphs are a general language for describing and
analyzing entities with relations/interactions. It is the fundamental term to extrect deep feature from 3D objects. Here we use Graph segmentation. It is a process of classifying one and all the components of a graph like nodes (entities), edges (relationships). Think of autonomous cars which need to get their environment monitored after a regular interval and predict what they would be next up to by the pedestrians.

Usually, human pedestrians are either represented as huge bounding boxes in three dimensions or as more degrees of motion skeletons. With faster and better three-dimensional semantic segmentation, autonomous car’s would have more and more algorithms which makes the perception feasible.

---

## Application of Geometric Deep Learning
The basic fundametal term of GDL is `Graph`. Many types of data and application is based on Graph.For a concrete example of how Graph Learning can improve existing machine learning tasks we can look at the computational sciences.

One of the bottlenecks in computational chemistry, biology, and physics is the representation concepts, entities, and interactions. The nature of science is empirical and is therefore the result of many external factors and relationships. Here are some examples of where this is most obvious:
* Protein interaction networks
* Neural networks
* Molecules
* Feynman diagrams
* Cosmological maps

![](https://i.imgur.com/rhjff9g.png)

![](https://i.imgur.com/jPGUTSX.png)

![](https://i.imgur.com/SiI1CNy.png)

---
## Types of Network and Graph

#### Networks (also known as Natural Graphs):
* **Social networks:** Society is a collection of 7+ billion individuals
* **Communication and transactions:** Electronic devices, phone calls, financial transactions
* **Biomedicine:** Interactions between genes/proteins regulate life
* **Brain connections:** Our thoughts are hidden in the connections between billions of neurons

### Graphs (as a representation):
* **Information/knowledge** are organized and linked
* **Software** can be represented as a graph
* **Similarity networks:** Connect similar data points
* **Relational structures:** Molecules, Scene graphs, 3D shapes, Particle-based physics simulations


`Sometimes the distinction between networks & graphs is blurred`

---

## Machine/Deep Learning vs Geometrict Deep Learning/Graph Representation Learning:

Complex domains have a rich relational structure, which can be represented as a relational graph. By explicitly modeling relationships we achieve better performance!

In Modern ML/DL tools is not as much complex like Graph. Modern deep learning toolbox is designed for simple sequences & grids

## Modern ML Toolbox

![](https://i.imgur.com/5Jw8dpe.png)

## Deep Learning in Graph
How can we develop neural networks that are much more broadly applicable?
Graphs are the new frontier of deep learning

![](https://i.imgur.com/4snLxmJ.png)

## Why Is It Hard?
**Networks are complex:** 
* Arbitrary size and complex topological structure (i.e., no spatial locality like grids)

![](https://i.imgur.com/UMZwIPi.png)

* No fixed node ordering or reference point
* Often dynamic and have multimodal features

## Representation Learning in GDL

![](https://i.imgur.com/Fp0Yv7F.png)

**Map nodes to d-dimensional embeddings such that similar nodes in the network are embedded close together**

![](https://i.imgur.com/YO7kvav.png)

## Introduction; Structure of Graph
The two prerequisites needed to understand Graph Learning is in the name itself; Graph Theory and Deep Learning. This is all you need to know to understand the nature of, and build a high-level intuition for these two ideas.

## Graph Theory — crash course
What is a graph?
A **graph**, in the context of graph theory, is a structured datatype that has nodes (entities that hold information) and edges (connections between nodes that can also hold information). A graph is a way of structuring data, but can be a datapoint itself. Graphs are a type of Non-Euclidean data, which means they exist in 3D, unlike other datatypes like images, text, and audio. Graphs can have certain properties, which limit the possible actions and analysis that can be performed on them. These properties can be defined.

**Graph Definitions** A set of items connected by edges. Each item is called a vertex or node. Formally, a graph is a set of vertices and a binary relation between vertices, adjacency.
![](https://i.imgur.com/h223xVH.png)


Graphs can have labels on their **edges and/or nodes**, 
![](https://i.imgur.com/vG9neFP.png)


Labels can also be considered **weights**, but that’s up to the graph’s designer.


Labels don’t have to be numerical, they can be **textual**.


![](https://i.imgur.com/LeaG16f.png)

**Labels don’t have to be unique;** it’s entirely possible and sometimes useful to give multiple nodes the same label. Take for example, a hydrogen molecule:
![](https://i.imgur.com/ZyccUkj.png)


Graphs can have **features** (a.k.a attributes).
![](https://i.imgur.com/nf9YHYP.png)

Take care not to mix up features and labels. An easy way to think about it is using an analogy to names, characters, and people:


`a node is a person, a node’s label is a person’s name, and the node’s features are the person’s characteristics`.

---

### Graphs can be Directed or Undirected:
![](https://i.imgur.com/iZGiwg3.png)
A node in the graph can even have an edge that points/connects to itself. This is known as a self-loop.

---
Graphs can be either:
* **Heterogeneous** — composed of different types of nodes
* **Homogeneous** — composed of the same type of nodes
and are either:
* **Static** — nodes and edges do not change, nothing is added or taken away
* **Dynamic** — nodes and edges change, added, deleted, moved, etc.
Roughly speaking, graphs can be vaguely described as either
* **Dense** — composed of many nodes and edges
* **Sparse** — composed of fewer nodes and edges
Graphs can be made to look neater by turning them into their planar form, which basically means rearranging nodes such that edges don’t intersect

These concepts and terminology will come in handy as we explore the many different methods currently being employed in the various GNN architectures. Some of these basic methods are described in:

---
### Node Degree
![](https://i.imgur.com/rkwJ6e3.png)

---
### Bipartite Graph 
![](https://i.imgur.com/3TstS9Y.png)

---
### Representing Graph: Adjacency Matrix
![](https://i.imgur.com/KqDyUtt.png)

---
### Adjacency Matrix
![](https://i.imgur.com/3JFpsM8.png)

---
### Adjacency Matrix And Sparse
![](https://i.imgur.com/LvDsoi2.png)

---
### Networks Are Sparse Graph
![](https://i.imgur.com/uTu14UJ.png)

---
### Representing Graph: Edges List
![](https://i.imgur.com/haMEHiK.png)

---
### Representing Graph: Adjacency List

![](https://i.imgur.com/ZYPsb52.png)

---

## Different Types of Tasks
We are generally perform four types of tasks by using Graph Machine Learning Algorithms.

* **Node-Leve ML Task**
* **Edge-Level ML Task**
* **Sub Graph- Level Ml Task**
* **Graph Level ML Taks**

