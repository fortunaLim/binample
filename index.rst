..
   # *******************************************************************************
   # Copyright (c) 2026 Contributors to the Eclipse Foundation
   #
   # This program and the accompanying materials are made available under the
   # terms of the Apache License Version 2.0 which is available at
   # https://www.apache.org/licenses/LICENSE-2.0
   #
   # SPDX-License-Identifier: Apache-2.0
   # *******************************************************************************

Binample Module Documentation
==============================

This is the documentation for **binample**, a simple example S-CORE module
created for learning the Bazel-based build and documentation workflow.

.. contents:: Table of Contents
   :depth: 2
   :local:

Overview
--------

Binample is a minimal "Hello World" application written in C++.
It prints a greeting message to the console and is used to practice the
Eclipse S-CORE module structure, build system, and docs-as-code workflow.

The main source code is located under ``score/binample/`` and can be built with:

.. code-block:: bash

   bazel build //score/binample:binample

Build and Run
-------------

To build the binample application:

.. code-block:: bash

   bazel build //score/binample:binample

To run it:

.. code-block:: bash

   bazel run //score/binample:binample

Expected output:

.. code-block:: text

   Hello from binample!, ISH

Documentation
-------------

This documentation is built using the S-CORE docs-as-code toolchain
(Sphinx + sphinx-needs) with:

.. code-block:: bash

   bazel run //:docs
