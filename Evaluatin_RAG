# Evaluating a RAG solution
Here’s a well-formatted explanation of traditional retrieval metrics for evaluating a retriever:

---

### **Traditional Retrieval Metrics for Evaluating a Retriever:**

1. **Top-k Accuracy**:
   - **Definition**: Measures whether at least one relevant document is found within the top \(k\) retrieved documents.
   - **Purpose**: This metric evaluates whether the retriever is able to rank relevant documents within the top \(k\) positions.
   
2. **Mean Reciprocal Rank (MRR)**:
   - **Definition**: MRR considers the ranking of the retrieved documents. It is calculated as the average of the **Reciprocal Ranks (RR)** for each query.
   - **Reciprocal Rank (RR)**: The RR is the inverse of the rank position of the **first relevant document**. For example:
     - If the first relevant document is in the third position, the RR is \( \frac{1}{3} \).
   - **Calculation**: MRR is the mean of the RR for all queries.
   - **Interpretation**: A higher MRR indicates that the retriever is better at ranking the most relevant documents higher.
   
   **Example**:
   - Query 1: Relevant document at position 3 → RR = \( \frac{1}{3} \)
   - Query 2: Relevant document at position 1 → RR = 1
   - Query 3: Relevant document at position 4 → RR = \( \frac{1}{4} \)
   - **MRR** = \( \frac{1}{3} \times \left( \frac{1}{3} + 1 + \frac{1}{4} \right) \)

3. **Recall**:
   - **Definition**: Measures the retriever’s ability to retrieve relevant documents from the corpus.
   - **Calculation**: Recall is the ratio of the number of relevant documents successfully retrieved to the total number of relevant documents available.
   - **Interpretation**: A higher recall indicates that the retriever is able to find and retrieve most of the relevant documents.
   
4. **Precision**:
   - **Definition**: Measures the retriever’s ability to retrieve only relevant documents and avoid irrelevant ones.
   - **Calculation**: Precision is the ratio of the number of relevant documents successfully retrieved to the total number of documents retrieved.
   - **Interpretation**: Higher precision means that the retriever is less likely to retrieve irrelevant documents.
   
---

### **Considerations for Chunked Documents:**

- If the documents are **chunked** (i.e., the document is split into smaller pieces), the metrics need to be computed at the **chunk level**.
- **Ground Truth**: The ground truth for evaluating the retriever in this case is a pair consisting of:
  - **Question**
  - **List of relevant document chunks**
  
  Since in many cases, there is only one chunk containing the answer to the question, the ground truth will become a pair of **question** and **relevant document chunk**.

---

This format highlights the definitions, calculations, and interpretations of the evaluation metrics, making it easier to understand each concept and its purpose. Let me know if you'd like further elaboration on any point!
