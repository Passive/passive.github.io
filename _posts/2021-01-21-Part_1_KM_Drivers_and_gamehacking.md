---
title: Kernel Drivers & Gamehacking - Creating an undetectable cheat
layout: post
---

## Introduction
Learn about kernel mode drivers and methods of kernel-to-usermode communication
methods. In a small series of blog posts we will be developing a simple ESP for
a BattlEye protected process.

## What are kernel mode drivers?
A kernel mode driver is a driver that runs in "Ring 0", allowing for pretty much
total control over system memory. We use kernel mode drivers to combat kernel mode
anti-cheat solutions such as EasyAntiCheat or BattlEye.

## What would one written for gamehacking do?
A kernel mode driver, written specifically to assist someone trying to hack a game
usually includes methods to read memory, write memory and get specific process
information.

## How does a game hacker interact with the driver?
Most of the time the game hacker will also write a usermode application "Ring 3", that
will communicate with the driver using different communication methods in order to
send and receive data.

## What different communication methods are there?
There are tons, and it would take a while to list them all. The main ones we will be
looking at are IOCTL (I/O control) and function hooking.

These will be explained in the next post, along with how to get started developing
drivers.

## Conclusion
In this post you should have learned a little bit about kernel mode drivers and
how they assist game hackers greatly.
