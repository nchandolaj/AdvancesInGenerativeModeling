# Embeddings

**Embeddings** are the primary way Modern AI (like Large Language Models) handles representation. For example, "Embeddings", a specific type of representation, are used to help AI understand the meaning of words.


## 1. What is an Embedding?
An embedding is a specific type of **learned representation** where high-dimensional data (like words) is mapped into a lower-dimensional vector space.

Unlike a simple dictionary where every word is just an ID number, an embedding ensures that words with **similar meanings** are placed physically close to each other in this mathematical space.

## 2. Word Embeddings and Vector Math
One of the most famous properties of embeddings is that they allow us to perform "math" on concepts. Because the representation captures semantic relationships, the distance and direction between vectors actually mean something.

The classic example is:
$$\text{King} - \text{Man} + \text{Woman} \approx \text{Queen}$$

In an embedding space:
* The vector for **"King"** and **"Queen"** will be near each other.
* The vector for **"Man"** and **"Woman"** will be near each other.
* The "direction" or relationship between Man and Woman is the same as the direction between King and Queen.

## 3. How Embeddings are Learned
Embeddings are not designed by hand; they are learned during the **Training** phase we discussed earlier.

1.  **Context:** The model looks at millions of sentences. 
2.  **Assumption:** Words that appear in similar contexts probably have similar meanings. (e.g., "The **dog** barked" and "The **hound** barked").
3.  **Update:** The model adjusts the numbers in the word's vector until its internal **Representation** accurately predicts which words are likely to appear next to it.

## 4. Moving Beyond Words: Multimodal Embeddings
Today’s most advanced AI models use **Multimodal Embeddings**. This means the model can represent images, text, and audio in the *same* latent space.

* If you have a picture of a sunset and the word "sunset," their vectors will be very close together in the model's brain.
* This is why you can search for "dog" in your phone's photo gallery even if you never tagged the photos—the model sees the **representation** of the image and recognizes it matches the **representation** of the word.

## Summary of Embeddings

| Feature | Raw Word | Embedding Vector |
| :--- | :--- | :--- |
| **Format** | Text String ("Apple") | List of Numbers ([0.1, -0.5, ...]) |
| **Relational** | No (Apple/Banana are just words) | Yes (Close distance = similar meaning) |
| **Flexibility** | Rigid | Extremely flexible for math & search |

