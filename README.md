# -Audiology---Classifying-2-types-of-hearing-disorders-with-a-Shallow-Neuroph-Neural-Network
In this example, we will use a shallow neural network implemented using the Neuroph framework to classify two types of hearing disorders. Specifically, we'll create a model to classify between two types of hearing loss (e.g., sensorineural hearing loss and conductive hearing loss).
Prerequisites:

    Neuroph Framework: A lightweight Java neural network framework that will be used to implement the shallow neural network.
    Java Development Kit (JDK): To run the Java code.
    Dataset: A dataset containing hearing test data or features (e.g., audiogram results). If you don't have a specific dataset, you can create a synthetic dataset for training and testing.

The steps below assume you already have some audiology data or synthetic features representing the conditions of different types of hearing disorders.
Steps to Build the Shallow Neural Network for Classifying Hearing Disorders:
Step 1: Install and Set Up Neuroph

First, ensure you have Neuroph installed in your project. You can add it using Maven or download the JAR from the Neuroph website.
Maven Dependency for Neuroph (in your pom.xml):

<dependency>
    <groupId>net.sf.neuroph</groupId>
    <artifactId>neuroph-core</artifactId>
    <version>2.9.0</version>
</dependency>

Step 2: Preparing the Dataset

Let's assume you have a dataset with features such as frequency (in Hz), volume level, and hearing test results that correspond to the two types of hearing loss.

For simplicity, let's represent each hearing disorder as two classes:

    0: Sensorineural Hearing Loss
    1: Conductive Hearing Loss

We'll create a simple dataset where we have a few input features and corresponding labels.
Example of Dataset (Features and Labels):
Frequency (Hz)	Volume Level (dB)	Disorder Type (0 or 1)
250	30	0
500	40	0
1000	60	1
2000	70	1
3000	80	0
4000	60	1
Step 3: Code for Classifying Hearing Disorders

The following Java code demonstrates how to use Neuroph to build a shallow neural network to classify the two types of hearing disorders based on audiogram-like features.
Java Code for the Shallow Neural Network:

import org.neuroph.core.Neuron;
import org.neuroph.core.Layer;
import org.neuroph.core.input.WeightedSum;
import org.neuroph.util.NeuronProperties;
import org.neuroph.core.Neuron;

import org.neuroph.core.Layer;
import org.neuroph.core.input.WeightedSum;
import org.neuroph.core.transfer.Sigmoid;
import org.neuroph.core.NeuronProperties;
import org.neuroph.util.NeuronProperties;

import org.neuroph.util.NeuronProperties;

import org.neuroph.util.NeuronProperties;

   import org.neuroph
2 import org.turn Neuron based network assumptions.
