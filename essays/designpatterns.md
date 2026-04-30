---
layout: essay
type: essay
title: "Lego-fication of Design"
# All dates must be YYYY-MM-DD format!
date: 2026-04-29
published: false
labels:
  - Engineering
  - Design
---

<img width="200px" class="rounded float-start pe-4" src="https://miro.medium.com/v2/resize:fit:1100/format:webp/1*0omAifR-lzAB-cZ0rKuVjw.jpeg">

## Replicable Design

Give two different people a bin of Legos to create with and odds are their creations will be totally different. Now direct one to make an elaborate tree and the other to replicate said tree without disassembling it. The tree may be similar but it will take a long time and how could the replicator know what the insides were like? If the Lego builders were told specific ways to make components of the tree then it becomes easier for the replicator to understand what methods were used and make a good copy or even fix part of the original tree if, say, a cat knocks it over and part breaks off.  

The core concept of Legos is unlimited possibilities through modularity. Every Lego brick can interface with other Lego bricks. In the same vein, code interfaces with other bits of code but can be combined in a number of different ways. Lego sets include directions to build models that someone already designed and built, builders can then bring those methods to other projects while having a good template and knowledge of what to expect. The coding equivalent is a design pattern.

Design patterns are blueprints to solutions that are commonly needed in coding. They allow different coders to better understand what others have written and provide a robust base to alter as needed for your project.

Though I learned about design patterns only recently, I immediately recognized some of them in my own coding. For instance my implementation of a single Prisma client in a Nextjs project is an example of a singleton design pattern.

## A Single-what??

Design patterns give coders a standardized language to communicate what their code needs, does, and how it is structured. There are three types of design patterns: creational, structural, and behavioral.

Creational patterns deal with--you guessed it--creation. The aforementioned singleton pattern belongs to this type. This means that throughout the whole project there is only one of its kind. Structural patterns govern how collections of objects are represented. In my most recent project I used a facade pattern to bundle many actions relating to authorizing a user's access into one black box. Behavioral patterns are concerned with how components interact. An instance of my usage is an observer pattern in which a component reloads when a state changes.

In all, design patterns are very useful to implement and a great tool especially for teams. Just make sure you don't step on any!
