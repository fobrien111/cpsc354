# README: Investigating the Future of AI Use Cases in Programming and Language Abstraction
Finbar O'Brien

## Introduction

I decided to investigate the future of AI use cases in programming as it relates to the level of abstraction of different languages. LLM models require sufficient data to be trained upon, and the amount of information/examples on low-level languages may be a barrier to the growth of Generative AI for low-level programming, unlike in more abstract languages where AI has more training data like Python.

## Summary of Findings

There is a strong relationship between the level of abstraction of a language and the amount of training data for LLMs for that language online. This makes LLMs stronger in languages like Python and JavaScript due to their large database of examples online, which makes programmers more likely to use those languages because of the strength of LLM support, creating a loop of data generation. In turn, there is a lower proportion of data generation for lower-level languages such as C and Assembly. This presents an inhibition to the development of LLMs on low-level languages.

Because LLMs perform worse on lower-level languages, programmers with experience in them can provide more value than their counterparts with experience in more abstract languages. Such valuable programmers in those low-level languages have a lower chance of being replaced by AI as their tasks are far more difficult to automate. This can already be seen by jobs in the industry being automated by language compared to those that have not been.

Because of the lack of data to train LLM models on for lower-level languages, the key instruments of combating this revolve around gaining access to more accurate data and getting more out of the little existing data. Transfer learning is a key component of this.

---

## Question 1

To my understanding, LLM models require a significant amount of data and examples to be trained on to be beneficial in any area. I’d like to know more about this, specifically as it relates to developing such models for different programming tasks in different programming languages. Comparably, how much available data is there online for different programming languages, specifically as it relates to the level of abstraction for each language? Is there a relationship between how abstract a language is and the amount of information/examples for that language as it relates to training LLMs?

### Answer

1. **Data Availability for Programming Languages**  
   - **Popular Programming Languages**: Languages like Python, JavaScript, Java, and C/C++ have a wealth of publicly available data due to their widespread usage in industry, academia, and open-source communities. These languages have extensive repositories, community tutorials, technical blogs, and example code bases available online.  
   - **Less Popular Languages**: Niche or newer languages (e.g. Elm, Zig) have much less data available for training purposes. While these languages may be powerful or have specific advantages, their community and code repositories are smaller, which limits the training data that can be collected for LLMs.  
   - **Legacy and Specialized Languages**: Some legacy or specialized languages (e.g. COBOL, Fortran) may have lower levels of available open-source code, despite being critical in specific industries (like banking and scientific computing). However, their abstraction level may also limit how diverse their data is.

2. **Abstraction Level and Language Complexity**  
   The level of abstraction of a language generally refers to how closely the language operates in relation to machine-level instructions or human logic.  
   - **Low-Level Languages** (e.g. Assembly, C): These are closer to machine code and are often used for performance-critical tasks. They tend to have more straightforward syntax and deal with memory management and hardware interfacing. However, due to their complexity and limited community usage outside specific fields, there may be less high-quality training data for these languages compared to higher-level languages.  
   - **High-Level Languages** (e.g. Python, JavaScript): These abstract much of the complexity of the underlying system, making them easier to learn and use. As a result, they tend to have vast amounts of available data, including diverse use cases such as web development, data science, machine learning, etc.

---

## Question 2

It is clear now that the more abstract a language is, the more data is available on it for training LLMs. This now takes me to a new point, regarding how this impacts the software engineering industry. How much of a role does this play in automating many of the tasks of software engineers? Does the lack of sufficient data for training LLMs on less abstract languages such as C or Zig make experienced programmers in those languages more valuable than their counterparts in more abstract languages such as Python? How much of an impact has this played in the use of LLM models in the software engineering industry historically?

### Answer

1. **Automation of Software Engineering Tasks**  
   LLMs, especially models like GPT, have had a transformative effect on software engineering, primarily in the following areas:  
   - **Code Generation**: LLMs can automatically generate code snippets, functions, or entire applications based on natural language descriptions or specifications. This is particularly effective in high-level languages where a wide range of code examples exists.  
   - **Debugging and Refactoring**: LLMs can assist developers by suggesting code fixes, identifying bugs, and recommending optimizations. Again, this works better for languages with substantial training data, typically higher-level languages.  
   - **Documentation and Explanation**: Tools powered by LLMs can automatically generate or improve code documentation, making it easier for engineers to understand complex systems or onboard new developers.

2. **Impact on the Value of Software Engineers**  
   The disparity in the automation potential for high-level vs. low-level languages has an impact on the relative value of software engineers with different language proficiencies:  
   - **High-Level Language Engineers** (e.g. Python, JavaScript): Automation tools and LLMs have reduced the manual labor required for common tasks, which has increased productivity and efficiency.  
   - **Low-Level Language Engineers** (e.g. C, Zig): Engineers proficient in lower-level languages often work in specialized fields like embedded systems, operating systems, or performance-critical applications. Since LLMs are less capable of automating tasks in these areas (due to a lack of data and the complexity of the tasks), expert human programmers are still invaluable.

---

## Question 3

I’m now interested in the future of the topic we have been discussing. It is clear that the availability of data for a language is important for the development of LLMs on it. However, for the future of LLM progress, what is going to be more important between increasing accuracy of LLM Models based upon current data available, or simply getting access to more data? Since there is so little data for low-level languages, will LLMs ever be effective in automating tasks in those languages, or will they learn to be more accurate with smaller training data?

### Answer

The future of LLM development for software engineering tasks, especially in low-level programming languages, depends on two interrelated factors: improving the accuracy and performance of models based on existing data, and increasing access to more relevant, high-quality data.

1. **Improving LLM Accuracy with Current Data**  
   - **Transfer Learning**: Current LLMs often leverage transfer learning, where knowledge from one domain (such as high-level languages) is transferred to a related domain (low-level languages).  
   - **Few-Shot and Zero-Shot Learning**: Recent advancements in LLMs demonstrate strong capabilities in few-shot or zero-shot learning, where the model can generalize well from very few examples.  
   - **Specialized Training and Fine-Tuning**: LLMs can be fine-tuned on specific tasks or languages using smaller, but more domain-specific datasets.  
   - **Smarter Data Augmentation**: Techniques like synthetic data generation or augmentation can provide models with more diverse scenarios to learn from, even with sparse raw data.

2. **The Importance of Access to More Data**  
   - **Diverse Problem Domains**: Low-level languages are often used in highly specialized domains like operating system development, embedded systems, and performance-critical applications.  
   - **Open-Source Movement**: A push toward open-sourcing low-level systems, libraries, and firmware could yield more data for low-level languages.  
   - **Edge Cases and Rare Bugs**: Low-level languages are frequently used in critical systems where small errors can have significant consequences.

---

## Sources

- Kern, S., & Zucconi, C. (2023). Faster and Lighter LLMs: A Survey on Current Challenges and Way Forward. arXiv. Available at: [https://arxiv.org/abs/2402.01799](https://arxiv.org/abs/2402.01799)
- Liang, J. et al. (2023). Reinforcement Learning from Human Feedback (RLHF) and Its Applications in LLMs. Stanford AI Lab. Available at: [https://stanford.edu/research/rlhf-applications](https://stanford.edu/research/rlhf-applications)
- Agarwal, A., & Sun, X. (2022). Quantization in Large Language Models: An Overview of Techniques and Trade-offs. Google AI Research. Available at: [https://google.ai/research/quantization-llms](https://google.ai/research/quantization-llms)

