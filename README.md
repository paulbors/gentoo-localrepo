# gentoo-localrepo
Fixes and patches to Gentoo Linux default tree.

## Table of Contents
* [gentoo-localrepo](#gentoo-localrepo)
  * [Table of Contents](#table-of-contents)
  * [What is Gentoo?](#what-is-gentoo)
  * [Installing Gentoo Linux](#installing-gentoo-linux)
  * [Why this project?](#why-this-project)
    * [Which bug fixes are published here?](#which-bug-fixes-are-published-here)
* [Gentoo Ebuilds](#gentoo-ebuilds)
  * [Basic guide to write Gentoo Ebuilds](#basic-guide-to-write-gentoo-ebuilds)
  * [Custom Repositories](#custom-repositories)
  * [Installing Ebuilds from this repo](#installing-ebuilds-from-this-repo)

## What is Gentoo?
Gentoo is a free operating system based on Linux that can be automatically
optimized and customized for just about any application or need.

Gentoo compiles from source but is not Linux From Surce.

## Installing Gentoo Linux
You can start by reading the [Gentoo Handbook](https://wiki.gentoo.org/wiki/Handbook:Main_Page) for your architecture.

## Why this project?
While looking over [Machine Learning with TensorFlow](https://www.manning.com/books/machine-learning-with-tensorflow),
I wanted to try it out on my favorite Linux distro and it turns out that at the time I wanted to install it Tensorflow
[was a bit unstable](https://github.com/tensorflow/tensorflow/issues/33108) when it came to the packages. While the core
developers were fixing those packages quite fast, I wanted to have my own cake and eat it too (patch before release).

Then I decided to keep the older patches in case I wanted to port them from one machine to another in order to distribute
the model training.

### Which bug fixes are published here?
By the time you read this chances are that most of the bug fixes would find its way into the official
[Gentoo](https://github.com/gentoo/gentoo) repository.

Some of them might make it there later, such as the backported fix
to Bazel v0.29.1 to get Tensorflow2 up and going before having to patch the more complex Tensorflow Ebuild.

Yet others might never make it since this is my own playground.

# Gentoo Ebuilds
Ebuilds are at the core of Gentoo's package installation. One can start here.

## Basic guide to write Gentoo Ebuilds
Get started with your Hello World package installer via the
[Basic guide to write Gentoo Ebuilds](https://wiki.gentoo.org/wiki/Basic_guide_to_write_Gentoo_Ebuilds).

## Custom Repositories
Technically speaking, this project is nothing but a [custome localrepo](https://wiki.gentoo.org/wiki/Custom_repository)
of 3rd party Ebuilds.

## Installing Ebuilds from this repo
As a user of Gentoo, you would setup your own [custome localrepo](https://wiki.gentoo.org/wiki/Custom_repository)
and use the ebuild from this repo until this evolve (if ever) big enough and useful enough for me to publish it
via [layman](https://wiki.gentoo.org/wiki/Layman).
