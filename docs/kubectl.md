# Kubernetes Objects – Simply Explained

## What Are Kubernetes Objects?

In Kubernetes, there are **objects** that define **how a cluster should look**. They store information about **what should run**, **how it should run**, and **how many resources** can be used.

Examples of information stored in an object:
- Which app should run?
- How many copies (replicas) should there be?
- What rules apply (e.g. restart on failure)?

An object is like a **wish list** – Kubernetes calls this the **"desired state"**. Kubernetes takes care of making sure that everything runs exactly as described. If something goes wrong (e.g. a container crashes), it will automatically be fixed.

## How Does Kubernetes Work With That?

Every object has two important parts:
- `spec`: what you want (the desired state)
- `status`: what is actually happening

Kubernetes constantly compares these two and brings the system back to the desired state.

## How Do You Create an Object?

You can create an object using the command line tool **`kubectl`**, for example:

```bash
kubectl apply -f test.yaml
