---
layout: default
title: Setting Up the Development Environment
---

# Setting Up the Development Environment

Before you can start coding in **X++**, it’s essential to set up your development environment. This section will guide you through installing the necessary tools and configuring them to begin your journey with **Dynamics 365 Finance and Supply Chain Management (D365F&SCM)** development.

## Prerequisites

Before proceeding, ensure that you have the following:

1. **Access to Dynamics 365 Finance and Supply Chain Management (D365F&SCM)** development environment.
2. **Microsoft Visual Studio** – the primary IDE used for X++ development.
3. **Microsoft Dynamics Lifecycle Services (LCS)** – used for managing your D365F&SCM environment and deploying packages.
4. **A development or sandbox environment** in D365F&SCM to deploy your code.

## Step 1: Install Microsoft Visual Studio

Visual Studio is the integrated development environment (IDE) used for **X++** programming. To get started, follow these steps to install Visual Studio:

1. Go to the [Visual Studio download page](https://visualstudio.microsoft.com/).
2. Download and install **Visual Studio 2022** (or the version recommended by your D365F&SCM instance).
3. During installation, make sure to select the following workloads:
   - **ASP.NET and web development** (required for web services and APIs).
   - **.NET desktop development** (this will cover general .NET development tasks, including X++ development).
   - **Data storage and processing** (for integration with databases, which will be essential in D365F&SCM development).

Once Visual Studio is installed, you can move on to the next step.

## Step 2: Install the D365F&SCM Development Tools

The next step is to install the **D365F&SCM Development Tools** for Visual Studio. These tools provide all the necessary features for interacting with the **Dynamics 365 Finance and Supply Chain Management** application.

1. Open **Visual Studio**.
2. Go to **Tools** > **Extensions and Updates**.
3. In the Extensions window, search for **Dynamics 365 for Finance and Operations**.
4. Install the **Dynamics 365 for Finance and Operations development tools** extension.

These tools will allow you to interact with the **Application Object Tree (AOT)**, deploy customizations, and work with various D365F&SCM components directly from within Visual Studio.

## Step 3: Set Up the Development Environment in Lifecycle Services (LCS)

To ensure that you’re working in a valid development environment, you need to set up your instance of **Lifecycle Services (LCS)**.

1. Sign in to your **LCS** account at [Lifecycle Services](https://lcs.dynamics.com/).
2. Create a new **Project** or select an existing project if you already have one.
3. In your LCS project, create a **D365F&SCM environment** (typically a sandbox or development environment).
4. After the environment is provisioned, note the **environment URL** and **connection details**.

The **LCS** environment will help you manage the environment where you’ll deploy your customizations and code, ensuring everything is properly linked.

## Step 4: Configure Visual Studio to Connect with D365F&SCM

Once you have the **D365F&SCM Development Tools** installed and your environment set up, you need to connect **Visual Studio** to your **D365F&SCM instance**.

1. Open **Visual Studio**.
2. Go to **Dynamics 365** > **Environment** > **Add a New Environment**.
3. Enter the connection details from your **LCS project** (such as your **Environment URL** and **AOS** details).
4. Click **Connect**. This will allow you to access your D365F&SCM environment directly from Visual Studio.

## Step 5: Set Up the Application Object Tree (AOT)

The **AOT** is an important part of the development environment in **D365F&SCM**. It’s where all the metadata for your environment resides, including tables, classes, and forms. In this step, you'll set up your workspace in Visual Studio to interact with the AOT.

1. In Visual Studio, open the **D365F&SCM** project.
2. In the **Solution Explorer**, you should now see your environment components listed under **Application Object Tree (AOT)**.
3. Navigate to the **AOT** and verify that you have access to all the components you need for development, such as **Tables**, **Classes**, **Forms**, and **Reports**.

## Step 6: Test Your Setup

To ensure everything is set up correctly, try creating a simple **Hello World** X++ job:

1. In Visual Studio, create a new **Dynamics 365 X++ job**.
2. Write the following basic code in the job:
   
   ```static void HelloWorld(Args _args)  
   {  
       info("Hello, X++!");  
   }
3. Build the project and deploy it to your environment.
4. Run the job and check the output in the **Info log** to confirm that everything is working correctly.

If you see the message "Hello, X++!" in the Info log, congratulations! Your development environment is set up and ready for coding.

---

## What’s Next?

Now that you’ve successfully set up your development environment, it’s time to dive into the basics of **X++ Data Types**. Understanding data types is a fundamental part of any programming language, and it’s no different in X++.

In the next section, we’ll explore **X++ Data Types** and how they are used to define variables, manage data, and work with various kinds of information in D365F&SCM.

Let’s move on to [Data Types in X++](data-types.md)!
