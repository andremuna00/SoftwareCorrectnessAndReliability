# 📚 **Software Correctness and Reliability**  

Welcome to the repository for the **Software Correctness and Reliability** course! This repository contains PDF files with exercises and the final project, developed in collaboration with **Simone Jovon**.  

---

## 📘 **Course Overview**  
The main objective of this course is to deepen the understanding of software correctness and reliability techniques through theoretical exercises and practical implementations.

---

## 🏋️ **Exercises**  

![image](https://github.com/user-attachments/assets/5b2c97f2-d576-4e77-869c-70fbb9322462)

### 🔧 **Key Topics Covered**  
1. **Building the Control Flow Graph**  
   - Construct the control flow graph (CFG).  
   - Apply techniques such as *reaching definitions* and *constant folding*.  

2. **Reaching Definition Analysis**  
   - Compute the reaching definitions for the CFG.  
   - Analyze the domain and understand its properties.  

3. **Safe Analysis**  
   - Define what is safe within the analysis and identify potential risks.  

4. **Transfer Functions**  
   - Formalize transfer functions associated with various program statements.  

5. **Interprocedural Control Flow Graph**  
   - Extend the CFG to include interprocedural flows for comprehensive analysis.  

6. **Abstract Domains**  
   - Explore different abstract domains:  
     - **Parity**  
     - **Sign (extended with 0+ and 0-)**  
     - **Intervals**  
     - ...
   - Perform abstract interpretation using the **Domain of Intervals** on a given program.  

---

## 💻 **Final Project**  

![image](https://github.com/user-attachments/assets/011fe7fa-40ee-4030-ad41-dc646eec694d)

### **Objective**  
Enhance the **LiSA (Library for Static Analysis)** capabilities by introducing a new abstract domain: **Pentagons**.

### **Why Pentagons?**  
The pentagon domain offers an intermediate level of precision between **Intervals** and **Octagons**. Its main features include:  
- **Representation**: Handles variables in the form `x ∈ [a, b] ∧ x < y`, where:  
  - `x` and `y` are program variables.  
  - `a` and `b` are rational values.  
- **Applications**:  
  - Verify **array accesses** with greater precision.  
  - Address **array underflows** (`a ≥ 0`).  
  - Confirm **array overflows** (`x < arr.Length`).  
- **Precision**:  
  - More precise than **Intervals** due to symbolic reasoning.  
  - Less precise than **Octagons** as it cannot capture equalities like `x + y == 22`.  

### **Implementation**  
This project is implemented in **Java** and is based on the **LiSA** software framework.  

---

## 📂 **Repository Contents**  
- PDF files covering the theoretical exercises mentioned above.  

---

## 🤝 **Contributors**  
This project was developed by:  
- **Simone Jovon**  
- **Andrea Munarin**  

Feel free to reach out if you have any questions or suggestions!  

---

## 🏆 **Acknowledgments**  
Special thanks to the **Software Correctness and Reliability** course instructors for their guidance and support.  
